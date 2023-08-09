# Exercicio099.py

from time import sleep
def maior(*num):
    cont = maior = 0
    print('-='*30)
    print('ANALISANDO OS RESULTADOS....')
    for valor in num:
        print(f'{valor}', end=' ', flush=True)
        sleep(0.3)
        if cont == 0:
            maior = valor
        else:
            if valor > maior:
                maior = valor
        cont += 1
        print(f'Foram informados {cont} valores ao todo. ')
        print(f'O maior valor informado foi {maior}. ')


maior(1,2,3,4,5)
maior(3,3)
maior(5,5)
