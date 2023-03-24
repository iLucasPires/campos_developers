# Campos_developers aula 03

Neste terceiro dia de curso, aprendemos um pouco de tipo de dados em Python e notebooks Jupyter.

## Resumo do dia anterior

Relembrando o que aprendemos na aula anterior:

- Aprendemos usar git branches para desenvolver novas funcionalidades isoladas umas das outras.
- Aprendemos o conceito de git flow, que é um fluxo de trabalho para projetos que usam git branches.

Agora com esses conceitos em mente, vamos aprender um pouco sobre Python.

## Oque vamos aprender hoje?

- [Tipos de dados](#tipos-de-dados)
  - [Exemplos](#exemplos)
    - [Inteiros](#inteiros)
    - [Ponto flutuante](#ponto-flutuante)
    - [Strings](#strings)
    - [Booleanos](#booleanos)
- [Ambiente virtual](#ambiente-virtual)
- [Notebooks Jupyter](#notebook-jupyter)

## Python

Python é uma linguagem de programação de alto nível, interpretada, de script, imperativa, orientada a objetos, funcional, de tipagem dinâmica e forte, que suporta múltiplos paradigmas de programação, incluindo programação orientada a objetos, programação imperativa e, em menor grau, programação funcional.


## Modo interativo

O modo interativo do Python é uma ferramenta que permite que você escreva e execute código Python diretamente no terminal.

Para entrar no modo interativo, basta digitar `python` no terminal.

```bash
python # entra no modo interativo
```

Voce deve ver algo parecido com isso:

```bash
Python 3.10.6 (main, Nov 14 2022, 16:10:14) [GCC 11.3.0] on linux
Type "help", "copyright", "credits" or "license" for more information.
>>> # aqui você pode escrever e executar código Python diretamente no terminal
```

Vamos começar a brincar com o Python no modo interativo, para ver os tipos de dados que ele possui, vamos usar a função `type` para verificar o tipo de dado de uma variável.

## Tipos de dados

Python possui os seguintes tipos de dados:

- `int`: números inteiros (números sem casas decimais)
- `float`: números decimais (números com casas decimais)
- `str`: strings (texto)
- `bool`: booleanos (valores `True` ou `False`)

### Exemplos

#### Inteiros

vamos criar uma variável chamada `numero` e atribuir o valor 1 a ela

se nós usar a função `type` para verificar o tipo de dado da variável `numero`, veremos que o tipo de dado é `int`

```python
>>> numero = 1 # atribui o valor 1 a variável numero
>>> type(numero) # verifica o tipo de dado da variável numero
<class 'int'> # a função type retorna o tipo de dado da variável
```

#### Ponto flutuante

vamos criar uma variável chamada `numero` e atribuir o valor 1.0 a ela

se nós usar a função `type` para verificar o tipo de dado da variável `numero`, veremos que o tipo de dado é `float`

```python
>>> numero = 1.0 # atribui o valor 1.0 a variável numero
>>> type(numero) # verifica o tipo de dado da variável numero
<class 'float'> # a função type retorna o tipo de dado da variável
```

#### Strings

Vamos criar uma variável chamada `numero` e atribuir o valor "1" a ela, note que o valor da variável `numero` é uma string, mesmo que o valor dela seja um número, pois o valor foi colocado entre aspas simples ou duplas.

se nós usar a função `type` para verificar o tipo de dado da variável `numero`, veremos que o tipo de dado é `str`

**OBS:** O Python diferencia letras maiúsculas de minúsculas, ou seja, `A` é diferente de `a`.

```python
>>> numero = "1" # atribui o valor "1" a variável numero
>>> type(numero) # verifica o tipo de dado da variável numero

<class 'str'> # a função type retorna o tipo de dado da variável
```

#### Booleanos

Vamos criar uma variável chamada `numero` e atribuir o valor `True` a ela, note que o valor da variável `numero` é um booleano, pois o valor é `True` ou `False`.

se nós usar a função `type` para verificar o tipo de dado da variável `numero`, veremos que o tipo de dado é `bool`

```python
>>> numero = True # atribui o valor True a variável numero
>>> type(numero) # verifica o tipo de dado da variável numero
<class 'bool'> # a função type retorna o tipo de dado da variável
```

Existem alguns tipos de dados que são compostos, ou seja, eles são formados por outros tipos de dados, mas vamos falar sobre eles em outra aula.

**OBS:** Para sair do modo interativo do Python, basta digitar `exit()` ou `quit()`.

## Ambiente Virtual

Ambiente virtual é um ambiente isolado que permite que você instale pacotes Python sem afetar o ambiente global do Python, ou seja, você pode instalar pacotes Python em um ambiente virtual sem afetar o ambiente global do Python.

Para criar um ambiente virtual, basta usar o comando `python -m venv <nome_do_ambiente>`.

```bash
python -m venv venv # cria um ambiente virtual chamado venv
# ou
virtualenv venv # cria um ambiente virtual chamado venv
# neste caso, você precisa ter o pacote virtualenv instalado, caso não tenha, use o comando pip install virtualenv
```

Para ativar o ambiente virtual, basta usar o comando `source <nome_do_ambiente>/bin/activate`, no caso do Linux e MacOS, ou `source <nome_do_ambiente>/Scripts/activate`, no caso do Windows, caso você esteja usando o PowerShell, use `.\venv\Scripts\Activate`.

```bash
source venv/bin/activate # ativa o ambiente virtual venv no Linux
source venv/Scripts/activate # ativa o ambiente virtual venv no Windows
# ou
.\venv\Scripts\Activate # ativa o ambiente virtual venv no PowerShell

(venv) # o nome do ambiente virtual aparece entre parênteses
```

caso o comando venv não esteja disponível ou esta tento algum problema, você pode tentar usar o pip para instalar o pacote virtualenv, e depois usar o comando virtualenv para criar o ambiente virtual.

```bash
pip install virtualenv # ou pip3, esse comando instala o pacote virtualenv
virtualenv venv # cria um ambiente virtual chamado venv

# e repita os passos para ativar o ambiente virtual
```

**OBS:** Caso ainda esteja tendo problemas entre em contato comigo, posso tentar ajudar, tem o meu discord no readme do meu perfil.

## Notebook Jupyter

Notebooks Jupyter é uma aplicação web que permite criar e compartilhar documentos que contém código, equações, visualizações e texto explicativo.

Podemos usar o Google Colab para criar notebooks Jupyter, para isso, basta acessar o link
[https://colab.research.google.com/](https://colab.research.google.com/) e criar um novo notebook.

Ou local, como estamos usando o visual studio code, podemos instalar a extensão Jupyter, para isso, basta acessar o menu de extensões do visual studio code, pesquisar por Jupyter e instalar a extensão.

**OBS:** Lembre-se de ativar o ambiente virtual antes de instalar a extensão Jupyter.

agora podemos criar uma arquivo com a extensão `.ipynb`, que o visual studio code vai reconhecer como um notebook Jupyter, e vai pedir para instalar as dependências do notebook Jupyter.

agora podemos criar um novo notebook Jupyter, clicando no botão `+ Code` no canto superior esquerdo da tela.

e podemos escrever código Python no notebook Jupyter, como se estivéssemos usando o modo interativo do Python, depois de escrever o código, podemos executar o código clicando no botão `Run` no canto superior esquerdo da tela.

**OBS:** provalmente ele vai pedir para selecionar o virtualenv que você quer usar, selecione o virtualenv que você criou, e depois vai pedir para instalar as dependências do notebook Jupyter, clique em `Install`.
