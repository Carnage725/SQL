# 30-Day SQL + DBMS + PostgreSQL Syllabus

**Profile:** Complete beginner | 2 hours/day | 80/20 focused
**Split:** Days 1–12 (Real-world foundations) → Days 13–30 (LeetCode-style problem solving)
**Format:** Theory + examples → 3–5 exercises per day

---

## Phase 1: Real-World Foundations (Days 1–12)

### Week 1: SQL Core — The 20% That Does 80% of the Work

| Day | Topic | Focus | DBMS Concept |
|-----|-------|-------|--------------|
| **1** | Setup + SELECT basics | SELECT, FROM, WHERE, column aliases, LIMIT | What is a database, DBMS, RDBMS, client-server model |
| **2** | Filtering & sorting | Comparison operators, AND/OR/NOT, IN, BETWEEN, LIKE, ORDER BY, NULL handling (IS NULL) | Tables, rows, columns, data types, schemas |
| **3** | Aggregate functions | COUNT, SUM, AVG, MIN, MAX, GROUP BY, HAVING | Primary keys, uniqueness, entity integrity |
| **4** | JOINs — Part 1 | INNER JOIN, LEFT JOIN — concept of linking tables | Foreign keys, referential integrity, relationships (1:1, 1:M, M:M) |
| **5** | JOINs — Part 2 | RIGHT JOIN, FULL OUTER JOIN, self-joins, multi-table joins | Normalization: 1NF, 2NF, 3NF (why we split tables) |
| **6** | Subqueries | Subqueries in WHERE, FROM, SELECT; correlated vs non-correlated | ACID properties (Atomicity, Consistency, Isolation, Durability) |
| **7** | Week 1 review + practice | Mixed problems covering Days 1–6 | Review all DBMS concepts so far |

### Week 2: Real-World SQL + PostgreSQL Specifics

| Day | Topic | Focus | DBMS / PostgreSQL Concept |
|-----|-------|-------|---------------------------|
| **8** | INSERT, UPDATE, DELETE | DML operations, RETURNING clause (PG), WHERE in UPDATE/DELETE safety | Transactions: BEGIN, COMMIT, ROLLBACK |
| **9** | CREATE TABLE + constraints | Data types (INTEGER, VARCHAR, TEXT, BOOLEAN, TIMESTAMP, SERIAL, UUID), PRIMARY KEY, FOREIGN KEY, UNIQUE, NOT NULL, DEFAULT, CHECK | DDL vs DML vs DCL, PostgreSQL-specific types |
| **10** | Indexes & EXPLAIN | CREATE INDEX, B-tree basics, reading EXPLAIN ANALYZE output, when to index | How indexes work (B-tree), query execution plans, trade-offs |
| **11** | Views, CTEs, DISTINCT ON | CREATE VIEW, WITH (CTEs) for readable queries, PG's DISTINCT ON | Logical vs physical data independence, views as abstraction |
| **12** | Phase 1 capstone | Build a small schema (e-commerce: users, products, orders, order_items), write 10 real-world queries | ER diagrams, schema design process, denormalization trade-offs |

---

## Phase 2: LeetCode-Style Problem Solving (Days 13–30)

### Week 3: Pattern-Based Problem Solving

| Day | Topic | Pattern | Key Techniques |
|-----|-------|---------|----------------|
| **13** | Easy SELECTs + filtering | Direct retrieval | WHERE gymnastics, CASE WHEN, COALESCE, type casting |
| **14** | Aggregation problems | Group-and-filter | GROUP BY + HAVING combos, conditional aggregation (SUM(CASE...)) |
| **15** | JOIN problems | Multi-table reasoning | Choosing the right JOIN type, handling NULLs from LEFT JOINs |
| **16** | Subquery problems | Nested logic | EXISTS vs IN, scalar subqueries, derived tables |
| **17** | Ranking & window functions — Part 1 | Row numbering | ROW_NUMBER(), RANK(), DENSE_RANK(), PARTITION BY |
| **18** | Window functions — Part 2 | Running calculations | LAG(), LEAD(), SUM() OVER, moving averages, cumulative sums |
| **19** | Week 3 review | Mixed medium problems | Combine all patterns learned so far |

### Week 4: Advanced Patterns + Interview Favorites

| Day | Topic | Pattern | Key Techniques |
|-----|-------|---------|----------------|
| **20** | String & date manipulation | Data transformation | PG functions: TO_CHAR, DATE_TRUNC, EXTRACT, AGE, string functions |
| **21** | Finding duplicates & gaps | Data quality patterns | GROUP BY + HAVING COUNT > 1, self-joins for gaps, EXCEPT |
| **22** | Top-N per group | Partitioned ranking | ROW_NUMBER() + CTE/subquery filter, LATERAL joins (PG) |
| **23** | Consecutive problems | Sequence detection | LAG/LEAD for streaks, difference-of-row-numbers trick |
| **24** | Pivoting & unpivoting | Reshape data | CASE + aggregation pivot, CROSSTAB (PG), UNION ALL for unpivot |
| **25** | Recursive CTEs | Hierarchical data | WITH RECURSIVE for trees, org charts, bill of materials |
| **26** | Week 4 review | Mixed hard problems | Timed practice — simulate interview conditions |

### Days 27–30: Interview Prep & Consolidation

| Day | Topic | Focus |
|-----|-------|-------|
| **27** | DBMS theory rapid-fire | Normalization deep-dive, ACID vs BASE, CAP theorem basics, indexing types (B-tree, Hash, GIN, GiST in PG), concurrency control (locks, MVCC in PG) |
| **28** | PostgreSQL-specific features | JSONB queries, array types, LATERAL joins, UPSERT (ON CONFLICT), partitioning basics, pg_stat for monitoring |
| **29** | Mock interview — SQL problems | 5 timed problems (easy → hard), 45-minute mock |
| **30** | Mock interview — DBMS Q&A + SQL | 10 DBMS theory questions + 3 hard SQL problems, full review |

---

## Daily Structure (2 hours)

| Block | Duration | Activity |
|-------|----------|----------|
| **Theory** | 30 min | Read concept explanation + study worked examples |
| **Guided practice** | 30 min | Walk through 2–3 example queries step by step |
| **Exercises** | 45 min | Solve 3–5 problems independently |
| **Review** | 15 min | Check solutions, note patterns, update cheat sheet |

---

## DBMS Interview Topics Checklist

These are sprinkled throughout the 30 days but here's the consolidated list:

- [ ] What is DBMS / RDBMS / SQL
- [ ] ACID properties
- [ ] Keys: Primary, Foreign, Candidate, Super, Composite
- [ ] Normalization: 1NF, 2NF, 3NF, BCNF
- [ ] Denormalization: when and why
- [ ] ER diagrams & relationships (1:1, 1:M, M:M)
- [ ] Indexing: B-tree, Hash, when to use, trade-offs
- [ ] Transactions & isolation levels
- [ ] Concurrency: locks, deadlocks, MVCC (PostgreSQL)
- [ ] Views vs materialized views
- [ ] Stored procedures & functions (basics)
- [ ] CAP theorem (basics)
- [ ] Query optimization & EXPLAIN

---

## PostgreSQL-Specific Topics Checklist

- [ ] Data types: SERIAL, UUID, JSONB, ARRAY, TIMESTAMP WITH TIME ZONE
- [ ] DISTINCT ON
- [ ] RETURNING clause
- [ ] UPSERT (INSERT ... ON CONFLICT)
- [ ] LATERAL joins
- [ ] JSONB operators & functions
- [ ] EXPLAIN ANALYZE reading
- [ ] Common Table Expressions (WITH)
- [ ] Recursive CTEs (WITH RECURSIVE)
- [ ] CROSSTAB for pivoting
- [ ] Index types: B-tree, GIN, GiST
- [ ] MVCC & transaction isolation

---

## How to Use This With Claude

Each day, come to this chat and say:

> **"Day X — teach me [topic]"**

I'll give you:
1. Clear theory explanation with examples
2. A practice table/dataset to work with
3. 3–5 exercises (easy → medium)
4. Solutions when you're ready

Let's start whenever you're ready with **Day 1**.