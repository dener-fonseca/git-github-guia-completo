# ⌨️ Comandos Básicos do Git

Os comandos do Git permitem criar repositórios, registrar alterações, acompanhar versões e organizar o desenvolvimento de projetos de forma segura e eficiente.

Nesta seção, você conhecerá os principais comandos utilizados no dia a dia de qualquer desenvolvedor.

---

# ⚙️ 1. Configuração inicial

Antes de começar a utilizar o Git, é recomendado configurar seu nome e e-mail. Essas informações serão associadas aos commits realizados no projeto.

```bash
git config --global user.name "Seu Nome"
git config --global user.email "seu@email.com"
```

## 📌 Explicação

| Comando | Função |
|----------|---------|
| `git config --global user.name` | Define o nome do usuário |
| `git config --global user.email` | Define o e-mail do usuário |

> Essa configuração normalmente é feita apenas uma vez por computador.

---

# 📁 2. Criando um repositório Git

Para transformar uma pasta comum em um repositório Git, utilize os comandos abaixo:

```bash
git init
git add .
git commit -m "Primeiro commit"
```

## 📌 Explicação dos comandos

| Comando | Função |
|----------|---------|
| `git init` | Inicializa um repositório Git |
| `git add .` | Adiciona os arquivos para o staging area |
| `git commit -m "mensagem"` | Salva um snapshot do projeto |

---

# 🔍 3. Comandos mais usados no dia a dia

Esses comandos ajudam a acompanhar o estado do projeto durante o desenvolvimento.

```bash
git status
git diff
git log --oneline
git show
```

## 📌 Explicação dos comandos

| Comando | Função |
|----------|---------|
| `git status` | Mostra o estado atual dos arquivos |
| `git diff` | Exibe diferenças entre alterações |
| `git log --oneline` | Mostra o histórico resumido de commits |
| `git show` | Exibe detalhes do último commit |

---

# 🌿 4. Trabalhando com branches

As branches permitem desenvolver funcionalidades separadamente sem alterar diretamente a versão principal do projeto.

## 📌 Criando e trocando de branch

```bash
git branch nova-funcionalidade
git checkout nova-funcionalidade
```

Ou utilizando um único comando:

```bash
git checkout -b nova-funcionalidade
```

## 📌 Mesclando branches

Depois de concluir o trabalho no branch secundário, você pode unir as alterações ao branch principal:

```bash
git checkout main
git merge nova-funcionalidade
```

---

# ↩️ 5. Desfazendo alterações

O Git também oferece comandos para desfazer mudanças de maneira segura.

```bash
git restore nome-do-arquivo
git restore .
git reset --soft HEAD~1
```

## 📌 Explicação dos comandos

| Comando | Função |
|----------|---------|
| `git restore nome-do-arquivo` | Desfaz alterações em um arquivo |
| `git restore .` | Desfaz alterações no diretório atual |
| `git reset --soft HEAD~1` | Remove o último commit mantendo os arquivos |

---

# 📚 6. Resumo dos principais comandos

| Comando | Descrição |
|----------|------------|
| `git config --global user.name` | Configura o nome do usuário |
| `git config --global user.email` | Configura o e-mail do usuário |
| `git init` | Inicializa um repositório |
| `git add .` | Adiciona arquivos ao staging |
| `git commit -m "mensagem"` | Cria um commit |
| `git status` | Mostra o estado do projeto |
| `git diff` | Exibe diferenças entre arquivos |
| `git log --oneline` | Mostra histórico resumido |
| `git branch nome-branch` | Cria um branch |
| `git checkout nome-branch` | Troca de branch |
| `git checkout -b nome-branch` | Cria e troca de branch |
| `git merge nome-branch` | Mescla branches |
| `git restore arquivo` | Desfaz alterações |
| `git reset --soft HEAD~1` | Desfaz o último commit |

---

# ✅ Conclusão

Esses comandos formam a base do uso diário do Git.

Com eles, é possível:

- iniciar repositórios;
- acompanhar alterações;
- salvar versões do projeto;
- trabalhar com branches;
- organizar o desenvolvimento;
- recuperar versões anteriores de forma segura.

Dominar esses comandos é o primeiro passo para utilizar o Git de maneira profissional 🚀
