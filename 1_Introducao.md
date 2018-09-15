# 1. Introdução

<br>

## Porque Python?

**Sintaxe simples e elegante:** facilita o aprendizado, simplifica a solução de problemas e aumenta a produtividade do programador.

**Excepcionalmente bem planejada**, o que faz dela uma linguagem consistente.

**Ampla gama de aplicações**. Uma das linguagem favoritas para web, redes, segurança, análise e processamento de dados, inteligência artificial, e claro, scripting.

**Código aberto**, sua licença garante a liberdade de uso e distribuição.
<br>
<br>
## Um pouco de contexto

Criada no final da década de 80 pelo holandês **Guido van Rossum**, na época pesquisador do CWI, onde permaneceu até pouco depois do lançamento da versão 1.0 da linguagem, em 1994. 

Guido reuniu uma pequena equipe de desenvolvedores e  continuou a trabalhar na linguagem, passando por institutos de pesquisa e empresas até o lançamento da versão 2, em 2000, quando o desenvolvimento passou a ter maior participação da comunidade.

A versão 3 foi lançada em 2008 para corrigir falhas de projeto da linguagem, e não é compatível com as versões anteriores.

Atualmente a linguagem é mantida pela **Python Software Foundation** e se encontra na versão 3.7, enquanto alguns recursos ainda são portados para a versão 2, mantida como legado. 
<br>
<br>

## *Bônus:* Conhecendo o IDLE

Um interpretador Python é incluso na maioria dos sistemas operacionais que atendem ao padrão POSIX (Linux e OSX). O download da versão mais recente do interpretador pode ser baixado em [python.org/downloads](python.org/downloads). 

O download inclui também um editor de texto chamado IDLE, que usaremos no curso.

Para abrir o IDLE, digite no seu terminal:

```
idle3
```

Ao abrir o IDLE é exibida uma janela com o que chamamos de shell interativo. Nele podemos executar um código Python linha a linha, o que é útil para rascunhar programas curtos.

Temos também a opção de criar um novo arquivo (`Arquivo > Novo Arquivo`) e escrever o programa nele. Para executar o arquivo, basta selecionar a opção `Executar > Executar módulo`.

Como um primeiro exercício, crie um novo arquivo no IDLE, digite e execute o programa abaixo (não se preocupe ainda em entender como ele funciona):

```python
nome = input('Digite seu nome: ')
print('Olá, ' + nome)
```
<br>

[Representando dados](./2_Representando_dados.md)
