# Campos_developers aula 01

Neste primeiro dia de curso, apredemos a instalar e usar as principais ferramentas que vamos usar durante o curso. São elas:

- [Python](https://www.python.org/)
- [Git](https://git-scm.com/)
- [Visual Studio Code](https://code.visualstudio.com/)

Também aprendemos a usar o GitHub para hospedar nossos projetos e compartilhar nossos códigos com a comunidade.
E aqui está um pequeno resumo e tutorial de como instalar e usar essas ferramentas.

## Python

O Python é uma linguagem de programação de alto nível, interpretada, de script, imperativa, orientada a objetos, funcional, de tipagem dinâmica e forte. Foi lançada por Guido van Rossum em 1991.

### Instalação

Para instalar o Python no Ubuntu, basta executar o comando abaixo:

```bash
sudo apt install python3
```

Para instalar o Python no Windows, basta baixar o instalador no
[site oficial do Python](https://www.python.org/downloads/windows/) e executá-lo (não se esqueça de marcar a opção "Add Python 3.x to PATH").

caso você tenha dúvidas sobre como instalar o Python no Windows, veja o tutorial abaixo:

- [Como instalar o Python no Windows](https://www.youtube.com/watch?v=QX4d2FkLs8M&ab_channel=CamposDevelopers)

### Execução

Para executar o Python no Linux e no Windows, basta executar o comando abaixo:

```bash
python # ou python3
```

## Git

Git é um sistema de controle de versão distribuído, usado principalmente no desenvolvimento de software, mas pode ser usado para registrar o histórico de edições de qualquer tipo de arquivo. Foi criado por Linus Torvalds em 2005.

### Instalação

Para instalar o Git no Linux, basta executar o comando abaixo:

```bash
sudo apt install git
```

Para instalar o Git no Windows, basta baixar o instalador no [site oficial do Git](https://git-scm.com/downloads) e executá-lo.

caso você tenha dúvidas sobre como instalar o Git no Windows, veja o tutorial abaixo:

- [Como instalar o GIT no Windows](https://www.youtube.com/watch?v=gmyiJcn1WuQ&ab_channel=CamposDevelopers)

### Configuração

Para configurar o Git no Linux e no Windows, basta executar os comandos abaixo no terminal (Linux) ou no Git Bash (Windows):

```bash
git config --global user.name "Seu Nome" # use o mesmo nome do GitHub
git config --global user.email "seu@email.com" # use o mesmo e-mail do GitHub
```

## Visual Studio Code

O Visual Studio Code é um editor de código-fonte desenvolvido pela Microsoft para Windows, Linux e macOS. Ele inclui suporte para depuração, controle de versão Git incorporado, realce de sintaxe, complementação inteligente de código, snippets e refatoração de código.

### Instalação

Para instalar o Visual Studio Code no Linux, basta executar o comando abaixo:

```bash
sudo snap install --classic code
# ou baixe o instalador no site oficial do Visual Studio Code
```

Para instalar o Visual Studio Code no Windows, basta baixar o instalador no
[site oficial do Visual Studio Code](https://code.visualstudio.com/) e executá-lo.

caso você tenha dúvidas sobre como instalar o Visual Studio Code no Windows, veja o tutorial abaixo:

- [Como instalar o Visual Studio Code no Windows](https://www.youtube.com/watch?v=E5Bl3pxJeuI&ab_channel=CamposDevelopers)

### Configuração

Para configurar o Visual Studio Code no Linux e no Windows, basta instalar as extensões abaixo:

- [Python Support for Visual Studio Code](https://marketplace.visualstudio.com/items?itemName=ms-python.python)

## GitHub

GitHub é uma plataforma de hospedagem de código-fonte com controle de versão usando o Git. A plataforma permite que programadores, utilitários ou qualquer usuário cadastrado na plataforma contribuam em projetos privados e/ou Open Source de qualquer lugar do mundo.

### Criação de conta

Para criar uma conta no GitHub, basta acessar o site oficial do GitHub e clicar no botão "Sign up for GitHub". Você pode criar uma conta com seu e-mail ou com sua conta do Google.

### Criação de repositório

Para criar um repositório no GitHub, basta acessar o site oficial do GitHub e clicar no botão "New" no canto superior direito da tela. Em seguida, preencha os campos abaixo:

- Nome do repositório: `hello`
- Descrição: opcional
- Público ou privado: `Público`
- Inicializar o repositório com um README: `Sim`
- gitignore: template `Python`
- Licença: `nenhuma ou a que você preferir` (recomendo a estudar sobre licenças de software e escolher uma que se adeque ao seu projeto)

## Mão na massa

### Primeiro programa

Para testar se tudo foi instalado corretamente, vamos criar nosso primeiro programa em Python. Para isso, crie um arquivo chamado `hello.py` com o seguinte conteúdo:

```python
print("Hello World!") # imprime a mensagem "Hello World!" no terminal
```

E execute o programa com o comando abaixo:

```bash
python hello.py # ou python3 hello.py
```

Se tudo estiver correto, parabéns! você acabou de executar seu primeiro "Hello World!" em Python.

### Usando Git e GitHub

Para usar o Git e o GitHub, vamos criar um repositório local e um repositório remoto no GitHub. Para isso, crie um diretório chamado `aula01` e execute os comandos abaixo:

```bash
git init # cria um repositório local
git remote add origin http://github.com/SEU_USUARIO/aula01.git # adiciona a referência do repositório remoto
git pull origin main # sincroniza o repositório local com o repositório remoto
git add . # adiciona todos os arquivos do diretório atual para o repositório local
git commit -m "Primeiro commit" # cria um commit com a mensagem "Primeiro commit"
git push origin main # envia o repositório local para o repositório remoto
```

Se tudo estiver correto, o repositório local deve ser enviado para o repositório remoto no GitHub. Para verificar, acesse o repositório remoto no GitHub e verifique se o arquivo `hello.py` foi enviado. Se sim, parabéns! você acabou de enviar seu primeiro programa para o GitHub.
