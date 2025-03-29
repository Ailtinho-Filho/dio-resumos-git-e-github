# Guia Completo de Uso do Git

Este guia aborda os conceitos básicos do Git e de como usar repositórios locais e remotos no GitHub de forma simples e prática.


## 1. Instalando o Git

### **Windows**
1. Acesse  e baixe o instalador em: (https://git-scm.com/downloads/win)
2. Execute o instalador e aceite as opções padrão.
3. Após a instalação, abra o Git Bash para usar o Git.

### **Linux (Debian/Ubuntu)**
1.baixe o instalador pelo Linux em: (https://git-scm.com/downloads/linux)
2. Abra o terminal e execute os seguintes comandos:

    
    sudo apt update
    sudo apt install git
    

### **MacOS**
1. Acesse e baixar o instalador em: (https://git-scm.com/downloads/mac)

## 2. Configurando o Git

Para configurar seu nome de usuário e e-mail globalmente, execute os seguintes comandos. Esses dados serão usados em todos os seus commits:

```
git config --global user.name "Seu Nome"
git config --global user.email "seuemail@example.com"
```


## 3. Criando um Novo Repositório

Para criar um repositório local, execute os seguintes comandos:

```
mkdir meu-projeto
cd meu-projeto
git init
```

Isso criará um novo repositório Git vazio na pasta `meu-projeto`.


## 4. Adicionando Arquivos ao Repositório ##

Crie um arquivo de exemplo e adicione ao repositório com os seguintes comandos:

```
echo "# Meu Projeto" > README.md
git add README.md
git commit -m "Primeiro commit"
```


## 🐱‍👤5. Conectando ao GitHub ##

### **Criando um Repositório no GitHub**
1. Acesse o [GitHub](https://github.com/) e faça login.
2. Crie um novo repositório clicando em **New Repository**.
3. Dê um nome ao repositório e clique em **Create Repository**.

### **Vinculando o Repositório Local ao Remoto**
Após criar o repositório no GitHub, conecte seu repositório local ao remoto com os seguintes comandos:

```
git remote add origin https://github.com/seu-usuario/meu-projeto.git
git branch -M main
git push -u origin main
```


## 6. Clonando um Repositório ##

Para clonar um repositório remoto para sua máquina local, execute:

```
git clone https://github.com/seu-usuario/meu-projeto.git
```


## 7. Fluxo Básico de Uso ##

1. Modifique os arquivos conforme necessário.
2. Adicione as mudanças ao Git:

    ```
    git add .
    ```

3. Crie um commit com uma mensagem descritiva:

    ```
    git commit -m "Descrição do que foi feito"
    ```

4. Envie as mudanças para o repositório remoto no GitHub:

    ```
    git push origin main
    ```


## 8. Verificando o Status ##

Para verificar o status do seu repositório e ver quais arquivos foram modificados, use o comando:

```
git status
```


## 9. Atualizando o Repositório Local ##

Para garantir que seu repositório local esteja atualizado com as últimas mudanças do repositório remoto, execute:

```
git pull origin main
```
##🔨Ferramentas ##
-
-Git<br>

-Github<br>

## Autor ##
Ailton Rodrigo
</br>
⌨️ com ⭐ por Ailton Filho
</br>

## Referências ##

[git docs](https://git-scm.com/docs)

[utilize de base o repo do  Armstrong Lohãns](https://gist.github.com/lohhans/f8da0b147550df3f96914d3797e9fb89)

[github dock](https://docs.github.com/pt/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)

[Guia do uso do Git](https://www.notion.so/Guia-do-uso-do-Git-1c5e97a9d597806e8a6dfe3ff25a3f38)
Esse Notion contém o mesmo conteúdo desse repo e com vídeos adicionais do tema

