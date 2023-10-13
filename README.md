#Alíquota 2023

salario = float(input('Qual seu salário atual? R$'))
porcento = float(input('Quantos % de aumento você gostaria? %'))
newsalario = salario + (salario*porcento/100)
aumento = (newsalario - salario)

#MOSTRA SE TERÁ DE DECLARAR OU NÃO

print('Se atualmente você ganha R${}, com {}% de aumento, passará a ganhar R${:.2f}.'.format(salario, porcento, newsalario))
#print('O salário aumentou em R${:.2f}'.format(aumento))

if newsalario <= 2112:
    desconto = newsalario - (newsalario*7.5/100)
    INSS = newsalario - desconto
    print('Sendo o seu salário total de R${}, você não terá que declarar imposto de renda. \nPorém terá de pagar R${:.2f} de desconto do INSS'.format(newsalario,INSS))

elif newsalario >= 2112.01:
    desconto = newsalario - (newsalario*9/100)
    INSS = newsalario - desconto
    print('Sendo seu salário total de R${}, você terá que declarar R${:.2f} de imposto de renda.'.format(newsalario, INSS))

elif newsalario >= 2826.66:
    desconto = newsalario - (newsalario*15/100)
    INSS = newsalario - desconto
    print('Sendo seu salário total de R${}, você terá que declarar R${:.2f} de imposto de renda.'.format(newsalario, INSS))

elif newsalario >= 3751.06:
    desconto = newsalario - (newsalario*22.5/100)
    INSS = newsalario - desconto
    print('Sendo seu salário total de R${}, você terá que declarar R${:.2f} de imposto de renda.'.format(newsalario, INSS))

elif newsalario >= 4664.68:
    desconto = newsalario - (newsalario*27.5/100)
    INSS = newsalario - desconto
    print('Sendo seu salário total de R${}, você terá que declarar R${:.2f} de imposto de renda.'.format(newsalario, INSS))

