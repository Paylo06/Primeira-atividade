Aqui eu mostro como eu faço para abrir o arquivo pelo Ubuntu (Versão 2026)

pwd (para saber em qual diretorio eu estou)

cd /home/joaop/modulo1/linux (Onde está o arquivo da minha atividade)

nano nome python_script.sh (para abri-lô, mas é o mesmo codigo para criar um arquivo também)

---coloquei isso dentro do script---

#!/bin/bash

sudo apt update

sudo apt install python3

python3 /home/joaop/modulo1/linux/nome.py

--------------------------------------------

./python_script.sh (para executa-lo)

--------------------------------------------

Esse arquivo ele faz a atualização automática do python no meu Ubuntu, e também abre outro arquivo no formato python (versão 3), que pede para escrever o nome de quem abriu o arquivo, o código está descrito logo abaixo:

nome = input ('digite seu nome')

print('seja bem vindo, parceiro', nome)

Ele é bem simples, um nome = input com o texto "digite seu nome", para que qualquer pessoa que abrir o arquivo possa digitar seu próprio nome, é um print com o texto "Seja bem vindo, parceiro", com o dado 'nome' que foi guardado na memoria com o nome digitado por quem abre o arquivo.

(Para além disso coloquei também a minha primeira atividade, que não se torna necessaria grandes explicações sobre mas abaixo vou explica-la, esta denominada como primeira_atividade.ipynb)

print("Vamos fazer algumas operações, digite dois valores logo abaixo: ")

valor1 = input ("Primeiro valor: ")
valor1 = int(valor1)

print("\n")

valor2 = input ("Segundo valor: ")
valor2 = int(valor2)
2

soma = valor1 + valor2
subtracao = valor1 - valor2
multiplicacao = valor1 * valor2
divisao = valor1 / valor2
resto_div = valor1 % valor2

print(f"Essa é a soma dos dois valores: {soma}")
print(soma)
print(f"Essa é a subtração dos dois valores: {subtracao}")
print(subtracao)
print(f"Essa é a multiplicação dos dois valores: {multiplicacao}")
print(multiplicacao)
print(f"Essa é a divisão dos dois valores: {divisao}")
print(divisao)
print(f"Essa é o resto da divisao dos dois valores: {resto_div}")
print(resto_div)

Essas primeiras linhas fazem contas basicas como, adição, subtração, multiplicação, divisão e resto de divisão

--

Aqui temos a segunda parte que é um loop de uma operação de soma, que ira parar quando o numero escolhido pelo usuário for maior que o total ja definido, ou a soma feita posteriormente for igual ou maior, tendo uma mensagem para cada tipo de resposta final.

print("Vamos fazer uma operação que  seja maior que o total: ")

total = 200

valor = input ("Digite o valor desejado: ")
valor = int(valor)

while valor < total:
  print(f"vamos somar pois o {valor} não é maior que o {total}")
  somador = input ("Digite o valor desejado para somar: ")
  somador = int(somador)
  valor += somador
  print(f"O valor atual é: {valor}")


if valor > total:
  print(f"O valor atual de, {valor} é maior que o total")
else:
  print(f"O valor {valor}, é igual ao valor total de {total}, ")
