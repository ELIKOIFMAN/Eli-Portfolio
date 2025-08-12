# Joins — Logic

**Use-case recognition:**
- Need all from left + matches from right → LEFT JOIN
- Only matches on both sides → INNER JOIN
- Need all unique keys from both → FULL OUTER JOIN

**Pitfalls:**
- Multiplication of rows due to non-unique join keys → deduplicate or aggregate first.
- Filters on the right table with LEFT JOIN require `ON` vs `WHERE` awareness.

**Pattern drill:**
- Pre-aggregate on the many-side, then join.
- Use `EXISTS` for semi-joins when you only need presence/absence.
