# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What This Repo Is

A collection of VS Code snippet files (`.code-snippets`) for SQL and Python. These files live directly in the VS Code user snippets folder (`%APPDATA%\Code\User\snippets\` on Windows) and are active immediately — no build or install step needed.

## Snippet Files and Their Prefixes

| File | Prefix(es) | Purpose |
|---|---|---|
| `jpm-python.code-snippets` | `nupy` | Python script bootstrap |
| `jpm-python-snowflake.code-snippets` | `nupysf` | Python + Snowflake bootstrap |
| `jpm-sql-postgres.code-snippets` | `nupg`, `nupgw1`–`nupgw4` | PostgreSQL script + window functions |
| `jpm-sql-mssql.code-snippets` | `nums` | MS SQL script bootstrap |
| `jpm-sql-snowflake.code-snippets` | `nusf`, `nusfcsv` | Snowflake SQL bootstrap |

## Snippet File Format

Each file is a JSON object keyed by a human-readable name. Each snippet has:
- `prefix` — the trigger shorthand typed in the editor
- `scope` — language mode (e.g. `"sql"`, `"python"`)
- `description` — shown in IntelliSense
- `body` — array of strings, one per line; tab stops use `${N:placeholder}` syntax; `$CURRENT_YEAR`, `$CURRENT_MONTH`, `$CURRENT_DATE` are VS Code built-in variables

## Conventions

- Author line is always `Joseph P. Merten`
- Every snippet ends with a `-- Change Log` (SQL) or equivalent section
- SQL scripts include `BEGIN;` / `-- ROLLBACK;` / `-- COMMIT;` safety guards
- Tab stops are shared across the body using the same index (e.g. `${4:schema_name}` appears multiple times so editing one updates all)
- The final tab stop `${0}` marks the cursor's resting position after all placeholders are filled

## Open To-Do (from README)

Window function snippets for PostgreSQL are planned:
- `nupgw1` — Ranking (ROW_NUMBER, RANK, DENSE_RANK, NTILE) ✅ done
- `nupgw2` — Aggregate (SUM, AVG, COUNT running totals) ✅ done
- `nupgw3` — Value/Offset (LAG, LEAD, FIRST_VALUE, LAST_VALUE) ✅ done
- `nupgw4` — Distribution (PERCENT_RANK, CUME_DIST, PERCENTILE_CONT/DISC) ✅ done
