# Entry Classification

## Work Domains → Categories

Based on user's work context (see [ABOUT.md](ABOUT.md)):

### Client Work
Работа с клиентами ИИ-сервиса «Второй мозг»: запросы, настройка, сопровождение, оплата, дедлайны.
**Keywords:** блогер, предприниматель, клиент, запрос, настройка, сопровождение, оплата, дедлайн
**→ Category:** task (p1-p2) → Todoist

### AI & Tech
Разработка и улучшение ИИ-сервисов, технологии, автоматизация.
**Keywords:** GPT, Claude, модель, агент, API, пайплайн, автоматизация, интеграция, LLM, embeddings
**→ Category:** learning или project → thoughts/

### Product
Продуктовые идеи и развитие ИИ-сервиса «Второй мозг».
**Keywords:** продукт, SaaS, MVP, гипотеза, монетизация, юнит-экономика, сервис, второй мозг
**→ Category:** idea или project → thoughts/

### Company Ops
Операционные вопросы соло-фриланса и сервиса.
**Keywords:** процесс, автоматизация, финансы, доход, подписка, биллинг, ИИ-сервис «Второй мозг»
**→ Category:** task или project (depends on urgency)

### Content
Контент как вспомогательный инструмент (без основного фокуса).
**Keywords:** пост, контент, тезис, статья, заметка
**→ Category:** idea → thoughts/ideas/ или task если есть дедлайн

---

## Decision Tree
Entry text contains...
│
├─ Клиент / оплата / дедлайн? ────────────────> TASK (p1-p2)
│  (клиент, блогер, предприниматель, оплата)
│
├─ Срочно или операционно? ─────────────────> TASK (p2-p3)
│  (нужно сделать, не забыть, ответить)
│
├─ Изучение ИИ / технологий? ───────────────> LEARNING
│  (модель, агент, API, автоматизация)
│
├─ Идея продукта / сервиса? ─────────────────> IDEA или PROJECT
│  (MVP, SaaS, второй мозг)
│
├─ Стратегия / планирование? ───────────────> PROJECT
│  (план, система, масштабирование)
│
├─ Личное осознание? ───────────────────────> REFLECTION
│  (понял, заметил, состояние)
│
└─ Идея контента? ──────────────────────────> IDEA
   (пост, тезис)

---

## Apply Decision Filters

Перед сохранением спроси:
- Это приближает к платящему клиенту?
- Это снижает хаос и прокрастинацию?
- Это можно упростить или автоматизировать?
- Это усиливает ИИ-сервис «Второй мозг»?

Если **да на 2+ вопроса** → повысить приоритет.

---

## Photo Entries

For `[photo]` entries:
1. Проанализировать изображение
2. Определить домен:
   - Скриншот клиентского диалога → Client Work
   - Схема / архитектура → AI & Tech или Product
   - Текст / статья → Learning
3. Кратко описать суть в daily-записи

---

## Output Locations

| Category | Destination | Priority |
|----------|-------------|----------|
| task (client) | Todoist | p1-p2 |
| task (ops) | Todoist | p2-p3 |
| task (content) | Todoist | p3-p4 |
| idea | thoughts/ideas/ | — |
| reflection | thoughts/reflections/ | — |
| project | thoughts/projects/ | — |
| learning | thoughts/learnings/ | — |

---

## File Naming
thoughts/{category}/{YYYY-MM-DD}-short-title.md

Examples:
thoughts/ideas/2026-01-second-brain-onboarding.md
thoughts/projects/2026-01-ai-second-brain-mvp.md
thoughts/learnings/2026-01-claude-agents-setup.md

---

## Thought Structure

Use preferred format:
```markdown
---
date: {YYYY-MM-DD}
type: {category}
domain: {Client Work|AI & Tech|Product|Company Ops|Content}
tags: [goal/career, goal/product]
---

## Context
Что привело к мысли или задаче

## Insight
Ключевая идея или наблюдение

## Implication
Что это значит для ИИ-сервиса «Второй мозг» или дохода

## Next Action
Один конкретный следующий шаг

## Anti-Patterns (ИЗБЕГАТЬ)

При создании мыслей НЕ делать:
- Абстрактные рассуждения без Next Action
- Академическая теория без применения к вашему проекту/продукту
- Повторы без синтеза (кластеризуй похожие!)
- Хаотичные списки без приоритетов
- Задачи типа "подумать о..." (конкретизируй!)

---

## MOC Updates

After creating thought file, add link to:
```
MOC/MOC-{category}s.md
```

Group by domain when relevant:
```markdown
## AI & Tech
- [[2024-12-16-claude-mcp-setup]] - MCP integration

## Product
- [[2024-12-16-saas-pricing-model]] - Pricing research
```
