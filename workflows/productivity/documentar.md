---
description: Atualizar documentação e dashboard semanal do AgroShort
---

# /documentar — Atualizar Documentação e Dashboard do AgroShort

Use este workflow para revisar e atualizar toda a documentação do projeto e o dashboard de apresentação semanal.

## Fontes de Dados
- **`DIARIO_DE_BORDO/{data}.md`** — registros automáticos de cada ação (rule global)
- **Código fonte** — verificar estado real dos arquivos no repo

## Passos

1. **Revisar `docs/CHANGELOG.md`**
   - Verificar se todas as entregas recentes estão registradas
   - Adicionar entradas que faltam no formato Keep a Changelog
   - Agrupar por sprint (Adicionado, Modificado, Corrigido)

2. **Atualizar `docs/features/feature-tracker.md`**
   - Revisar o status de cada tela/feature (⬜ 🎨 🔨 ✅ 🔌 🚀)
   - Atualizar a tabela de resumo com contagens corretas
   - Verificar se o sprint atribuído ainda está correto

3. **Atualizar `docs/api/database-schema.md`**
   - Conferir se todas as tabelas do Supabase estão documentadas
   - Verificar se colunas novas foram adicionadas
   - Atualizar RLS policies documentadas

4. **Atualizar `docs/api/edge-functions.md`**
   - Conferir se todas as Edge Functions estão documentadas
   - Atualizar request/response se mudou
   - Adicionar novas functions criadas

5. **Verificar `docs/deliverables/handoff-checklist.md`**
   - Marcar itens concluídos no checklist
   - Adicionar itens novos que surgiram

6. **Atualizar `docs/README.md`** (se necessário)
   - Refletir mudanças na estrutura do projeto
   - Atualizar links para novos documentos

7. **Atualizar `docs/dashboard-reuniao.html`** (dashboard semanal para o Adriano)
   - Este é o **ÚNICO** material visual de apresentação
   - Ler `DIARIO_DE_BORDO/` da semana para coletar entregas
   - Atualizar: data, badge de status, ring de progresso, KPIs, barras por área, timeline, entregas, ações do Adriano, footer
   - Progresso global = sprints concluídos / 8 (conservador, não inflar)
   - Score de auditoria = último relatório em `🔍 auditorias/`
   - Tom das ações do Adriano = **colaborativo** ("preparação para lançamento"), nunca "bloqueante"
   - Atualizar `const progress = XX` no JavaScript

8. **Verificar consistência entre todos os docs**
   - Score de auditoria idêntico em: dashboard, feature-tracker, handoff-checklist
   - Prazo = 8 semanas em todos os docs
   - Contagem de telas consistente

9. **Resumir** o que foi atualizado ao usuário
