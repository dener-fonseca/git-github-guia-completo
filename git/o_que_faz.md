# 🔧 O que o Git faz?

O Git é um **sistema de controle de versão distribuído** que registra mudanças em arquivos ao longo do tempo, criando um histórico completo do seu projeto. [web:17]  
Com isso, você consegue:

- ver o que mudou, quando e por quem;
- voltar a versões anteriores (reverter);
- experimentar novas funcionalidades sem “estragar” o trabalho principal (usando branches).

## 🎨 Como funciona (simplificado)

O fluxo básico do Git pode ser entendido assim:

Arquivos do Projeto → Git → Repositório Local → (opcional) GitHub / outro remoto

Resumindo:

- você trabalha nos arquivos normalmente;
- o Git rastreia essas mudanças;
- você salva trechos do projeto em **commits**;
- esses commits ficam no **repositório local**;
- se quiser, você envia para um repositório remoto (por exemplo, GitHub).

## Principais funções

| Função              | O que faz |
|---------------------|-----------|
| **Rastrear mudanças** | Salva o histórico completo das alterações em cada arquivo. |
| **Criar branches**    | Permite trabalhar em funcionalidades distintas em paralelo. |
| **Fazer merge**       | Combina as mudanças de um branch no outro (por exemplo, em `main`). |
| **Reverter mudanças** | Volta a versões anteriores de commits ou arquivos. |

## 🖼️ Visualização do fluxo

Podemos imaginar o histórico do Git como uma sequência de snapshots:

📁 Projeto
├── v1.0 (commit 1)
├── v1.1 (commit 2) ← HEAD (versão atual)
└── v1.2 (commit 3)

Cada commit representa um ponto no tempo em que você salvou o estado do projeto.

**Exemplo prático**: você edita um arquivo 5 vezes e, em cada momento, faz um commit → o Git guarda 5 versões distintas que você pode revisitar se precisar.

Dessa forma, o Git transforma o erro em recurso: você pode testar, estragar e voltar sempre para uma versão segura.