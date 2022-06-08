
<h1 align="center"> Aprendendo
<img align="center" alt="leo-Git" height="60" width="60" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/git/git-plain-wordmark.svg" /> e <img align="center" alt="leo-Git" height="50" width="50" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/github/github-original-wordmark.svg" />
</h1>

<img align="center" alt="leo-animação" height="" width="100%" src="./images/gif.gif" />

<br>

    📌 Proposta

    A proposta deste guia é ajudar as pessoas que queiram aprender 
    a utilizar o git e o github como ferramenta de trabalho, organização 
    e aprendizado. Este guia pode ajudar você a conhecer a ferramenta 
    e até mesmo a tirar dúvidas caso já a utilize. 

---
## 🧭 Índice

- [Fundamentos e conceitos iniciais](#-Fundamentos-e-conceitos-iniciais)
- [Git e GitHub são a mesma coisa](#-Git-e-GitHub-são-a-mesma-coisa)
- [Instalação e configuração](#-Instalação-e-configuração)
- [Comandos iniciais](#-Comandos-iniciais)
- [O que são e como trabalhar com branchs](#-O-que-são-e-como-trabalhar-com-branchs)
- [git clone](#-git-clone)
- [git pull](#-git-pull)
- [Fork](#-fork)
- [pull requeste](#-pull-requeste)
- [git ignore](#-git-ignore)


---
## ⚙ Fundamentos e conceitos iniciais


- Vamos começar entendendo o problema

<p align="justify">
Lembremos da época de escola em que tinhamos que formar equipes e fazer um trabalho, cada um ficava responsável por uma parte, portanto você fazia sua parte e mandanva para "o colega", aquele mesmo, que ficava responsável por juntar tudo no final. Você termina sua parte e manda para ele, ele analisa a sua parte e lhe pede para alterar algo pois não está legal, você gera um novo arquivo com a alteração e manda, porém ele lhe retorna novamente pedindo outra alteração, você gera mais um arquivo e manda, desta vez "o colega" diz que a versão anterior estava melhor e pede para você manda-lá novamente, só que você não tem mais, pois apagou. 😟

Então temos um problema, a pasta do trabalho está cheia de arquivos "trabalho final", "Agora vai", "ultimo", "trabalho dos infernos" e alguma das versões que "o colega" pediu você não tem mais, e agora? 😰

- A solução é o git! 🤯

O git é uma ferramenta de versionamento de código gratuita e open source, com ela você pode organizar as versões do seu código sem ter que criar inúmeros arquivos para fazer alterações, ela permite que tenhamos controle de tudo aquilo que já escrevemos, apagamos e tudo que fizemos ou vamos fazer de alterações, de modo fantasioso podemos descrevê-la como uma máquina do tempo para códigos. 😁

Ainda sim podemos trabalhar com várias pessoas no mesmo projeto, sem que ocorram conflitos.

- Conceito de repositório

O git e o github trabalham com repositórios, diretórios, mas não precisa se assustar, no seu dia a dia você é acostumado a mexer com pastas, seja criando, movendo, apagando, o git chama essas pastas de repositórios.
</p>

---
## 📍 Git e GitHub são a mesma coisa
<h2 align="center"> <img align="center" alt="leo-git-github" height="250" width="" src="./images/image1.png" /> </h2>

<p align="justify">
Não! O git e o github são coisas diferentes, porém trabalham juntos.

- Afinal qual a diferença?

O git é uma ferramenta instalada localmente, ou seja, fica na sua máquina, tudo que você fizer ficará armazenado e somente você terá acesso, justamente por ser local.

Já github é uma plataforma onde podemos hospedar nossos códigos, lá temos acesso as versões criadas, alterações feitas e ainda funciona como uma rede social para programadores, muitos profissionais utilizam o github como portifólio para mostrarem seu projetos.

    💡 Em tempos mais antigos quando as empresas ofertavam vagas de emprego para
    desevolvedores, inseriam o git e o github como pré-requistos adicionais
    ou diferencial, atualmente as empresas já inserem git e github como
    requisito para a vaga.
</p>

## 🌐 Instalação e configuração

- Para instalar o git é muito simples, basta acessar o site oficial [clique aqui](https://git-scm.com/) e baixar a versão mais atual do git.
<h2 align="center"> <img align="center" alt="leo-animação" height="" width="" src="./images/image2.png" /> </h2>
A instalação é padrão, basicamente você só precisa ir clicando em next, next até chegar ao fim!

Neste link o git será baixado para o sistema operacional windows, porém você pode obter o git também para linux ou macOS
[Saiba mais](https://git-scm.com/book/pt-br/v2/Come%C3%A7ando-Instalando-o-Git)

- Crie sua conta no github [clique aqui](https://github.com/) 

<h2 align="center"> <img align="center" alt="leo-animação" height="" width="" src="./images/image4.png" /> </h2>

A criação da conta no github é muito simples, basta ir fornencendo as informações que lhe forem pedidas e lembre-se do email que inserir lá, utilizaremos este mesmo email em configurações do git.

- Git Bash

O git fornce um terminal exclusivo chamado de git bash, ele é um terminal normal que já é instalado junto com o git e podemos executar todos os comandos de um terminal normalmente, a diferença é que o bash é personalizado para mexermos com git, mas fique a vontade para utilizar o seu terminal preferido. Para abrirmos basta clicar com o botão direito na pasta escolhida e pronto ele abrirá dentro daquele repositório (pasta).

<h2 align="center"> <img align="center" alt="leo-animação" height="" width="" src="./images/image3.png" /> </h2>

Com o git bash aberto você pode inserir o comando:

```bash
$ git --version
```
Este coamndo mostra a versão do git instalada atualmente e se mostrar a versão significa que está tudo certo e podemos começar a trabalhar.

Agora vamos nos indentificar para o git com os comandos:

```bash
$ git config --global user.name "seu nome"
```
```bash
$ git config --global user.email "seu email"
```
Utilize o mesmo email que inseriu para criar sua conta no github.

Caso precise ou queira visulalizar os seus dados insira o comando:

```bash
$ git config --list
```
🎉 Agora sim estamos prontos para começar!

---
## 📝 Comandos iniciais
- git init
    ```bash
    $ git init
    ```
    
- git add
    ```bash
    $ git add
    ```

- git commit
    ```bash
    $ git commit -m "nome_do_commit"
    ```

- git remote add origin
    ```bash
    $ git remote add origin link_do_repositório
    ```

- git push -u origin
    ```bash
    $ git push -u origin nome_da_branch
    ```

---
## O que são e como trabalhar com branchs


---
## git clone


---
## git pull


---
## Fork


---
## pull requeste


---
## git ignore

