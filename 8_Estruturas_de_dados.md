# 8. Estruturas de dados

Estruturas de dados são agrupamentos que permitem representar e organizar informações muito além do que seria possível com tipos de dados simples. 

Python possui um poderoso conjunto de estruturas de dados (também conhecidas como *containers*) embutidas na linguagem. Algumas delas foram vistas anteriormente: listas e tuplas são casos especiais de estruturas de dados com caractetísticas em comum. 

A seguir veremos outras das principais estruturas da linguagem.
<br>

## Conjuntos (sets)

Conjuntos em Python possuem as mesmas características de seus equivalentes matemáticos: não possuem ordem definida nem elementos duplicados. Também possuem operações como união, interseção e diferença.

**Declaração**
```python
conjunto = {1, 2, 3}
```
```python
# declaração de conjunto vazio
conjunto = set() 
```
`set()` também pode ser usado para gerar um conjunto a partir de uma sequência.
<br>

**Exemplos:**
```python
# teste de pertencimento
cesta = {'maça', 'banana', 'maça', 'laranja'}
'laranja' in cesta
```
```python
# remoção de itens duplicados de uma lista
nova_lista = list(set(uma_lista))
```
```python
# remoção de caracteres repetidos em uma string
set('abracadabra')
```
<br>

**Métodos**
| Método | Resultado |
| ------ | --------- |
| .add(n) | Adiciona um elemento ao conjunto |
| .union(cj) | Retorna um conjunto com os elementos de ambos |
| .intersection(cj) | Retorna conjunto com elementos comuns a ambos |
| .difference(cj) | Retorna a conjunto com a diferença entre ambos |
| .symmetric_difference(cj) | Retorna conjunto com elementos não comuns |
| .isdisjoint(cj) | Retorna True se a interseção é vazia |
| .issubset(cj) | Retorna True se um conjunto está contido no outro |
| .issuperset(cj) | Retorna True se um conjunto contém no outro |
| .copy() | Retorna uma cópia do conjunto |
| len() | Retorna o número de elementos do conjunto (cardinalidade) |

Alguns desses métodos possuem um operador equivalente:

| Operador | Equivalente |
| -------- | ----------- |
| A \| B | A.union(B) |
| A & B | A.intersection(B) |
| A - B | A.difference(B) |
| A ^ B | A.symmetric_difference(B) |
| A < B | A.issubset(B) |
| A > B | A.issuperset(B) |


<br>

## Dicionários

Dicionários são estruturas similares a sequências, porém cada *valor* possui uma chave ao invés de um índice. Cada chave está associada a um único valor, formando o que chamamos de um *par chave-valor*. Chaves podem ser valores numéricos, strings ou qualquer outro tipo *imutável*. 

Assim como conjuntos, dicionários também não possuem uma ordem definida.

**Declaração**

```python
# declaração de um dicionario vazio
dicionario = {}
```
```python
gato = {'tamanho': 'grande', 'cor': 'cinza'}
```
**Acesso**
```python
gato['cor']
```
Dicionários usam uma técnica conhecida como *hashing* na associação dos pares, o que otimiza a busca de itens em relação a outras sequências.  

**Adição**
```python
dicionario['nova_chave'] = 'novo_valor'
```

**Remoção**
```python
del dicionario['nova_chave']
```

**Métodos**
| Método | Resultado |
| ------ | --------- |
| .get(chave) | Retorna o valor associado ou None caso não exista|
| .pop(chave) | Retorna o valor associado e remove o par do dicionário |
| .clear() | Apaga todos os pares chave-valor |
| .copy() | Retorna uma cópia do dicionário |
| .items() | Retorna uma *visualização* dos pares do dicionário |
| .keys() | Retorna uma *visualização* das chaves do dicionário |
| .values() | Retorna uma *visualização* dos valores do dicionário |

**Iteração**
Para iterar por um dicionário, o par chave-valor pode ser obtido simultaneamente com o uso do método items().
```python
knights = {'gallahad': 'the pure', 'robin': 'the brave'}
for chave, valor in knights.items():
    print(chave, valor)
```

<br>

[Próximo capítulo](./9_Funcoes_.md)