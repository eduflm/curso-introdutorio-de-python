# 3. Escrevendo código

Para escrever um programa, precisamos obedecer a algumas regras simples. O conjunto dessas regras é o que chamamos de sintaxe. 
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
<br>

## Blocos

Linhas de código são agrupadas em blocos, o que permite o controle de fluxo do programa.

Em Python, blocos são delimitados pela indentação. Sempre que um bloco é iniciado, avançamos um nível de indentação, e ao final do bloco retornamos um nível.

Cada nível de indentação é geralmente representado por 4 espaços ou um *tab*.

```Python
# exemplo
```

<br>

## Controle de fluxo

O controle de fluxo através dos blocos é feito com o uso de expressões condicionais. As condicionais mais comuns em Python são:

| Palavra chave | Significado |
| ---- | ---------------- |
| if  | SE |
| elif (*else if*) | ENTÃO SE |
| else  | ENTÃO |


Uma condicional é composta de uma palavra chave, uma expressão a ser avaliada e o sinal de dois pontos (`:`), marcando o início de um novo bloco.

Alguns exemplos do uso de condicionais:

```Python
if contador > limite_tempo:
    print('Tempo esgotado!')
```
TODO: diagram de blocos

```Python
if
else
```
TODO: diagram de blocos

```Python
if
elif
else
```
TODO: diagram de blocos

<br>

## *Bônus:* Comentários

Nos exemplos anteriores, vimos linhas de código precedidas pelo símbolo `#`. Essas linhas, que chamamos de comentários, são ignoradas pelo interpretador, e sua única finalidade é documentar um trecho de código.

```Python
# Comentários geralmente são feitos numa linha própria

programa_valido = True    # Mas podem estar na mesma linha do código

# Comentários Podem também ter várias linhas,
# sempre usando a mesma sintaxe.
#
# E podem ter vários parágrafos quando necessário!
```



## Atividade 1*