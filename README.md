# primeiro
from random import randint
computador = randint(0,10)
print('Sou seu computador, pensei agora em um número de 0 a 10')
print('Quer tentar adivinhar?')
acertou = False
palpites = 0
while not acertou:
  jogador = int(input('Qual seu palpite:'))
  palpites += 1
  if jogador == computador:
    acertou = True
  else:
    if jogador < computador:
      print('Ainda não, é maior!')
    elif jogador > computador:
      print("continue, é menos!")
print('Boa! Você acertou com {} palpites'. format(palpites))
