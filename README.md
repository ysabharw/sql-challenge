# SQL Challenge - Employee Database Analysis

## Project Overview

In this project, I built a relational database for a company that contains information about employees, their departments, and salaries. The database was constructed using PostgreSQL, and SQL queries were performed to extract meaningful insights. The challenge involved creating multiple tables, establishing relationships between them, and performing various data analysis queries.

## Technologies Used

* PostgreSQL
* pgAdmin4
* QuickDBD (for ERD creation)
* Python
* Git
* VS Code

## Database Schema

The database includes the following tables:

1. **Employees** : Stores employee information such as `emp_no`, `first_name`, `last_name`, `birth_date`, `sex`, `hire_date`, etc.
2. **Departments** : Stores department information like `dept_no` and `dept_name`.
3. **Dept_Emp** : Maps employees to their respective departments.
4. **Dept_Manager** : Stores department managers' information.
5. **Salaries** : Stores employees' salary information.
6. **Titles** : Stores job title information for employees.

### ERD Creation

* **pgAdmin4** : Used to visualize the database schema, relationships, and structure directly in PostgreSQL.
* **QuickDBD** : Used to create a quick Entity Relationship Diagram (ERD) during the design phase to visualize the relationships between tables before final implementation.

## Resources Used

Throughout the project, several external resources were referenced to resolve issues and build the project:

1. **PostgreSQL Official Documentation** :

* PostgreSQL docs were used to understand SQL query syntax and functions such as `COPY`, `CREATE TABLE`, and `FOREIGN KEY`.
* Link: [https://www.postgresql.org/docs/](https://www.postgresql.org/docs/)

1. **Stack Overflow** :

* Various posts on Stack Overflow helped resolve issues related to PostgreSQL, SQL queries, and pgAdmin setup.
* Examples:
  * [Issue with password authentication](https://stackoverflow.com/questions/46439870/password-authentication-failed-for-user-postgres)
  * [Troubleshooting database connections](https://stackoverflow.com/questions/62031339/postgresql-server-running-on-port-5432)

1. **QuickDBD** :

* QuickDBD was used to create the ERD (Entity Relationship Diagram) for visualizing table relationships and refining the database structure during the design phase.
* Link: [https://app.quickdatabasediagrams.com/]()

1. **pgAdmin4** :

* pgAdmin4 was used to visually interact with PostgreSQL, manage database connections, and monitor schema relationships in real-time.
* Link: [https://www.pgadmin.org/](https://www.pgadmin.org/)

1. **PostgreSQL Error Codes Reference** :

* Used for debugging PostgreSQL errors during schema creation.
* Link: [https://www.postgresql.org/docs/current/errcodes-appendix.html](https://www.postgresql.org/docs/current/errcodes-appendix.html)

## Queries

Some of the key queries performed in this project include:

* List the employee number, last name, first name, sex, and salary of each employee.
* List the first name, last name, and hire date for employees hired in 1986.
* List the manager of each department along with their employee number, last name, and department information.
* List the frequency counts of all employee last names (how many employees share each last name).

## Issues Faced and Solutions

1. **Password Authentication Failed** :

* Initially faced errors with password authentication while trying to connect to PostgreSQL from pgAdmin. After troubleshooting, the issue was resolved by resetting the password and ensuring that the correct role and privileges were assigned to the `postgres` user.
* Resources used:
  * Stack Overflow [Password authentication failed for user](https://stackoverflow.com/questions/46439870/password-authentication-failed-for-user-postgres)
  * PostgreSQL documentation on user roles and privileges.

1. **CSV Import Issues** :

* Encountered "file not found" errors when trying to import CSV files into the database using the `COPY` command. This was resolved by correctly setting the file paths and checking permissions.
* Resources used:
  * QuickDB for testing file imports.

1. **Git Push Error** :

* Faced issues while pushing the code to GitHub due to "remote origin already exists" error. This was resolved by running the `git remote remove origin` command and re-adding the correct remote.
* Stack Overflow: [Remote origin already exists error](https://stackoverflow.com/questions/24565723/fatal-remote-origin-already-exists)

## Credits

Special thanks to the following resources for helping me complete the challenge/project:

* PostgreSQL Official Documentation
* Stack Overflow community
* QuickDBD for ERD creation
* pgAdmin4 for database management and visualization
