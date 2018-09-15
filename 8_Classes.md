# 8. Classes

Uma classe define uma estrutura de dados que ira possuir atributos e métodos. A classe adiciona a possiblidade de programar orientado a objetos em Python e facilitam a modoluridade e abstração da complexidade.

## Sintaxe básica

A sintaxe básica de uma classe se dá da seguinte forma:

```python
class Carro: 
    def __init__(self, nome):
        self.nome = nome
        self.__placa = None
        self.__quantidade_de_portas = None
        self.__ligado = False


def main():
    carro1 = Carro("Fusca")
    carro2 = Carro("Uno com escada")
    carro3 = Carro("Brasília")
```

## O método init

No exemplo anterior pode ser observado um método chamado "init", este método é o construtor da classe, sendo envocado toda vez que um novo objeto da classe carro é criado. No exemplo, obrigamos que seja passado o nome do carro para que o objeto seja instanciado.

## Atributos da classe

Os atributos da classe podem ser declarados fora do método init, contudo não é uma boa prática de programação. Recomenda-se criá-los dentro do métodos init.

Para criar atributos privados em Python, colocamos dois underlines antes do atributo.

```python
class Carro: 
    def __init__(self, nome):
        self.nome = nome #Atributo público
        self.__placa = None #Atributo privado
        self.__quantidade_de_portas = None #Atributo privado
        self.__ligado = False #Atributo privado
```


## Declaração de métodos

A declaração de métodos dentro da classe é feita da seguinte forma:

```python
class Carro: 
    def __init__(self, nome):
        self.nome = nome
        self.__placa = None
        self.__quantidade_de_portas = None
        self.__ligado = False
    
    def ligar_carro(self):
        self.__ligado = True
    
    def desligar_carro(self):
        self.__ligado = False
    
    def set_placa(self, placa):
        self.__placa = placa
    
    def get_placa(self,placa):
        return placa
```

Métodos podem ser declarados de maneira privada colocando dois underscores antes da declaração assim como nos atributos

## Sobrecarga de operadores

O python suporta sobrecarga de operadores. Abaixo, segue um exemplo:

```python
class Vetor:
    def __init__(self, numeros):
        self.numeros = numeros
        self.tamanho = len(numeros)
    
    def __add__(self,vetor):
        if self.tamanho == vetor.tamanho:
            novo_numeros = [None] * self.tamanho
            for i in range(self.tamanho):
                novo_numeros[i] = self.numeros[i] + vetor.numeros[i]
            return Vetor(novo_numeros)
                
        else:
            print("Não é possível somar esses dois vetores")
        

def main():
    vetor1 = Vetor([1,2,3,4])
    vetor2 = Vetor([5,6,7,8])
    vetor3 = vetor1 + vetor2
```

é possível utilizar os seguintes operadores em python: 

| Operador | Função | Descrição do método
| ------ | --------- | --------- |
| + | __add__(self,other) | Adição
| * | __mul__(self,other) | Multiplicação
| - | __sub__(self,other) | Subtração
| % | __mod__(self,other) | Resto da divisão
| / | __truediv__(self,other) | Divisão
| < | __lt__(self,other) | Menor que (less than)
| <= | __le__(self,other) | Menor ou igual que (less than or equal to)
| == | __eq__(self,other) | Igual a (equal to)
| != | __ne__(self,other) | Diferente de (not equal to)
| > | __gt__(self,other) | Maior que (Greater than)
| >= | __ge__(self,other) | Maior ou igual que (Greater than or equal to)
| [index] | __getitem__(self,other) | Índice
| in | __contains__(self,value) | Operador de checagem
| len | __len__(self,other) | Número de elementos
| str | __str__(self,other) | Representação em string

<br>