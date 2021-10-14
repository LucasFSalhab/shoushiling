# shoushiling

import random        #Aqui estamos fazendo configurações importante o módulo random para começar!.

random_choice = random.randint(0,2)
if random_choice == 0: 
    computer_choice = 'rock'
elif random_choice == 1:              #O computador escolhe aleatóriamente pedra, papel
    computer_choice = 'paper'         #ou tesoura, gerando um número aleatório de 0 a 2
else:                                 #e, então, o mapeia à string correspondente.
    computer_choice = 'scissors'
    

user_choice = input('rock, paper or scissors? ')     #Obtem a escolha do usuário com uma simples declaração
                                                     #de input.
winner = '' #configura a variável winner

if computer_choice == user_choice:
    winner = 'Tie'
elif computer_choice == 'paper' and user_choice == 'rock':       #Está é a lógica do nosso jogo, que verifica
    winner = 'Computer'                                          #se o computador ganha (ou não) e faz a mudança
elif computer_choice == 'rock' and user_choice == 'scissors':    #adequada na variável winner.
    winner = 'Computer'
elif computer_choice == 'scissors' and user_choice == 'paper':
    winner = 'Computer'
else:
    winner = 'User'
    

if winner == 'Tie':
    print('We both chose', computer_choice + ',play again.')    #Aqui anunciamos que o jogo foi um
else:                                                           #empate, ou o vencedor junto à escolha do
    print(winner, 'won, I chose', computer_choice + '.')        #computador.

    



