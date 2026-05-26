# Principais funções do GitHub

## 1. Repositórios remotos
O GitHub hospeda repositórios Git na nuvem, transformando o controle de versão local em uma colaboração online.  
Cada repositório pode ser público ou privado:
- Público: qualquer pessoa pode ver e clonar.
- Privado: apenas você e os membros autorizados veem o código.

Com isso, você pode guardar backups seguros do seu trabalho, compartilhar projetos e permitir que outras pessoas contribuam via forks e pull requests.

## 2. Pull Requests
O Pull Request (PR) é a forma principal de propor mudanças no GitHub.  
Funciona assim:
- você cria um branch com uma nova funcionalidade ou correção;
- envia esse branch para o GitHub;
- abre um Pull Request para juntar as mudanças no branch principal (normalmente main ou master).

Antes do merge, outras pessoas podem revisar o código, comentar trechos específicos e pedir alterações. Isso melhora a qualidade do código e facilita a colaboração.

## 3. Issues (relatórios e tarefas)
O GitHub usa Issues para:
- reportar bugs;
- sugerir novas funcionalidades;
- organizar tarefas de desenvolvimento.

Cada issue pode ter título, descrição, labels, assignees e estar ligada a um Pull Request. Issues funcionam como um quadro de tarefas integrado ao código.

## 4. GitHub Projects (Kanban)
O GitHub Projects permite criar quadros Kanban (To Do, In Progress, Done) ligados a issues e Pull Requests.  
Você pode mover cartões entre colunas, automatizar transições e organizar grandes projetos com várias equipes.

## 5. GitHub Pages
O GitHub Pages permite hospedar sites estáticos gratuitamente a partir de um repositório.  
Você cria o repositório, coloca HTML, CSS e JavaScript na pasta docs ou na branch gh-pages, e o GitHub gera um site acessível em https://usuario.github.io.

GitHub Pages é muito usado para portfólios, documentação de projetos e páginas de apoio a cursos.

## 6. GitHub Actions (automação)
O GitHub Actions automatiza tarefas de integração contínua e deploy (CI/CD).  
Exemplo em .github/workflows/test.yml:

name: Test
on: [push]
jobs:
  test:
      runs-on: ubuntu-latest
          steps:
                - uses: actions/checkout@v2
                      - name: Install dependencies
                              run: npm install
                                    - name: Run tests
                                            run: npm test

                                            Sempre que alguém faz git push, o GitHub roda o fluxo de teste, mostra se passou ou falhou e ajuda a garantir que o código em main está estável.

                                            ## 7. GitHub Wiki (documentação)
                                            Cada repositório pode ter uma Wiki própria, com páginas Markdown separadas da pasta principal.  
                                            A Wiki serve para explicar como usar o projeto, documentar configurações, exemplos e tutoriais, e registrar boas práticas internas.

                                            ## 8. Branch protection rules
                                            O GitHub permite proteger branches importantes (como main) com regras, por exemplo:
                                            - exigir aprovação de Pull Request;
                                            - exigir que testes passem;
                                            - impedir push direto ao branch principal.

                                            Isso aumenta a segurança e a qualidade do código em produção.

                                            ## 9. GitHub Discussions
                                            O GitHub Discussions permite ter fóruns de discussão dentro do repositório, separados de Issues.  
                                            É útil para perguntas, ideias de novas funcionalidades e feedback geral sobre o projeto.

                                            ## 10. GitHub CLI (linha de comando)
                                            O GitHub CLI (comando gh) permite fazer várias ações diretamente do terminal:
                                            - gh repo create meu-projeto --public
                                            - gh pr create --title "Nova feature" --body "Descrição"
                                            - gh issue create --title "Bug report"

                                            Com isso, você integra o fluxo do GitHub direto ao seu terminal.

                                            Resumo: as principais funções do GitHub são: repositórios remotos, Pull Requests, Issues, Projects (Kanban), Pages (hospedagem de sites), Actions (automação), Wiki (documentação), branch protection rules, Discussions (fóruns) e GitHub CLI (comandos no terminal). Tudo isso torna o GitHub uma plataforma completa para colaborar em projetos de software.