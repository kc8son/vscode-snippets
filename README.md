# Code snippets 
This is just a set of code snippets for:  
- python
- PostgreSQL
- MS SQL
- Snowflake

Others to be added as needed.


| File | Snippets |
|---|---|
| `jpm-python.code-snippets` | `nupy` |
| `jpm-python-snowflake.code-snippets` | `nupysf` |
| `jpm-sql-postgres.code-snippets` | `nupg`, `nupgw1`, `nupgw2`, `nupgw3`, `nupgw4`, `nupgw5`, `nupggi` |
| `jpm-sql-mssql.code-snippets` | `nums`, `numsw1`, `numsw2`, `numsw3`, `numsw4`, `numsw5`, `numsgi` |
| `jpm-sql-snowflake.code-snippets` | `nusf`, `nusfcsv`, `nusfw1`, `nusfw2`, `nusfw3`, `nusfw4`, `nusfw5`, `nusfgi` |

### Window Function Snippets

| # | Topic | PostgreSQL | MS SQL | Snowflake |
|---|---|---|---|---|
| w1 | Ranking — ROW_NUMBER, RANK, DENSE_RANK, NTILE, Top-N per group | `nupgw1` | `numsw1` | `nusfw1` |
| w2 | Aggregate — running totals, moving averages, partition totals, rolling min/max | `nupgw2` | `numsw2` | `nusfw2` |
| w3 | Value/Offset — LAG, LEAD, FIRST_VALUE, LAST_VALUE, NTH_VALUE | `nupgw3` | `numsw3` | `nusfw3` |
| w4 | Distribution — PERCENT_RANK, CUME_DIST, PERCENTILE_CONT, PERCENTILE_DISC | `nupgw4` | `numsw4` | `nusfw4` |
| w5 | Deduplication — preview dupes, delete via subquery/CTE, backup pattern, verify | `nupgw5` | `numsw5` | `nusfw5` |

### Gap and Island Snippets

| Topic | PostgreSQL | MS SQL | Snowflake |
|---|---|---|---|
| Gap and Island — continuous date streaks (flagged → islands → island_ranges) + gaps query | `nupggi` | `numsgi` | `nusfgi` |


To do:
1. ~~nupgw1. Ranking Functions - Assign a rank or position to each row within a partition.~~
1. ~~nupgw2. Aggregate Functions - Standard aggregates applied over a window instead of collapsing rows.~~
1. ~~nupgw3. Value / Offset Functions - Access values from other rows relative to the current row.~~
1. ~~nupgw4. Distribution Functions - Calculate relative position or percentile of a row within its partition.~~
1. ~~numsw1. Ranking Functions - Assign a rank or position to each row within a partition.~~
1. ~~numsw2. Aggregate Functions - Standard aggregates applied over a window instead of collapsing rows.~~
1. ~~numsw3. Value / Offset Functions - Access values from other rows relative to the current row.~~
1. ~~numsw4. Distribution Functions - Calculate relative position or percentile of a row within its partition.~~
1. ~~nusfw1. Ranking Functions - Assign a rank or position to each row within a partition.~~
1. ~~nusfw2. Aggregate Functions - Standard aggregates applied over a window instead of collapsing rows.~~
1. ~~nusfw3. Value / Offset Functions - Access values from other rows relative to the current row.~~
1. ~~nusfw4. Distribution Functions - Calculate relative position or percentile of a row within its partition.~~

To install — drop all 5 files into your VS Code snippets folder:

Windows: %APPDATA%\Code\User\snippets\
Mac: ~/Library/Application Support/Code/User/snippets\
