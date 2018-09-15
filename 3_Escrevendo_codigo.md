# 3. Escrevendo código

Para escrever um texto, precisamos observar o conjunto conjunto de regras da língua portuguesa, que chamamos de sintaxe. De forma semelhante, ao escrever um programa precisamos observar a sintaxe do Python,  para que ele seja interpretado corretamente. Do contrário o interpretador nos retornará uma mensagem de erro.

<br>

## Expressões

Uma expressão é a menor divisão possível de um programa.

Ela é composta de valores e operadores, e após ser avaliada pelo interpretador ela retorna um único valor ao programa.

```Python
2 ** 3          # retorna 8
```
```Python
0 == False      # retorna True
```
```Python
True and False  # retorna False
```
Uma expressão também pode ser composta de outras expressões.

```Python
(2 + 2) * 3     # retorna 12
```
O valor resultante de uma operação pode ser facilmente testado usando o interpretador interativo.

<br>

## Controle de fluxo

A execução do programa pelo interpretador é feita linha a linha, de cima para baixo. Frequentemente, porém, é necessário controlar o fluxo do programa, executando trechos de código apenas quando uma determinada condição é atendida. 

A seguir veremos recursos que permitem esse controle.

## Blocos

Blocos são agrupamentos de linhas de código, e são essenciais para o controle de fluxo. 

Em Python, blocos são delimitados pela indentação. Sempre que um bloco é iniciado, avançamos um nível de indentação, e ao final do bloco retornamos um nível.

Cada nível de indentação é geralmente representado por 4 espaços ou um *tab*.

```Python
numero = int(input('Digite um número: '))
if numero % 2 == 0 :
    print('O número é par!')
else:
    print('O número é impar')
```
<br>

## Expressões condicionais

Outro recurso essencial para o controle de fluxo são as expressões condicionais. Elas permitem que um bloco de código seja ou não executado, de acordo com o resultado de uma expressão.

As condicionais mais comuns em Python são:

| Palavra chave | Significado |
| ---- | ---------------- |
| if  | SE |
| elif (*else if*) | ENTÃO SE |
| else  | ENTÃO |


Uma condicional é composta de uma palavra chave, uma expressão a ser avaliada e o sinal de dois pontos (`:`), marcando o início de um novo bloco (e um novo nível de indentação).

Alguns exemplos do uso de condicionais:

```Python
if numero > 0:
    print('Número positivo!')
elif numero < 0:
    print('Número negativo!')
else:
    print("O número é zero")
```


```Python
if
else
```


```Python
if
elif
else
```
<br>

## *Bônus:* Comentários

Nos exemplos anteriores, vimos linhas de código precedidas pelo símbolo `#`. Essas linhas, que chamamos de comentários, são ignoradas pelo interpretador, e sua única finalidade é documentar um trecho de código.

```Python
# Comentários geralmente são feitos numa linha própria

aprendendo_python = True    # Mas podem estar na mesma linha do código

# Comentários Podem também ter várias linhas,
# sempre usando a mesma sintaxe.
#
# E podem ter vários parágrafos quando necessário!

''' E nem sempre é necessário colocar
o simbolo de comentário em todas as linhas
podemos fazer um comentário multilinhas utilziando
três aspas simples no início e no final do comentário'''
```

<br>

[Repetições](./4_Repeticoes.md)

