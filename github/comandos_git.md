# ⌨️ Comandos Git Ligados ao GitHub

Nesta seção, você aprenderá os principais comandos utilizados para integrar o Git ao GitHub, permitindo enviar projetos para a nuvem, colaborar em equipe e sincronizar repositórios remotos.

---

# ⚙️ 1. Configurando o Git e conectando ao GitHub

Antes de começar, configure seu nome e e-mail no Git:

```bash
git config --global user.name "Seu Nome"
git config --global user.email "seu@email.com"
```

Essas informações serão associadas aos seus commits.

---

## 📦 Criando e conectando um repositório ao GitHub

Depois de criar um repositório no GitHub, conecte-o ao seu projeto local:

```bash
git init
git add .
git commit -m "Primeiro commit"

git remote add origin https://github.com/usuario/nome-do-repo.git

git branch -M main

git push -u origin main
```

---

## 📌 Explicação dos comandos

| Comando | Função |
|----------|---------|
| `git init` | Inicializa um repositório Git |
| `git add .` | Adiciona arquivos ao staging |
| `git commit -m` | Cria um commit |
| `git remote add origin` | Conecta o projeto ao GitHub |
| `git branch -M main` | Define o branch principal |
| `git push -u origin main` | Envia o projeto para o GitHub |

---

# 📥 2. Clonando um repositório

Para baixar um projeto existente do GitHub para sua máquina:

```bash
git clone https://github.com/usuario/nome-do-repo.git
```

## 💡 O que acontece?

Esse comando:

- cria uma cópia local do projeto;
- baixa todo o histórico do repositório;
- conecta automaticamente o projeto ao repositório remoto.

---

# 🔀 3. Fluxo básico de Pull Request

O Pull Request é o principal mecanismo de colaboração no GitHub.

---

## 📌 Fluxo no terminal

```bash
git checkout -b nova-funcionalidade

# Fazer alterações no projeto

git add .
git commit -m "Adiciona sistema de login"

git push origin nova-funcionalidade
```

---

## 📌 Fluxo no GitHub

Depois do push:

1. Acesse o repositório no GitHub;
2. Clique em **"Compare & pull request"**;
3. Revise as alterações;
4. Crie o Pull Request;
5. Realize o merge após aprovação.

---

# 🔄 4. Sincronizando com o repositório remoto

Quando outras pessoas fizerem alterações no projeto, você pode atualizar sua cópia local utilizando:

```bash
git pull origin main
```

Ou, em outro branch:

```bash
git pull origin nome-do-branch
```

## 💡 O que o pull faz?

O comando `git pull`:

- baixa alterações do GitHub;
- atualiza o repositório local;
- sincroniza o histórico.

---

# 🍴 5. Trabalhando com Forks

Forks permitem contribuir para projetos de outras pessoas.

---

## 📌 Passo 1 — Fazer o fork

No GitHub, clique em **Fork** para criar uma cópia do projeto em sua conta.

---

## 📌 Passo 2 — Clonar seu fork

```bash
git clone https://github.com/SEUUSUARIO/projeto.git

cd projeto
```

---

## 📌 Passo 3 — Adicionar o repositório original

```bash
git remote add upstream https://github.com/usuario-original/projeto.git
```

O repositório original é chamado de `upstream`.

---

## 📌 Passo 4 — Atualizar sua cópia

```bash
git fetch upstream

git merge upstream/main

git push origin main
```

Isso mantém seu fork atualizado com o projeto original.

---

# 💻 6. GitHub CLI (opcional)

O **GitHub CLI** permite utilizar recursos do GitHub diretamente no terminal através do comando `gh`.

---

## 📌 Exemplos

```bash
gh auth login
```

```bash
gh repo create meu-projeto --public
```

```bash
gh pr create --title "Nova feature" --body "Descrição"
```

```bash
gh issue create --title "Bug report"
```

```bash
gh repo clone usuario/repositorio
```

---

## 💡 Vantagens do GitHub CLI

- maior produtividade;
- integração total com terminal;
- automação de tarefas;
- fluxo de trabalho mais rápido.

---

# 🛠️ 7. Outros comandos úteis

## 📌 Ver status do projeto

```bash
git status
```

---

## 📌 Ver histórico de commits

```bash
git log --oneline
```

---

## 📌 Ver diferenças entre arquivos

```bash
git diff
```

---

## 📌 Criar e trocar de branch

```bash
git checkout -b nova-func
```

```bash
git checkout main
```

---

## 📌 Mesclar branches

```bash
git checkout main

git merge nova-func

git push origin main
```

---

# ✅ Conclusão

Os comandos relacionados ao GitHub permitem transformar o versionamento local do Git em um fluxo colaborativo online.

Com eles, é possível:

- publicar projetos;
- sincronizar repositórios;
- colaborar em equipe;
- abrir Pull Requests;
- contribuir para projetos open source;
- automatizar tarefas e deploys.

Dominar esse fluxo é essencial para trabalhar profissionalmente com Git e GitHub 🚀
