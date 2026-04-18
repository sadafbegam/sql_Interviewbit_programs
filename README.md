# sql_Interviewbit_programs
# 🗄️ SQL InterviewBit Programs

A collection of SQL query solutions for problems from [InterviewBit](https://www.interviewbit.com/), covering a wide range of SQL concepts commonly tested in technical interviews.

---

## 📌 About

This repository contains solutions to SQL problems from InterviewBit's **Databases** section. Each solution is written as a clean SQL query with a focus on correctness and readability. The problems are based on classic relational schemas such as movies, actors, directors, and reviewers.

---

## 🗂️ Topics Covered

| Topic | Description |
|---|---|
| **SELECT & Filtering** | Basic SELECT queries, WHERE clauses, LIKE, BETWEEN |
| **Joins** | INNER JOIN, LEFT JOIN, self-joins across related tables |
| **Aggregations** | COUNT, SUM, AVG, MIN, MAX with GROUP BY and HAVING |
| **Subqueries** | Nested SELECT statements, correlated subqueries |
| **String Functions** | CONCAT, name formatting (first + last name combinations) |
| **NULL Handling** | IS NULL, IS NOT NULL, COALESCE |
| **Sorting & Limiting** | ORDER BY, LIMIT for top-N queries |

---

## 🗃️ Schema Overview

Most problems revolve around a **Movies** database with the following tables:

```
Movie        (movie_id, movie_title, movie_year, director_id, ...)
Director     (director_id, director_first_name, director_last_name)
Actor        (actor_id, actor_first_name, actor_last_name)
Cast         (actor_id, movie_id, role)
Reviewer     (reviewer_id, reviewer_name)
Rating       (reviewer_id, movie_id, stars, rating_date)
```

> **Note:** Name fields are typically concatenated **without a delimiter**, e.g., `'Alfred'` + `'Hitchcock'` → `'AlfredHitchcock'`.

---

## 📝 Sample Problems

- Find movies with the lowest duration along with the director's and actor's names
- Find all reviewers who gave a NULL rating
- Find movies where one or more actors acted in two or more movies
- Find the movie title and director name for a specific role (e.g., `'SeanMaguire'`)
- Fetch department-wise employee counts sorted in descending order

---

## 🚀 How to Use

1. **Clone the repository**
   ```bash
   git clone https://github.com/sadafbegam/sql_Interviewbit_programs.git
   cd sql_Interviewbit_programs
   ```

2. **Set up a local database** (MySQL recommended)
   ```sql
   -- Create and populate the schema before running queries
   SOURCE schema.sql;
   SOURCE seed_data.sql;
   ```

3. **Run any query**
   ```bash
   mysql -u root -p your_database < query_file.sql
   ```

---

## 🛠️ Prerequisites

- MySQL 5.7+ or any SQL-compatible database
- A SQL client such as MySQL Workbench, DBeaver, or the command-line `mysql` client

---

## 🤝 Contributing

Contributions, alternative solutions, and optimizations are welcome!

1. Fork this repository
2. Create a new branch: `git checkout -b feature/new-solution`
3. Commit your changes: `git commit -m "Add solution for <problem-name>"`
4. Push and open a Pull Request

---

## 📚 Resources

- [InterviewBit SQL Problems](https://www.interviewbit.com/sql-interview-questions/)
- [MySQL Documentation](https://dev.mysql.com/doc/)
- [W3Schools SQL Tutorial](https://www.w3schools.com/sql/)

---

## 👩‍💻 Author

**Sadaf Begam** — [GitHub Profile](https://github.com/sadafbegam)

---

## ⭐ Show Your Support

If you found this helpful, please consider giving the repo a ⭐ — it helps others find it too!
