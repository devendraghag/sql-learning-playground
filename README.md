# SQL Learning Playground

A self-contained SQL learning page for beginners. Explore a sample shop database, edit PostgreSQL-style queries, and see results immediately in your browser.

## Open it

Download or clone this repository, then open sql-playground.html directly in a modern browser. No server, database, build step, package install, or network connection is needed.

## What’s inside

- Query editor, lesson picker, Run and Reset controls
- Related customers, orders, and products sample tables with a table browser
- Beginner examples for filtering, joins, grouping, aggregates, sorting, limits, NULLs, and CASE
- Temporary in-page INSERT, UPDATE, and DELETE examples
- A categorized guide distinguishing runnable simulator features from illustrative PostgreSQL syntax
- Responsive layout, Ctrl/⌘ + Enter shortcut, and clear unsupported-statement feedback

## Simulator scope

This is a teaching interpreter, not PostgreSQL or a SQL validator. It runs a deliberately small PostgreSQL-style subset: SELECT with basic projections, DISTINCT, INNER/LEFT JOIN, WHERE comparisons and AND/OR, IS NULL, IN, BETWEEN, LIKE, GROUP BY, HAVING with aggregates, ORDER BY, LIMIT/OFFSET, basic COUNT/SUM/AVG/MIN/MAX, CASE, and COALESCE. It also runs simple single-row INSERT, one-column UPDATE with WHERE, and DELETE with WHERE. Changes live only in the open page; Reset restores the original rows.

Set operations, RIGHT/FULL/CROSS/SELF joins, subqueries, CTEs, window functions, MERGE, TRUNCATE, schema changes, constraints, permissions, and transaction controls are explained as examples and do not execute here. Unsupported input shows a message. The interpreter supports simple educational syntax and does not reproduce PostgreSQL’s planner, types, constraints, concurrency, or complete NULL semantics. Try illustrative syntax in PostgreSQL to learn its full behavior.

## PostgreSQL and dialect notes

PostgreSQL uses LIMIT (and also supports FETCH FIRST); SQL Server commonly uses TOP. PostgreSQL uses EXCEPT for set difference, while Oracle commonly uses MINUS. Other SQL syntax and behavior may vary by database.

## Project files

- sql-playground.html — complete standalone page (HTML, CSS, JavaScript, sample data, and lessons)
- README.md — this guide

## License

MIT
