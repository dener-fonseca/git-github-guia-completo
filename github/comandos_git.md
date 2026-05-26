# Comandos Git ligados ao GitHub

## 1. Configurar e conectar o local ao GitHub

Primeiro, configure seu nome e e‑mail (se ainda não fez):

git config --global user.name "Seu Nome"
git config --global user.email "seu@email.com"

Depois, crie um repositório no GitHub e conecte seu repositório local:

git init
git add .
git commit -m "primeiro commit"
git remote add origin https://github.com/usuario/nome-do-repo.git
git branch -M main
git push -u origin main

O comando remote add origin ... define o repositório remoto no GitHub.  
O comando git push -u origin main envia seu histórico para o GitHub.

## 2. Clonar um repositório do GitHub

Para baixar um projeto do GitHub:

git clone https://github.com/usuario/nome-do-repo.git

Isso cria uma pasta local já com o repositório conectado ao remoto.

## 3. Fluxo básico de Pull Request

No GitHub, você vai:

- criar um repositório,
- (opcionalmente) forkar outro repositório,
- abrir Pull Requests para contribuir.

No terminal, o fluxo é:

git checkout -b nova-funcionalidade
# fazer alterações
git add .
git commit -m "adiciona login"
git push origin nova-funcionalidade

Depois, no GitHub:

- acesse o repositório;
- clique em "Compare & pull request";
- revise e finalize o merge.

## 4. Sincronizar com o repositório remoto

Quando o repositório remoto mudar (outra pessoa fez push):

git pull origin main

Se estiver num branch diferente:

git pull origin nome-do-branch

O comando pull traz as alterações do GitHub para o seu repositório local.

## 5. Trabalhar com forks (contribuir em projetos de outros)

Para contribuir em um projeto de terceiro:

1) Faça fork no GitHub (cria sua cópia).  
2) Clone seu fork:

git clone https://github.com/SEUUSUARIO/projeto.git
cd projeto

3) Adicione o repositório original como upstream:

git remote add upstream https://github.com/usuario-original/projeto.git

4) Atualizar sua cópia antes de trabalhar:

git fetch upstream
git merge upstream/main
git push origin main

Depois, crie um branch, faça as alterações e abra um Pull Request no repositório original.

## 6. Comandos do GitHub CLI (opcional)

Se você instalar o GitHub CLI (gh), pode fazer muita coisa direto no terminal:

gh auth login
gh repo create meu-projeto --public
gh pr create --title "Nova feature" --body "Descricao"
gh issue create --title "Bug report"
gh repo clone usuario/repo

O GitHub CLI integra o GitHub direto ao seu fluxo de trabalho com Git.

## 7. Outros comandos úteis com GitHub

- Ver status:
  git status

  - Ver histórico:
    git log --oneline

    - Ver diferenças:
      git diff

      - Criar e trocar de branch:
        git checkout -b nova-func
          git checkout main

          - Mesclar branch:
            git checkout main
              git merge nova-func
                git push origin main

                Resumo: os comandos principais ligados ao GitHub são git clone, git remote add origin, git push, git pull, o fluxo de git checkout -b e git push para criar Pull Requests, e, opcionalmente, o uso do GitHub CLI (gh) para agilizar o trabalho.