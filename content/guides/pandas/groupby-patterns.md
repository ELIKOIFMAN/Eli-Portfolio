# GroupBy Patterns

- **Aggregate then post-process**: `df.groupby(keys).agg({...}).reset_index()`
- **Transform for ratios**: `df.groupby(keys)[col].transform('sum')`
- **Rank inside groups**: `df.sort_values([...]).groupby(keys).head(N)`
