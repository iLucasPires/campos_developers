# Campos_developers aula 05

Neste quinto dia de curso, aprendemos um pouco sobre pre-commit, aonde podemos usar a ferramenta, para resolver problemas de qualidade de código, e como configurar o pre-commit.

## Resumo do dia anterio

Relembrando o que aprendemos na aula anterior:

- Aprendemos um pouco sobre gitflow, a sua vantagens e desvantagens, e o fluxo de trabalho.
- Aprendemos sobre branches e como elas funcionam
- Aprendemos algumas alternativas ao gitflow

## O que vamos aprender hoje

**OBS:** Nós vamos precisa do nosso ambiente virtual para usar o pre-commit, então se você não tiver o seu ambiente virtual, crie um seguindo o tutorial da [aula 03](../aula03/README.md).

- [flake8](#flake8)
  - [Instalação do flake8](#instalação-do-flake8)
  - [Rodando o flake8](#rodando-o-flake8)
- [Black](#black)
  - [Instalação do Black](#instalação-do-black)
  - [Rodando o Black](#rodando-o-black)
- [Pre-commit](#pre-commit)
  - [Instalação do pre-commit](#instalação-do-pre-commit)
  - [Configurando o pre-commit](#configurando-o-pre-commit)
  - [Rodando o pre-commit](#rodando-o-pre-commit)
  - [Desinstalando o pre-commit](#desinstalando-o-pre-commit)



## flake8

O flake8 é uma ferramenta que verifica a qualidade do código, ele verifica se o código está de acordo com o padrão PEP8, e também verifica se o código está com algum erro de sintaxe.

- ### Instalação do flake8

    Para instalar o flake8, basta executar o seguinte comando:

    ```bash
    pip install flake8
    ```

- ### Rodando o flake8

    para rodar o flake8, basta executar o seguinte comando:

    ```bash
    flake8 <nome_do_arquivo>
    ```

## Black

O Black é uma ferramenta que formata o código para o padrão PEP8, ele formata o código de acordo com o padrão PEP8, e também verifica se o código está com algum erro de sintaxe.

- ### Instalação do Black

    Para instalar o Black, basta executar o seguinte comando:

    ```bash
    pip install black
    ```

- ### Rodando o Black

    para rodar o Black, basta executar o seguinte comando:

    ```bash
    black <nome_do_arquivo>
    ```

## Pre-commit

O pre-commit é uma ferramenta que executa comandos antes de cada commit, ele é muito útil para verificar a qualidade do código antes de cada commit, e assim evitar que o código com erros vá para o repositório.

- ### Instalação do pre-commit

    Para instalar o pre-commit, basta executar o seguinte comando:

    ```bash
    pip install pre-commit
    ```

- ### Configurando o pre-commit

    Para configurar o pre-commit, basta executar o seguinte comando:

    ```bash
    pre-commit install
    ```

    Após executar o comando, o pre-commit vai criar um arquivo chamado `.pre-commit-config.yaml` na raiz do seu projeto.
    Esse arquivo é o arquivo de configuração do pre-commit, e nele você pode configurar quais comandos serão executados antes de cada commit.

    **OBS:** Nesse repositório tem um arquivo de configuração do pre-commit,usando o flake8 e o black, você pode usar esse arquivo de configuração, ou criar o seu próprio.

- ### Rodando o pre-commit

    O pre-commit é executado automaticamente antes de cada commit, então não é necessário executar o pre-commit manualmente.

- ### Desinstalando o pre-commit

    Para desinstalar o pre-commit, basta executar o seguinte comando:

    ```bash
    pre-commit uninstall
    ```
