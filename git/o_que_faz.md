# 🔧 O que o Git faz?

O **Git** é um sistema de controle de versão distribuído que permite registrar, organizar e acompanhar alterações em arquivos ao longo do desenvolvimento de um projeto.

Com ele, é possível manter um histórico completo das modificações realizadas no código, facilitando o trabalho individual e colaborativo.

---

## 💡 O que o Git permite fazer?

Com o Git, você consegue:

- visualizar o que foi alterado no projeto;
- identificar quando e por quem as mudanças foram feitas;
- retornar para versões anteriores do código;
- testar novas funcionalidades sem comprometer a versão principal;
- trabalhar em equipe de forma organizada e segura.

---

## ⚙️ Como o Git funciona?

O funcionamento do Git pode ser resumido em um fluxo simples:

```text
Arquivos do Projeto
        ↓
       Git
        ↓
Repositório Local
        ↓
(opcional)
GitHub / Repositório Remoto
```

---

## 🧠 Fluxo básico de uso

No dia a dia, o processo normalmente acontece assim:

1. Você cria ou altera arquivos do projeto;
2. O Git identifica essas modificações;
3. As alterações são salvas em commits;
4. Os commits ficam armazenados no repositório local;
5. Se desejar, o projeto pode ser enviado para plataformas remotas como o GitHub.

---

## 📦 O que é um commit?

Um **commit** representa um ponto salvo do projeto.

Ele funciona como uma “foto” do estado dos arquivos em determinado momento, permitindo recuperar versões anteriores sempre que necessário.

Exemplo:

```bash
git commit -m "Adiciona tela de login"
```

---

## 🚀 Principais funções do Git

| Função | Descrição |
|--------|------------|
| **Rastrear mudanças** | Registra todo o histórico de alterações dos arquivos |
| **Criar branches** | Permite desenvolver funcionalidades separadamente |
| **Fazer merge** | Combina alterações de diferentes branches |
| **Reverter versões** | Recupera versões anteriores do projeto |
| **Trabalho colaborativo** | Facilita o desenvolvimento em equipe |

---

## 🌿 Trabalhando com branches

As **branches** permitem criar linhas paralelas de desenvolvimento.

Isso significa que você pode testar funcionalidades novas sem alterar diretamente a versão principal do projeto.

Exemplo:

```bash
git branch nova-funcionalidade
```

---

## 🖼️ Visualização do histórico

O histórico do Git pode ser imaginado como uma sequência de versões salvas:

```text
📁 Projeto
├── v1.0 → Commit 1
├── v1.1 → Commit 2
└── v1.2 → Commit 3 ← Versão atual
```

Cada commit representa um momento específico do desenvolvimento.

---

## 💻 Exemplo prático

Imagine que você edita um arquivo várias vezes durante o desenvolvimento.

Sempre que realiza um commit, o Git salva uma nova versão do projeto.

Assim, mesmo que algo dê errado, você pode voltar facilmente para uma versão anterior e segura.

---

## ✅ Conclusão

O Git revolucionou o desenvolvimento de software porque tornou o versionamento mais rápido, seguro e organizado.

Hoje, ele é uma das ferramentas mais importantes para qualquer desenvolvedor, sendo utilizado em projetos pessoais, acadêmicos e profissionais no mundo inteiro.
