# Campos_developers aula 04

Neste quarto dia de curso, aprendemos um pouco mais de gitflow, a sua vantagens e desvantagens, e o fluxo de trabalho.

## Resumo do dia anterior

Relembrando o que aprendemos na aula anterior:

- Aprendemos tipos de dados em Python
- Aprendemos o modo interativo do Python

## O que vamos aprender hoje

- [Gitflow](#gitflow)
  - [Vantagens do gitflow](#vantagens-do-gitflow)
  - [Desvantagens do gitflow](#desvantagens-do-gitflow)
  - [Fluxo de trabalho](#fluxo-de-trabalho)
  - [Branches](#branches)
- [Alterativa ao gitflow](#alterativa-ao-gitflow)

## Gitflow

Já vimos o conceito de git flow, que é um fluxo de trabalho para projetos que usam git branches.
mas vamos ver um pouco mais sobre o gitflow

### Vantagens do gitflow

- Facilita a colaboração entre desenvolvedores
- Facilita a manutenção de projetos
- Facilita a criação de releases

### Desvantagens do gitflow

- Complexo
- Pode ter muito conflito de merge
- Pode ser difícil de entender
- Pode ter codigo duplicado e inutilizado, pois pode ter muitas branches
- Pode ser difícil de fazer merge de hotfix, release e feature em develop, pois pode ter conflito

### Fluxo de trabalho

- Criar uma branch de feature
- Fazer commits na branch de feature
- Fazer merge da branch de feature na branch de develop
- Criar uma branch de release
- Fazer commits na branch de release
- Fazer merge da branch de release na branch de master
- Fazer merge da branch de release na branch de develop
- Criar uma branch de hotfix
- Fazer commits na branch de hotfix
- Fazer merge da branch de hotfix na branch de master
- Fazer merge da branch de hotfix na branch de develop

### Branches

- master: branch principal, onde fica o código que está em produção
- develop: branch principal, onde fica o código que está em desenvolvimento e que vai para produção
- feature: branch onde fica o código de uma nova funcionalidade que está sendo desenvolvida
- release: branch onde fica o código que está pronto para ser lançado(pode ter mais de uma release)
- hotfix: branch onde fica o código de correção de bugs

## Alterativa ao gitflow

**TODO :** ainda estou escrevendo sobre isso, preciso rever o conseito da aula 4, pois faltei e não consegui acompanhar o conteúdo

