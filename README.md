# Exerci769cio-5-_Func807o771es_em_Python
Exercício Funções em Python
UNIVERSIDADE FEDERAL RURAL DA AMAZÔNIA INSTITUTO CIBERESPACIAL 
 

DISCIPLINA: TÉCNICAS DE PROGRAMAÇÃO I 
DOCENTE: EDVAR DA LUZ OLIVEIRA 
Discente: Maria Cristina Dantas de Sousa

Exercício Funções em Python 
 
Questão 1: Crie uma função chamada soma_pares que recebe uma sequência de números e retorna a soma dos números pares. 
Resposta: 
def soma_pares(seq):
    return sum (num for num in seq if num % 2 == 0)
numeros = [1, 2, 3, 4, 5, 6]
print(soma_pares(numeros))  

Saída: 12

Obs.:   12, que é a soma de 2, 4 e 6

 
Questão 2: Escreva uma função chamada eh_primo que recebe um número e retorna True se ele for primo e false caso contrário. 
Resposta:
def eh_primo(num):
    if num < 2:
        return false
    for i in range (2, int(num**0.5) + 1):
        if num % i == 0:
            return false
    return True

print (eh_primo (7)) 
print (eh_primo (4))


 Saída: True
     False

Obs.: retorna True porque 7 é um número primo. 7 é maior que 2 e não é divisível por nenhum número entre 2 e 7. Portanto, a função retorna True.

retorna false porque 4 não é um número primo. 4 é divisível por 2. Portanto, a função retorna false.


Questão 3: Crie uma função chamada inverte_palavra que recebe uma string e retorna a string invertida. 
Resposta: 
def inverte_palavra(palavra):
    return palavra[::-1]

print(inverte_palavra('palavra')) 

Saída: arvalap

Obs.: 'arvalap', que é 'palavra' invertida



 
Questão 4: Implemente uma função chamada calcula_fatorial que recebe um número inteiro positivo e retorna o fatorial desse número. 
Resposta: 
def calcula_fatorial(num):
    if num == 0:
        return 1
    else:
        return num * calcula_fatorial(num-1)

 print (calcula_fatorial (5)) 


Saida: 
120

Obs.:  120, que é o fatorial de 5
 
Questão 5: Crie uma função chamada conta_vogais que recebe uma string e retorna a contagem de vogais (a, e, i, o, u) na string. 
Resposta: 
def conta_vogais(s):
    return sum (s. Count(vogal) for vogal in 'aeiou')
 
 print(conta_vogais('palavra'))  

 Saida: 
         3
3, que é a quantidade de vogais em 'palavra'
	  
Resoluções 
 
Questão 1: 
 
def soma_pares(*numeros): 
    return sum(num for num in numeros if num % 2 == 0) 
 
resultado = soma_pares(1, 2, 3, 4, 5, 6) 
print(resultado)  # Deve imprimir 12 
 
 
Questão 2: 
 
def eh_primo(numero):     if numero < 2:         return False     for i in range(2, int(numero**0.5) + 1): 
        if numero % i == 0:             return False     return True 
 
resultado = eh_primo(11) 
print(resultado)  # Deve imprimir True 
 
Questão 3: 
 
def inverte_palavra(palavra): 
    return palavra[::-1] 
 
resultado = inverte_palavra("python") 
print(resultado)  # "nohtyp" 
 
Questão 4: 
def calcula_fatorial(numero):     if numero == 0 or numero == 1:         return 1 
    return numero * calcula_fatorial(numero - 1) 
 
resultado = calcula_fatorial(5) print(resultado)  # Deve imprimir 120 
 
Questão 5: 
def conta_vogais(frase): 
    return sum(1 for char in frase if char.lower() in 'aeiou') 
 
resultado = conta_vogais("hello world") print(resultado)  # Deve imprimir 3 
