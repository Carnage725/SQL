# 20-Day SQL + DBMS + PostgreSQL Syllabus (80/20 Edition)

**Profile:** Complete beginner | 2 hours/day | Must-master content only
**Split:** Days 1–8 (Real-world foundations) → Days 9–20 (Problem solving + interview prep)
**Format:** Theory + examples → 3–5 exercises per day

---

## Phase 1: Real-World Foundations (Days 1–8)

| Day | SQL Topic | DBMS Concept |
|-----|-----------|--------------|
| **1** | SELECT, FROM, WHERE, aliases, LIMIT | What is RDBMS, client-server model |
| **2** | AND/OR/NOT, IN, BETWEEN, LIKE, ORDER BY, IS NULL | Data types, schemas, NULL |
| **3** | COUNT, SUM, AVG, MIN, MAX, GROUP BY, HAVING | Primary keys, entity integrity |
| **4** | INNER JOIN, LEFT JOIN, multi-table joins | Foreign keys, relationships (1:1, 1:M, M:M) |
| **5** | Self-joins, LEFT JOIN + IS NULL pattern, JOINs + aggregates | Normalization: 1NF, 2NF, 3NF |
| **6** | Subqueries (WHERE, FROM, SELECT), correlated subqueries | ACID properties, transactions (BEGIN/COMMIT/ROLLBACK) |
| **7** | CTEs (WITH), views, DISTINCT ON (PG) | Indexes: B-tree, when to index, trade-offs |
| **8** | EXPLAIN ANALYZE, reading query plans, creating indexes | Phase 1 capstone: build a schema + 10 real-world queries |

---

## Phase 2: Problem Solving + Interview Prep (Days 9–20)

| Day | SQL Pattern | Key Techniques |
|-----|-------------|----------------|
| **9** | CASE WHEN + conditional logic | CASE in SELECT, CASE inside aggregates (conditional aggregation), COALESCE, type casting |
| **10** | Window functions — ranking | ROW_NUMBER(), RANK(), DENSE_RANK(), PARTITION BY |
| **11** | Window functions — calculations | LAG(), LEAD(), SUM() OVER, running totals, moving averages |
| **12** | Top-N per group | ROW_NUMBER() + CTE filter, LATERAL joins (PG) |
| **13** | Aggregation problems | GROUP BY + HAVING combos, finding duplicates (COUNT > 1), conditional aggregation |
| **14** | JOIN-heavy problems | Multi-table reasoning, NULLs from LEFT JOINs, self-join patterns |
| **15** | Subquery problems | EXISTS vs IN, scalar subqueries, derived tables |
| **16** | Date & string manipulation | DATE_TRUNC, EXTRACT, AGE, TO_CHAR, string functions (PG) |
| **17** | JSONB queries (PG) | ->, ->>, @>, jsonb_array_elements, indexing JSONB with GIN |
| **18** | Mixed medium problems (timed) | Combine all patterns, 45-min mock |
| **19** | DBMS theory rapid-fire | Normalization deep-dive, ACID, MVCC (PG), isolation levels, index types, concurrency |
| **20** | Final mock interview | 10 DBMS theory questions + 5 SQL problems (easy → hard), full review |

---

## Daily Structure (2 hours)

| Block | Duration | Activity |
|-------|----------|----------|
| Theory | 30 min | Concept explanation + worked examples |
| Guided practice | 30 min | Walk through 2–3 queries step by step |
| Exercises | 45 min | Solve 3–5 problems independently |
| Review | 15 min | Check solutions, note patterns |

---

## DBMS Interview Checklist

- [ ] What is DBMS / RDBMS / SQL
- [ ] ACID properties (explain each)
- [ ] Keys: Primary, Foreign, Candidate, Composite
- [ ] Normalization: 1NF → 2NF → 3NF (with examples)
- [ ] Denormalization: when and why
- [ ] Relationships: 1:1, 1:M, M:M
- [ ] Indexes: B-tree, GIN, when to use, trade-offs
- [ ] Transactions & isolation levels
- [ ] MVCC in PostgreSQL
- [ ] Views vs materialized views
- [ ] Query optimization with EXPLAIN

---

## How to Use

Each day, say: **"Day X — teach me"**

I'll give you theory, examples, and 3–5 exercises.