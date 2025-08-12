# Window Functions — Syntax + Patterns

**Core syntax:**
```sql
<func>() OVER (
  PARTITION BY <keys>
  ORDER BY <sort>
  ROWS BETWEEN UNBOUNDED PRECEDING AND CURRENT ROW
)
```

**Patterns:**
- **Day-1 retention**: LEAD(date) = date + 1 on first event.
- **Top-N per group**: ROW_NUMBER() over partition, filter `= 1..N`.
- **Running totals**: SUM() with window frame.
