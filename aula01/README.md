# Campos_developers aula 01

Neste primeiro dia de curso, apredemos a instalar as principais ferramentas que vamos usar durante o curso. São elas:

- [Versionador de código Git](https://git-scm.com/)
- [Liguagem Python](https://www.python.org/)
- [Editor de código Visual Studio Code](https://code.visualstudio.com/)

Também aprendemos a usar o GitHub para hospedar nossos projetos e compartilhar nossos códigos com a comunidade.
E aqui está um pequeno resumo e tutorial de como instalar e usar essas ferramentas.

Nesse resumo, vamos aprender:

- [Instalação do Git](#instalação-do-git)
- [Execução do Git](#execução-do-git)
- [Instalação do Python](#instalação-do-python)
- [Execução do Python](#execução-do-python)
- [Instalação do Visual Studio Code](#instalação-do-visual-studio-code)
- [Execução do Visual Studio Code](#execução-do-visual-studio-code)

**Obs:** Nessas aulas, vamos usar o Windows como sistema operacional, mas também estou dando suporte para quem usa Linux. Então, se você usa Linux, não se preocupe, você vai conseguir acompanhar o curso normalmente, infelizmente não vou conseguir dar suporte para quem usa MacOS, mas provavelmente você vai conseguir acompanhar o curso normalmente.

## Git

Git é um sistema de controle de versão distribuído, usado principalmente no desenvolvimento de software, mas pode ser usado para registrar o histórico de edições de qualquer tipo de arquivo. Foi criado por Linus Torvalds em 2005.

### Instalação do Git

Para instalar o Git no Windows, basta baixar o instalador no [site oficial do Git](https://git-scm.com/downloads) e executá-lo.

E no Linux, basta executar o comando abaixo: (lembre-se de executar o comando no terminal)

```bash
sudo apt update # ou no lugar de apt, use o gerenciador de pacotes que você usa
sudo apt install git # ou no lugar de apt, use o gerenciador de pacotes que você us

# geralmente o git já vem instalado no Linux, mas se não vier, instale usando o comando acima
```

Caso você tenha dúvidas sobre como instalar o Git no Windows ou no Linux, veja os tutoriais abaixo:

- [Como instalar o GIT no Windows](https://www.youtube.com/watch?v=gmyiJcn1WuQ&ab_channel=CamposDevelopers)
- No linux é só executar o comando acima no terminal, mas caso não esteja conseguindo, me mande uma mensagem no discord que eu te ajudo. (link do discord esta no meu README)

**Obs:** Para executar os comandos via linha de comando no Windows, usaremos o git bash que vem junto com o Git ou podemos usar o PowerShell, já no caso do Linux, usaremos o terminal padrão do sistema.

## Execução do Git

O git é um programa que usamos variadas vezes durante esse curso, então vamos ver se realmente ele foi instalado corretamente, para isso pode rodar o comando abaixo no terminal:

```bash
git --version
```

![git](https://linuxhint.com/wp-content/uploads/2022/09/image7.png)

Ele deve retornar a versão do git que você instalou, se não retornar, provavelmente você não instalou o git corretamente.

### Configuração do Git

Para configurar o Git no Linux e no Windows, basta executar os comandos abaixo: (lembre-se de substituir os valores entre aspas pelos seus dados)

```bash
git config --global user.name "Seu Nome" # use o mesmo nome do GitHub
git config --global user.email "seu@email.com" # use o mesmo e-mail do GitHub
```

## Python

O Python é uma linguagem de programação de alto nível, interpretada, de script, imperativa, orientada a objetos, funcional, de tipagem dinâmica e forte. Foi lançada por Guido van Rossum em 1991.

### Instalação do Python

Para instalar o Python no Windows, basta baixar o instalador no
[site oficial do Python](https://www.python.org/downloads/windows/) e executá-lo (não se esqueça de marcar a opção "Add Python 3.x to PATH").

Ou se preferir, o python está disponível no [Microsoft Store](https://www.microsoft.com/pt-br/p/python-39/9p7qfqmjrfp7?activetab=pivot:overviewtab).

Para instalar o Python no Linux, basta executar o comando abaixo:

```bash
sudo apt install python3 # ou no lugar de apt, use o gerenciador de pacotes que você usa

# geralmente o python já vem instalado no Linux, mas se não vier, instale usando o comando acima
```

Caso você tenha dúvidas sobre como instalar o Python no Windows, veja o tutorial abaixo:

- [Como instalar o Python no Windows](https://www.youtube.com/watch?v=QX4d2FkLs8M&ab_channel=CamposDevelopers)
- No linux é só executar o comando acima no terminal, mas caso não esteja conseguindo, me mande uma mensagem no discord que eu te ajudo. (link do discord esta no meu README)

### Execução do Python

Para executar o Python no Linux e no Windows, basta executar o comando abaixo:

```bash
python # ou python3
```

**Obs:** No linux o comando é `python3`, pois antigamente muitas distribuições usavam o python 2 e o python 3, então para evitar conflitos, o comando `python` sempre apontava para o python 2, mas agora o python 2 não é mais suportado, mas ainda assim o padrão é usar o `python3` e possivelmente você vai precisar usar o `python3` em vez do `python` em alguns casos, mas não se preocupe, eu vou avisar quando isso acontecer.

![python](https://tutorialsinhand.com/ReadWriteData/Articles/1081/CheckPython.PNG)

Caso não funcione, tente reniciar o computador e executar o comando novamente, se mesmo assim não funcionar, provavelmente você não instalou o Python corretamente.

## Visual Studio Code

O Visual Studio Code é um editor de código-fonte desenvolvido pela Microsoft para Windows, Linux e macOS. Ele inclui suporte para depuração, controle de versão Git incorporado, realce de sintaxe, complementação inteligente de código, snippets e refatoração de código.

### Instalação do Visual Studio Code

Para instalar o Visual Studio Code no Windows ou no Linux, basta baixar o instalador no
[site oficial do Visual Studio Code](https://code.visualstudio.com/) e executá-lo.

Ou se preferir, no Windows o Visual Studio Code está disponível no [Microsoft Store](https://apps.microsoft.com/store/detail/visual-studio-code/XP9KHM4BK9FZ7Q?hl=pt-br&gl=br&activetab=pivot%3Aoverviewtab), e no Linux, o Visual Studio Code está disponível no [Snap Store](https://snapcraft.io/code).

- [Como instalar o Visual Studio Code no Windows](https://www.youtube.com/watch?v=E5Bl3pxJeuI&ab_channel=CamposDevelopers)
- [Como instalar o Visual Studio Code no Linux](https://www.youtube.com/watch?v=Dun7Vkpet6k&ab_channel=rorampy)

### Execução do Visual Studio Code

Para executar o Visual Studio Code no Linux e no Windows, basta executar o comando abaixo:

```bash
code
```

Ou clique no ícone do Visual Studio Code no menu iniciar do Windows ou no menu de aplicativos do Linux.

Devemos ter uma tela parecida com essa:

![vscode](https://user-images.githubusercontent.com/35271042/49915383-3250ef00-fe4a-11e8-9092-02270e104616.png)

### Configuração do Visual Studio Code

Para configurar o Visual Studio Code no Linux e no Windows, basta instalar as extensões abaixo:

- [Python Support for Visual Studio Code](https://marketplace.visualstudio.com/items?itemName=ms-python.python)

Caso não saiba como instalar extensões no Visual Studio Code, veja o tutorial abaixo:

- [Como instalar extensões no Visual Studio Code](https://livreeaberto.com/instalando-extensoes-do-vs-code)

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

Caso você tenha duvida como criar uma conta no GitHub e como criar um repositório, veja os tutoriais abaixo:

- [Como criar uma conta no GitHub](https://docs.github.com/pt/get-started/signing-up-for-github/signing-up-for-a-new-github-account)
- [Como criar um repositório no GitHub](https://docs.github.com/pt/get-started/quickstart/create-a-repohttps://docs.github.com/pt/get-started/quickstart/create-a-repo)

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
