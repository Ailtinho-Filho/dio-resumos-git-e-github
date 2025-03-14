
# Guia Completo de Uso do Git

Este guia aborda os conceitos básicos do Git e como usar repositórios locais e remotos no GitHub de forma simples e prática.

---

## 1. Instalando o Git

### **Windows**
1. Acesse [git-scm.com](https://git-scm.com/) e baixe o instalador.
2. Execute o instalador e aceite as opções padrão.
3. Após a instalação, abra o Git Bash para usar o Git.

### **Linux (Debian/Ubuntu)**
1. Abra o terminal e execute os seguintes comandos:

    ```sh
    sudo apt update
    sudo apt install git
    ```

### **MacOS**
1. Se você usa o **Homebrew**, execute:

    ```sh
    brew install git
    ```

---

## 2. Configurando o Git

Para configurar seu nome de usuário e e-mail globalmente, execute os seguintes comandos. Esses dados serão usados em todos os seus commits:

```sh
git config --global user.name "Seu Nome"
git config --global user.email "seuemail@example.com"
```

---

## 3. Criando um Novo Repositório

Para criar um repositório local, execute os seguintes comandos:

```sh
mkdir meu-projeto
cd meu-projeto
git init
```

Isso criará um novo repositório Git vazio na pasta `meu-projeto`.

---

## 4. Adicionando Arquivos ao Repositório

Crie um arquivo de exemplo e adicione ao repositório com os seguintes comandos:

```sh
echo "# Meu Projeto" > README.md
git add README.md
git commit -m "Primeiro commit"
```

---

## 5. Conectando ao GitHub

### **Criando um Repositório no GitHub**
1. Acesse o [GitHub](https://github.com/) e faça login.
2. Crie um novo repositório clicando em **New Repository**.
3. Dê um nome ao repositório e clique em **Create Repository**.

### **Vinculando o Repositório Local ao Remoto**
Após criar o repositório no GitHub, conecte seu repositório local ao remoto com os seguintes comandos:

```sh
git remote add origin https://github.com/seu-usuario/meu-projeto.git
git branch -M main
git push -u origin main
```

---

## 6. Clonando um Repositório

Para clonar um repositório remoto para sua máquina local, execute:

```sh
git clone https://github.com/seu-usuario/meu-projeto.git
```

---

## 7. Fluxo Básico de Uso

1. Modifique os arquivos conforme necessário.
2. Adicione as mudanças ao Git:

    ```sh
    git add .
    ```

3. Crie um commit com uma mensagem descritiva:

    ```sh
    git commit -m "Descrição do que foi feito"
    ```

4. Envie as mudanças para o repositório remoto no GitHub:

    ```sh
    git push origin main
    ```

---

## 8. Verificando o Status

Para verificar o status do seu repositório e ver quais arquivos foram modificados, use o comando:

```sh
git status
```

---

## 9. Atualizando o Repositório Local

Para garantir que seu repositório local esteja atualizado com as últimas mudanças do repositório remoto, execute:

```sh
git pull origin main
```
