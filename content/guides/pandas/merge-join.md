# Merge & Join

```python
pd.merge(a, b, on=['key1','key2'], how='left', validate='m:1')
```
- Validate cardinality to prevent row blow-ups.
- Align dtypes before merging to avoid silent mismatches.
