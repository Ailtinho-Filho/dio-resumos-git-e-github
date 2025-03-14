# dio-resumos-git-e-github
# Aula 01
## Guia Básico do Git para Repositórios

## 1. Instalando o Git
![image](https://github.com/user-attachments/assets/4fb7feca-fd5b-4a8f-9c66-c3ad9e079efa)### **Windows**
1. Baixe o instalador em: [git-scm.com](https://git-scm.com/)
2. Instale com as opções padrões.
3. Abra o **Git Bash**.


![image](https://github.com/user-attachments/assets/7e908e9b-74cb-480f-a1bc-2769e11931f2)### **Linux (Debian/Ubuntu)**
```sh
sudo apt update
sudo apt install git
```

### **MacOS**
```sh
brew install git
```

## 2. Configurando o Git

```sh
git config --global user.name "Seu Nome"
git config --global user.email "seuemail@example.com"
```

## 3. Criando um Novo Repositório

```sh
mkdir meu-projeto
cd meu-projeto
git init
```

**Imagem 1**: Criando um repositório localmente.
(Imagine um terminal com os comandos acima sendo digitados.)

## 4. Adicionando Arquivos ao Repositório

```sh
echo "# Meu Projeto" > README.md
git add README.md
git commit -m "Primeiro commit"
```

**Imagem 2**: Adicionando um arquivo ao Git.
(Imagine o comando `git status` mostrando que `README.md` foi adicionado.)

## 5. Conectando ao GitHub

### **Criar um repositório no GitHub**
1. Acesse [GitHub](https://github.com/) e faça login.
2. Clique em **New Repository**.
3. Dê um nome e clique em **Create Repository**.

**Imagem 3**: Tela de criação de repositório no GitHub.

### **Vincular o repositório local ao remoto**
```sh
git remote add origin https://github.com/seu-usuario/meu-projeto.git
git branch -M main
git push -u origin main
```

**Imagem 4**: Terminal mostrando o push para o repositório remoto.

## 6. Clonando um Repositório

```sh
git clone https://github.com/seu-usuario/meu-projeto.git
```

**Imagem 5**: Clonando um repositório para sua máquina.

## 7. Fluxo Básico de Uso

1. **Modificar arquivos**
2. **Adicionar ao Git**: `git add .`
3. **Criar commit**: `git commit -m "Mensagem do commit"`
4. **Enviar para o GitHub**: `git push origin main`

**Imagem 6**: Exemplo de workflow no Git.

## 8. Verificando o Status

```sh
git status
```

**Imagem 7**: Terminal mostrando `git status` com arquivos modificados.

## 9. Atualizando o Repositório Local

```sh
git pull origin main
```

**Imagem 8**: Atualizando o código local com o remoto.

---

Com esses passos, você pode gerenciar repositórios no Git e no GitHub com facilidade! 🚀

