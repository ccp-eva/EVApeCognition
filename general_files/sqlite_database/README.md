 # <img src="https://github.com/user-attachments/assets/cee0bb16-3166-4109-b489-e646159b40c3" alt="Logo-EVApeCognition" width="30"> EVApeCognition Database

To facilitate navigation of the EVApeCognition database, feel free to use the EVApeCognition.db file by opening the jupyter notebook file titled sqlite_examples.ipynb and following the instructions within. These instructions will guide you through a few examples of search queries which you can adapt to your own interests. 

Database created with SQLite (Hipp, 2000). See Hipp, D. R. (2000). SQLite. http://sqlite.org/

Representation of the database structure

![Diagram_data_final](https://github.com/user-attachments/assets/a12dbd69-3a5b-44e7-9aa1-7a61bf9f917c)


Here are some general keywords to facilitate the creation of SQLite queries in R

| SQL Term     | Meaning / Usage                                                                                          | R Example (inside `dbGetQuery()`)                                    |
| ------------ | -------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------- |
| **SELECT**   | Choose which columns to return. Use `DISTINCT` to get unique rows (no duplicates).                       | `"SELECT DISTINCT species FROM participant"`                         |
| **FROM**     | The table(s) to query data from.                                                                         | `"FROM participant"`                                                 |
| **JOIN**     | Combine rows from two or more tables based on a related column. Types include `INNER JOIN`, `LEFT JOIN`. | `"FROM participant JOIN dyad ON participant.ind_id = dyad.ind_1_id"` |
| **WHERE**    | Filter rows by a condition. Only rows matching this condition are returned.                              | `"WHERE species = 'chimpanzee'"`                                     |
| **ORDER BY** | Sort the results by one or more columns, ascending (`ASC`) or descending (`DESC`).                       | `"ORDER BY year_of_birth DESC"`                                      |
| **LIMIT**    | Limit the number of rows returned. Useful to get just the first few rows.                                | `"LIMIT 10"`                                                         |
| **OFFSET**   | Skip a number of rows before returning results (for pagination).                                         | `"LIMIT 10 OFFSET 20"`                                               |
| **GROUP BY** | Group rows by column(s) to apply aggregate functions (e.g., `COUNT()`, `SUM()`, `AVG()`).                | `"GROUP BY species"`                                                 |
| **HAVING**   | Filter groups created by `GROUP BY` using conditions on aggregates.                                      | `"HAVING COUNT(*) > 5"`                                              |
| **COUNT()**  | Aggregate function counting rows in each group or total.                                                 | `"SELECT species, COUNT(*) FROM participant GROUP BY species"`       |
| **AS**       | Rename a column or expression in the result for clarity.                                                 | `"COUNT(*) AS num_participants"`                                     |
| **COALESCE** | Returns the first non-NULL value from the list. Useful to replace NULLs with default values.             | `"SELECT COALESCE(year_of_birth, 'unknown') FROM participant"`       |
| **CAST**     | Converts `expr` to a specified data type (`TEXT`, `INTEGER`, etc.)                                       | `"SELECT CAST(year_of_birth AS TEXT) FROM participant"`              |
