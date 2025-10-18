[AULA1 - OP ARTIMETICOS E EXPRESSOES - DEV FULL STACK.pdf](https://github.com/user-attachments/files/22985372/AULA1.-.OP.ARTIMETICOS.E.EXPRESSOES.-.DEV.FULL.STACK.pdf)
# Introducao-a-programacao-com-python-aula1-IPP_aula1_lista_de_exercicios_1.ipynb
DESENVOLVIMENTO FULL STACK - EXERCÍCIOS - PUC-RIO



# Roteiro da terceira lista de exercícios
# Aula: Introdução à linguagem Python
# Puc-Rio
# Disciplina: Desevolvimento Full Stack
# Professor: José Carlos Ramalho Moreira

# Desafio 1: Crie uma variável com seu nome e exiba a quantidade de caracteres armazenados na variável.


nome = "Tiago"
print(len(nome))

# Desafio 2: Crie uma variável com uma string representando a data de seu nascimento no formato 'dd/mm/aaaa'. Em seguida, crie e exiba uma senha composta pela concatenção das partes definidas abaixo, na ordem apresentada:

# último caractere do ano;
# 1o. caractere do mês replicado 5 vezes;
# 2o. caractere do dia;
# 2o. caractere do ano replicado 2 vezes.

data_nascimento = '13/09/1990'  # A string tem 10 caracteres

data_nascimento[-1]  # último caractere do ano: '0'
data_nascimento[9] * 5  # 1o. caractere do mês replicado 5 vezes: '00000'
data_nascimento[0]  # 2o. caractere do dia: '1'
data_nascimento[9] * 2  # 2o. caractere do ano replicado 2 vezes: '00'


senha = data_nascimento[-1] + data_nascimento[9] * 5 + data_nascimento[0] + data_nascimento[9] * 2
print(senha)  # Saída: 00010


# Desafio 3: Agora vamos criar uma senha mais forte! Crie uma variável com uma string representando a data de seu nascimento no formato 'dd/mm/aaaa'. Crie outra variável com o seu nome. Em seguida, crie e exiba uma senha composta pela concatenção das partes definidas abaixo, na ordem apresentada:

# penúltimo caractere do ano;
# caractere '#';
# caractere do meio do nome;
# 2o. caractere do mês replicada 3 vezes;
# caractere '$';
# antepenúltimo caractere do nome replicado 2 vezes.

data_nascimento = '13/09/1990'
nome = 'Tiago'

# 1. Penúltimo caractere do ano
penultimo_ano = data_nascimento[-2]  # '9'

# 2. Caractere '#'
simbolo1 = '#'

# 3. Caractere do meio do nome
nome = 'Tiago'  # 5 letras
meio_nome = nome[2]  # índice fixo para o meio
print(meio_nome)  # Saída: 'a'



# 4. Segundo caractere do mês replicado 3 vezes
segundo_mes = data_nascimento[4] * 3  # '9' * 3  = '999'

# 5. Caractere '$'
simbolo2 = '$'


# 6. Antepenúltimo caractere do nome replicado 2 vezes
antepenultimo_nome = nome[-3] * 2  # 'a' * 2

# Montando a senha
senha_forte = penultimo_ano + simbolo1 + meio_nome + segundo_mes + simbolo2 + antepenultimo_nome
print(senha_forte)  # Saída: 9#a999$aa

#DESAFIO 4**

#Crie uma variável string com todas as letras maiúsculas do alfabeto, de 'A' a 'Z'. Em seguida, crie uma variável lista com os valores inteiros 15, 24, 19, 7, 14 e 13. Considerando que cada inteiro da lista corresponde ao índice da posição de uma letra na string, exiba a concatenação de todas as 6 letras e descubra a "palavra secreta".
#Por exemplo, se a lista possuir os valores 14 e 0, a palavra secreta será 'OI'.

alfabeto = "ABCDEFGHIJKLMNOPQRSTUVWXYZ"
indices = [15, 24, 19, 7, 14, 13]   
letra1 = alfabeto[15]  # 'P'
letra2 = alfabeto[24]  # 'Y'
letra3 = alfabeto[19]  # 'T'
letra4 = alfabeto[7]   # 'H'   
letra5 = alfabeto[14]  # 'O'
letra6 = alfabeto[13]  # 'N'     


palavra_secreta = "letra1 + letra2 + letra3 + letra4 + letra5 + letra6"
print(palavra_secreta)  # Saída: PYTHON    


