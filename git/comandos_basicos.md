# ⌨️ Comandos básicos do Git

## 1. Configuração inicial

Antes de começar a usar o Git, configure seu nome e e‑mail (isso aparecerá em todos os commits):

git config --global user.name "Seu Nome"
git config --global user.email "seu@email.com"

Essa configuração basta fazer uma vez por máquina e vale para todos os repositórios.

## 2. Iniciar um repositório

Para transformar uma pasta em repositório Git:

git init
git add .
git commit -m "Primeiro commit"

- git init → cria o repositório local.
- git add . → adiciona todos os arquivos ao staging area.
- git commit -m "mensagem" → salva um snapshot com descrição.

## 3. Comandos mais usados no dia a dia

git status → mostra o estado dos arquivos.
git diff → mostra as diferenças antes de commitar.
git log --oneline → mostra o histórico de commits.
git show → mostra o que foi alterado no último commit.

Esses comandos ajudam a acompanhar o que está acontecendo no repositório antes de salvar ou enviar mudanças.

## 4. Trabalhar com branches (super importante!)

O Git permite criar branches para trabalhar em funcionalidades separadas:

git branch nova-funcionalidade → cria um novo branch.
git checkout nova-funcionalidade → muda para esse branch.
git checkout -b nova-funcionalidade → cria e muda de branch em um único comando.

Depois de terminar o trabalho nesse branch, você pode voltar ao branch principal e mesclar:

git checkout main
git merge nova-funcionalidade

## 5. Desfazer mudanças simples

git restore nome-do-arquivo → desfaz mudanças em um arquivo.
git restore . → desfaz todas as alterações no diretório atual.
git reset --soft HEAD~1 → desfaz o último commit mantendo as mudanças no staging area.

## 6. Resumo dos comandos básicos

- git config --global user.name → configura o nome do usuário.
- git config --global user.email → configura o e‑mail.
- git init → inicia um repositório Git.
- git add . → adiciona arquivos ao staging.
- git commit -m "mensagem" → salva um commit.
- git status → mostra o estado dos arquivos.
- git diff → mostra diferenças.
- git log --oneline → mostra o histórico compacto.
- git branch nome-branch → cria um branch.
- git checkout nome-branch → muda de branch.
- git checkout -b nome-branch → cria e muda de branch.
- git merge nome-branch → mescla branch.
- git restore arquivo → desfaz mudanças.
- git reset --soft HEAD~1 → desfaz o último commit.

Em resumo, esses comandos formam o "núcleo" do dia a dia com Git, permitindo iniciar repositórios, registrar mudanças, organizar o trabalho em branches e, quando necessário, desfazer alterações de forma segura.