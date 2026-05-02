# 🧠 AI Workflows

> Coleção pessoal de workflows, agentes e ferramentas para desenvolvimento com IA.

Workflows projetados para funcionar como **slash commands** no [Antigravity](https://github.com/google-deepmind/antigravity), Claude Code, e outros agentes de IA.

---

## 📂 Estrutura

```
workflows/
├── git/                  → Versionamento, worktrees, branching
├── dev/                  → Metodologias de desenvolvimento
├── ai-agents/            → Orquestração e gestão de agentes IA
└── productivity/         → Organização, documentação, processos
```

---

## 🗂 Catálogo

### ⚡ Git & Versionamento

| Workflow | Descrição | Comando |
|---|---|---|
| [best-practice-worktree](workflows/git/best-practice-worktree.md) | Agente consultor + executor seguro de Git Worktree. Criar, validar, atualizar, integrar e finalizar branches com worktrees. | `/best-practice-worktree` |

### 🛠 Desenvolvimento

| Workflow | Descrição | Comando |
|---|---|---|
| [test-driven-development](workflows/dev/test-driven-development.md) | Enforce TDD rigoroso — Red-Green-Refactor sem exceções. | `/test-driven-development` |
| [bmad](workflows/dev/bmad.md) | Breakthrough Method for Agile AI-Driven Development. Pipeline completo de projeto. | `/bmad` |

### 🤖 AI Agents

| Workflow | Descrição | Comando |
|---|---|---|
| [importar-agentes](workflows/ai-agents/importar-agentes.md) | Catálogo inteligente de agentes — analisa seu projeto e recomenda os melhores agentes, skills e squads. | `/importar-agentes` |
| [opensquad](workflows/ai-agents/opensquad.md) | Sistema de squads de agentes IA — onboarding, menus, pipelines e memória. | `/opensquad` |

### 📋 Produtividade

| Workflow | Descrição | Comando |
|---|---|---|
| [feedbacks](workflows/productivity/feedbacks.md) | Transforma feedbacks desestruturados (WhatsApp, áudio, etc) em backlog organizado com tipo, prioridade e tags. | `/feedbacks` |
| [documentar](workflows/productivity/documentar.md) | Atualizar documentação e dashboard semanal de projetos. | `/documentar` |

---

## 🚀 Como usar

### No Antigravity

Os workflows são registrados como **global workflows** e ficam disponíveis como slash commands em qualquer projeto:

```
/best-practice-worktree
/feedbacks
/bmad
```

### Em outros agentes (Claude Code, Codex, Cursor)

Copie o conteúdo do `.md` desejado e use como **system prompt** ou **instrução inicial**.

---

## 📐 Anatomia de um Workflow

Cada workflow segue esta estrutura:

```markdown
---
description: Descrição curta para aparecer no menu de comandos
---

# Nome do Workflow

// turbo-all  ← (opcional) auto-run de comandos seguros

## Conteúdo e instruções do agente
```

| Elemento | Obrigatório | Descrição |
|---|---|---|
| `description` (frontmatter) | ✅ | Aparece no menu de slash commands |
| `// turbo-all` | ❌ | Permite auto-execução de comandos seguros |
| `// turbo` | ❌ | Auto-run apenas no passo específico |

---

## ➕ Como adicionar um novo workflow

1. Crie um arquivo `.md` na categoria correta dentro de `workflows/`
2. Adicione o frontmatter com `description`
3. Escreva as instruções do agente
4. Atualize este README com uma entrada na tabela
5. Para usar no Antigravity, copie também para `~/.gemini/antigravity/global_workflows/`

---

## 📄 Licença

Uso pessoal. Ferramentas criadas por [@joaovitorgarcia](https://github.com/joaovitorgarcia) / [BEYONDSTACKS](https://github.com/BEYONDSTACKS).
