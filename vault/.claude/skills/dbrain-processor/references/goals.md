# Goals Integration

## ALWAYS Do First

Before processing daily entries:

1. **Read current weekly focus:**
   Read goals/3-weekly.md → Extract ONE Big Thing

2. **Read yearly goals:**
   Read goals/1-yearly-2026.md → Know active goals by area

3. **Check monthly priorities:**
   Read goals/2-monthly.md → Top 3 priorities

---

## Goal Alignment

When creating a task, ALWAYS check alignment in this order:

1. **Does it connect to ONE Big Thing?**
   - Yes → add to task description: `→ Weekly focus`
   - No → continue checking

2. **Does it connect to a monthly priority?**
   - Yes → add: `→ Monthly: [Priority name]`
   - No → continue checking

3. **Does it connect to a yearly goal?**
   - Yes → add: `→ Goal: [Goal name]`
   - No → mark as **operational**

---

## Task Priority Boost

If a task aligns with goals, adjust priority:

| Alignment | Default | Boost to |
|-----------|---------|----------|
| ONE Big Thing | p3 | p2 |
| Monthly priority | p3 | p2–p3 |
| Yearly goal | p4 | p3 |
| No alignment | p4 | p4 |

**Rule:** If a task relates to *clients, деньги или доход* — it can never be below **p3**.

---

## Saving Thoughts

When saving entries to `thoughts/`:

1. **Check goal relevance:**
   - Scan `goals/1-yearly-2026.md` for matching areas
   - If matches → add link in frontmatter:
     ```yaml
     related:
       - "[[goals/1-yearly-2026#Career & Business]]"
     ```

2. **Tag with goal area:**
   #goal/career
   #goal/health
   #goal/personal-growth
   #goal/financial

---

## Goal Progress Tracking

Track goal activity automatically:
- Task created → goal = **active**
- Thought saved → goal = **active**
- No activity for **7+ days** → status = **stale**
- No activity for **14+ days** → status = **warning**

Primary focus is **Career & Business**. If Career goal is stale → surface warning immediately.

---

## Report Section

Add to daily / weekly report:

<b>📈 Прогресс по целям:</b>
• Доход $3k/мес с ИИ-сервиса: {progress}% {status_emoji}
• Доводить дела до конца: {progress}% {status_emoji}

<b>⚠️ Требует внимания:</b>
• {goal name} — без активности {days} дней

---

## Goal File Parsing

### 3-weekly.md — Find ONE Big Thing
Look for pattern:
```markdown
> **If I accomplish nothing else, I will:**
> [THE ONE THING]

### 1-yearly-2025.md — Find Active Goals

Look for tables:
```markdown
| Goal | Progress | Status |
|------|----------|--------|
| Goal name | X% | 🟡 |
```

### 2-monthly.md — Find Top 3

Look for section:
```markdown
## Top 3 Priorities

1. **[Priority 1]**
2. **[Priority 2]**
3. **[Priority 3]**
```

## Example Alignment

Entry: "Нужно подготовить презентацию для клиента X"

Check:
- ONE Big Thing: "Ship MVP" → Not related
- Monthly #1: "Client deliverables" → ✅ Related
- Yearly: "Client Revenue" → ✅ Related

Result:
```
Task: Подготовить презентацию для клиента X
Description: → Monthly: Client deliverables → Goal: Client Revenue
Priority: p2 (boosted from p3)
```
