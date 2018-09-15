# 4. Repetições

Algumas vezes, precisamos executar um bloco de código mais de uma vez. Para isso usamos o recurso que conhecemos como repetição.

<br>

## while

`while` nos permite executar um bloco de código **enquanto** uma expressão for verdadeira. Usamos `while` quando não sabemos ao certo quantas vezes a execução precisa ser repetida, e por isso chamamos esse tipo de repetição de *não contada.*

**Exemplo:**

```python
nome = ''
while (nome != 'seu nome')
    print('Por favor, digite seu nome')
    nome = input()
print('Obrigado!')
```


<br>

## for

A repetição `for`, por sua vez, é uma repetição *contada*, executando o código um determinado número de vezes. 

A repetição `for` depende de uma **sequência**, ou seja, uma estrutura que possa ser iterada. A quantidade de vezes que o código será repetido é igual ao número de itens contidos na sequência. Veremos detalhes sobre essas estruturas a seguir.

Por enquanto, usaremos a função `range()`. Ela gera uma sequencia de números com o comprimento desejado.

**Exemplo:**

```python
# imprime os números de 0 a 9
for numero in range(10):
    print(numero)
```

Como veremos adiante, podemos iterar qualquer sequência. 

```python
# imprime cada um dos caracteres da string
for char in 'abcdefgh':
    print(char)
```

<br>

## *Bônus:* range()

Como vimos anteriormente, a função `range()` gera uma sequência numérica com um determinado comprimento. Podemos também definir alguns parâmetros adicionais:

```python
# range(inicio, fim, incremento)

range(0, 10, 1)  # equivalente ao range(10)

range(0, 10, 2)  # gera sequência de 0 a 8 em incrementos de 2

range(10, 0, -1) # gera sequência de 10 a 1
```

<br>

[Sequencias](./5_Sequencias.md)