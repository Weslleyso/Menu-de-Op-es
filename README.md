# Menu-de-Op-es
#Usuário escolhe 2 números e poderá somar, multiplicar, saber quem é maior, trocar números e sair do programa

num1=int(input('insira um número: '))
num2=int(input('insira um número: '))

while True:
    
    escolha = int(input('''
    1 - soma 
    2 - multiplicar
    3 - maior
    4 - novos números
    5 - sair
    sua escolha: '''))
    print('-'*40)

    if escolha == 5:
        print('FIM')
        break
    elif escolha == 1:
        soma = num1 + num2
        print(f'a soma deu {soma}\n')
       
    elif escolha == 2:
        multi= num1*num2
        print(f'a multiplicação deu {multi}\n')
        
    elif escolha == 3:
        if num1>num2:
            print(f'{num1} é maior que {num2}\n')
              
        if num2>num1:
            print(f'{num2} é maior que {num1}\n')
          
        elif num1 == num2:
            print(f'{num1} é igual a {num2}\n')
                               
    elif escolha == 4:
        num1=int(input('insira um número: '))
        num2=int(input('insira um número: '))
