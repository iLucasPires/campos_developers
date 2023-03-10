# Campos_developers aula 02

Neste segundo dia de curso, aprendemos novos comandos Git e o conceito de Branches.

## Resumo do dia anterior

relembrando o que aprendemos na aula anterior:

- aprendemos a instalar e usar as principais ferramentas que vamos usar durante o curso. São elas:
  - [Liguagem Python](https://www.python.org/)
  - [Versionador de código Git](https://git-scm.com/)
  - [Editor de código Visual Studio Code](https://code.visualstudio.com/)
- Também aprendemos a usar o GitHub para hospedar nossos projetos e compartilhar nossos códigos com a comunidade.

- e o mais importante, aprendemos alguns comando git que vai ser importante para hoje. São eles:
  - `git init`: inicia um repositório git
  - `git add`: adiciona arquivos para serem versionados
  - `git commit`: salva as alterações no repositório
  - `git status`: mostra o status do repositório
  - `git push`: envia as alterações para o repositório remoto
  - `git pull`: pega as alterações do repositório remoto
  - `git clone`: clona um repositório remoto

agora com esses comandos em mente, podemos aprender alguns novos comandos e conceitos.

## Branches

Branches são linhas de desenvolvimento paralelas. Elas permitem que você desenvolva funcionalidades isoladas umas das outras. As branches são criadas a partir da branch `main`.

## Alguns novos comandos Git

### Criando uma nova branch

Para criar uma nova branch, basta executar o comando abaixo:

```bash
git branch -b nome_da_branch
```

#### Listando as branches

Para listar as branches, basta executar o comando abaixo:

```bash
git branch
```

#### Mudando de branch

Para mudar de branch, basta executar o comando abaixo:

```bash
git checkout nome_da_branch
```

#### Deletando uma branch

Para deletar uma branch, basta executar o comando abaixo:

```bash
git branch -d nome_da_branch
```

### Git Merge

O comando `git merge` é usado para unir duas ou mais branches. Ele é usado para unir uma branch com a branch atual.

#### Unindo duas branches

Para unir duas branches, basta executar o comando abaixo:

```bash
git checkout branch_destino
git merge branch_origem
```

## GIT Flow

O Git Flow é um modelo de branches que facilita o desenvolvimento de projetos. Ele é composto por 3 a 5 branches principais:

![git flow](https://www.alura.com.br/artigos/assets/git-flow-o-que-e-como-quando-utilizar/imagem3.png)

- `main`: branch principal do projeto. Ela contém a versão mais estável do projeto.
- `develop`: branch de desenvolvimento. Ela contém a versão mais recente do projeto.
- `feature`: branch de desenvolvimento de uma nova funcionalidade. Ela é criada a partir da branch `develop` e é unida com a branch `develop` quando a funcionalidade é finalizada.
- `release`: branch de preparação de uma nova versão. Ela é criada a partir da branch `develop` e é unida com a branch `main` quando a versão é finalizada.
- `hotfix`: branch de correção de bugs. Ela é criada a partir da branch `main` e é unida com a branch `main` e com a branch `develop` quando o bug é corrigido.

## Mão na massa

Vamos supor que você está trabalhando no codigo que fizemos na aula anterior, no caso esse abaixo:

```python
print("Olá mundo!")
```

A sua versão do código está em produção ou seja está na branch `main`. Agora você precisa fazer uma correção de um bug(vamos supor que o bug é o `!` e precisamos remover) que foi encontrado na versão que está em produção. Para isso, você precisa criar uma branch `hotfix`

```bash
  git checkout main # main é a branch principal
  git branch -b hotfix # criando a branch hotfix
```

Agora você precisa fazer as correções necessárias

```python
  print("Olá mundo")
```

Depois de fazer as correções, você precisa adicionar as alterações, fazer o commit e enviar as alterações para o repositório remoto.

```bash
  git add . # adicionando todas as alterações
  git commit -m "[FIX] Corrigindo bug" # commitando as alterações
  git push origin hotfix # enviando as alterações para o repositório remoto
```

Agora você precisa fazer o merge da branch `hotfix` com a branch `main` e com a branch `develop`.

```bash
  git checkout main # voltando para a branch main
  git merge hotfix # unindo a branch hotfix com a branch main
  git push origin main # enviando as alterações para o repositório remoto
  git checkout develop # voltando para a branch develop
  git merge hotfix # unindo a branch hotfix com a branch develop
  git push origin develop # enviando as alterações para o repositório remoto
```

Vamos supor agora que você precisa fazer uma nova funcionalidade no seu projeto, por exemplo, imprimir o `Olá mundo` em inglês também. Para isso, você precisa criar uma branch `feature`

```bash
  git checkout develop # voltando para a branch develop
  git branch -b feature # criando a branch feature
```

Agora você precisa fazer as alterações necessárias

```python
  print("Olá mundo")
  print("Hello world")
```

Depois de fazer as alterações, você precisa adicionar as alterações, fazer o commit e enviar as alterações para o repositório remoto.

```bash
  git add . # adicionando todas as alterações
  git commit -m "[FEATURE] Adicionando nova funcionalidade" # commitando as alterações
  git push origin feature # enviando as alterações para o repositório remoto
```

Agora novamente você precisa fazer o merge da branch `feature` com a branch `develop`.

```bash
  git checkout develop # voltando para a branch develop
  git merge feature # unindo a branch feature com a branch develop
  git push origin develop # enviando as alterações para o repositório remoto
```

e assim por diante...
