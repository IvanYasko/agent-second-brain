# Critical Processing Rules

See [ABOUT.md](ABOUT.md) for user context and preferences.

---

## Rule 1: Skip Processed Entries
If entry contains ````

Дубликаты запрещены — вместо этого обновлять существующую задачу.

---

## Rule 4: Consider Workload
**ПЕРЕД назначением даты задачи:**

1. Вызвать `find-tasks-by-date`
   - `startDate`: "today"
   - `daysCount`: 7
2. Подсчитать количество задач на день
3. Если в целевом дне **3+ задач**:
   - сдвинуть задачу на ближайший день с меньшей нагрузкой

**Исключение:**
Задачи, напрямую связанные с клиентом или оплатой, не откладывать, даже при перегрузе.

---

## Rule 5: Mark After Processing
После обработки **КАЖДОЙ** записи обязательно добавлять маркер.

**Общий формат:**
```markdown

## Rule 6: Apply Decision Filters

Before saving any thought or task, check:
- Это масштабируется?
- Это можно автоматизировать?
- Это усиливает экспертизу/бренд?
- Это приближает к продукту/SaaS?

If 2+ yes → boost priority.

## Rule 7: Avoid Anti-Patterns

NEVER create:
- Абстрактные задачи без Next Action ("Подумать о...")
- Хаотичные списки без приоритетов
- Повторы без синтеза
- Академическая теория без применения

See [ABOUT.md](ABOUT.md) → Anti-Patterns section.

---

## Checklist Before Completion

- [ ] All new entries processed
- [ ] No duplicates in Todoist
- [ ] All tasks have dates and concrete actions
- [ ] Decision filters applied
- [ ] Anti-patterns avoided
- [ ] MOC files updated
- [ ] Report generated
