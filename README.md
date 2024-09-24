# agencia_programa
tamanho = int
valor_total = float
recorte = int

#Trecho para escolher a opção do serviço
op = int(input( 'Entre com a opção desejada: ' ))


servico = op
match servico:
        case 1:
            print('Impressão Digital')
            papel = int(input('Entre com a quandidade de impressão: '))          

            valor_papel = papel * 8
            print(f'O valor total de impressão é R$: {valor_papel:,.0f}')
        
        case 2:
            print('Impressão Plotter')
            op_p = int(input('Entre com a opção: '))
            servico_1 = op_p

            match servico_1:
                case 1:
                    print('Adesivo')
                      
                case 2:
                    print('Banner')
                    altura_lona = float(input('Entre com a altura do banner em cm: '))
                    largura_lona = float(input('Entre com a largura do banner em cm: '))

            tamanho = altura_lona * largura_lona
            metro = tamanho / 100
            print(f'O tamanho total do banner é: {metro:,.0f} ')


                    #condição pra saber se o valor cai no mínimo
            if tamanho <= 100.0:
                    valor_total = 40.0
                    print(f'Valor da lona entra no valor mínino R$: {valor_total:,.2f}')

                    
            else:
                    valor_total = (tamanho * 40.0) / 100

                    #função para arrendondar valor
                    valor_arredondado = lambda valor_total: round (valor_total,2)
                    arredondado = valor_arredondado (valor_total)  
                    print(f'O valor total do Banner R$: {arredondado:,.2f}')

        case 3:
            print('Recorte')
            
            op_r = int(input('\n 1-Recorte Especial \n 2-Corte Reto \n Entre com a opção:'))
            servico_recorte = op_r

            match servico_recorte:
                case 1:
                    print('O Valor é R$: ')
                      
                case 2:
                    print('O Valor é R$: ')
                    

            
            

  

            

         
