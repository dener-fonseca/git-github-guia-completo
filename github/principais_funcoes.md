# 🚀 Principais Funções do GitHub

O GitHub oferece muito mais do que hospedagem de código.  
A plataforma reúne ferramentas completas para colaboração, gerenciamento de projetos, automação, documentação e integração entre equipes de desenvolvimento.

Nesta seção, você conhecerá os principais recursos que tornam o GitHub uma das plataformas mais importantes do mundo da tecnologia.

---

# 📦 1. Repositórios Remotos

O GitHub permite armazenar repositórios Git na nuvem, possibilitando acesso remoto ao projeto e colaboração entre desenvolvedores.

Os repositórios podem ser:

| Tipo | Descrição |
|------|------------|
| **Público** | Qualquer pessoa pode visualizar e clonar |
| **Privado** | Apenas usuários autorizados têm acesso |

## 💡 Vantagens

- Backup seguro do projeto
- Compartilhamento de código
- Trabalho colaborativo
- Controle de versões online
- Contribuições via forks e Pull Requests

---

# 🔀 2. Pull Requests

O **Pull Request (PR)** é o principal mecanismo de colaboração do GitHub.

Ele permite propor alterações no projeto antes de integrar as mudanças ao branch principal.

## 📌 Fluxo básico

1. Criar um branch
2. Desenvolver a funcionalidade
3. Enviar o branch para o GitHub
4. Abrir um Pull Request
5. Revisar o código
6. Realizar o merge

## 💡 Benefícios

- Revisão de código
- Discussões sobre alterações
- Maior qualidade do software
- Controle sobre mudanças importantes

---

# 🐞 3. Issues

As **Issues** funcionam como um sistema de gerenciamento de tarefas e problemas.

Elas podem ser utilizadas para:

- reportar bugs;
- sugerir funcionalidades;
- organizar tarefas;
- discutir melhorias;
- registrar problemas do projeto.

## 📌 Recursos das Issues

- Título e descrição
- Labels
- Assignees
- Comentários
- Vinculação com Pull Requests

---

# 📋 4. GitHub Projects

O **GitHub Projects** permite criar quadros organizacionais semelhantes ao método Kanban.

Exemplo:

```text
To Do → In Progress → Done
```

## 💡 Recursos

- Organização de tarefas
- Integração com Issues e PRs
- Automação de fluxo
- Gerenciamento de equipes

Muito utilizado em projetos profissionais e metodologias ágeis.

---

# 🌐 5. GitHub Pages

O **GitHub Pages** permite hospedar sites estáticos gratuitamente diretamente de um repositório.

Você pode publicar:

- portfólios;
- documentações;
- páginas de cursos;
- projetos pessoais;
- landing pages.

## 📌 Exemplo de endereço

```text
https://usuario.github.io
```

## 📌 Tecnologias suportadas

- HTML
- CSS
- JavaScript
- Markdown

---

# ⚙️ 6. GitHub Actions

O **GitHub Actions** é o sistema de automação do GitHub.

Ele permite automatizar processos como:

- testes automáticos;
- deploy;
- integração contínua (CI);
- entrega contínua (CD);
- validações de código.

## 📌 Exemplo de workflow

```yaml
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
```

Sempre que um `git push` acontece, o GitHub pode executar tarefas automaticamente.

---

# 📚 7. GitHub Wiki

Cada repositório pode possuir uma **Wiki** integrada para documentação.

Ela é utilizada para:

- tutoriais;
- manuais;
- documentação técnica;
- exemplos de uso;
- boas práticas internas.

A Wiki utiliza Markdown e facilita a organização do conhecimento do projeto.

---

# 🔒 8. Branch Protection Rules

O GitHub permite proteger branches importantes, como `main` ou `master`.

## 📌 Regras comuns

- exigir aprovação de Pull Request;
- impedir push direto;
- exigir testes automatizados;
- bloquear merges com falhas.

## 💡 Objetivo

Garantir maior segurança e estabilidade no projeto.

---

# 💬 9. GitHub Discussions

O **GitHub Discussions** funciona como um fórum integrado ao repositório.

Ele é ideal para:

- perguntas da comunidade;
- sugestões;
- troca de ideias;
- feedback;
- discussões gerais sobre o projeto.

Diferente das Issues, Discussions são voltadas para conversas e não necessariamente para tarefas técnicas.

---

# 💻 10. GitHub CLI

O **GitHub CLI** permite utilizar recursos do GitHub diretamente pelo terminal através do comando `gh`.

## 📌 Exemplos

```bash
gh repo create meu-projeto --public
```

```bash
gh pr create --title "Nova feature"
```

```bash
gh issue create --title "Bug report"
```

## 💡 Vantagens

- Fluxo mais rápido
- Integração total com terminal
- Automação de tarefas
- Produtividade para desenvolvedores

---

# ✅ Conclusão

O GitHub evoluiu de uma simples plataforma de hospedagem Git para um ecossistema completo de desenvolvimento de software.

Com recursos como:

- repositórios remotos;
- Pull Requests;
- Issues;
- GitHub Actions;
- Projects;
- GitHub Pages;
- documentação integrada;
- automação e colaboração;

o GitHub se tornou uma das ferramentas mais importantes para desenvolvedores e empresas em todo o mundo 🚀
