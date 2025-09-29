 Stage 1: Introduction to SQL
===============================

1. **What is SQL?**
--------------------

*   **SQL (Structured Query Language)** is the standard programming language used to interact with **relational databases**.
    
*   It allows users to:
    
    *   **Query data** (retrieve specific information).
        
    *   **Insert new records** into a database.
        
    *   **Update existing data**.
        
    *   **Delete unwanted data**.
        
    *   **Manage structures** like tables, views, and indexes.
        

 **Key Characteristics of SQL**:

*   **Declarative language** → You describe what you want, not how to do it.
    
*   **Standardized** → SQL is ANSI/ISO standard (though vendors like MySQL, PostgreSQL, Oracle add extra features).
    
*   **Widely used** → Core to data analytics, web development, enterprise systems, and reporting.
    

 **Use Cases**:

*   Banks use SQL to maintain customer transactions.
    
*   E-commerce platforms use SQL to manage orders, inventory, and users.
    
*   Analysts use SQL to prepare data for reporting and dashboards.
    

2. **Databases, DBMS, and RDBMS**
----------------------------------

### **Database**

*   A collection of **organized data** that can be easily accessed, managed, and updated.
    
*   Example: A library database contains books, members, and borrowing records.
    

### **DBMS (Database Management System)**

*   Software used to **store, retrieve, and manage** data in databases.
    
*   Example: Microsoft Access, file-based storage systems.
    

### **RDBMS (Relational Database Management System)**

*   Special type of DBMS that organizes data into **tables** (relations).
    
*   Tables can be linked through **relationships** using keys.
    
*   Examples: MySQL, PostgreSQL, Oracle, SQL Server.
    

 **Difference between DBMS & RDBMS**:

*   DBMS → Works with files, does not enforce relationships.
    
*   RDBMS → Ensures relationships using **primary keys and foreign keys**, follows relational model by E. F. Codd.
    

3. **Tables, Rows, Columns, Schema**
-------------------------------------

*   **Table:** A structured format of data arranged in rows and columns.
    
*   **Row (Record):** A single data entry in a table.
    
*   **Column (Field):** A named attribute of data, like Name, Age, Salary.
    
*   **Schema:** The blueprint/structure of a database, showing how tables are defined and connected.
    

 **Example Table: Employees**

EmpIDNameAgeDepartmentCity101Arjun28HRDelhi102Meena32ITMumbai103Rakesh26FinanceChennai

Here:

*   EmpID is a column (unique for each row).
    
*   Each line represents a row (record).
    
*   The full table is part of a schema (could include other tables like Departments, Salaries, etc.).
    

4. **Keys and Constraints**
----------------------------

### **Keys**

*   **Primary Key** → Uniquely identifies each row in a table. Cannot be NULL or duplicate.Example: EmpID in Employees table.
    
*   **Foreign Key** → Links two tables together, referencing a primary key in another table.Example: DepartmentID in Employees table referencing Departments table.
    

### **Constraints**

Constraints are rules applied to table columns:

*   **NOT NULL** → Value cannot be left empty.
    
*   **UNIQUE** → Ensures all values in a column are distinct.
    
*   **CHECK** → Restricts data with a condition (e.g., Age > 18).
    
*   **DEFAULT** → Provides a default value when none is supplied.
    
*   **PRIMARY KEY** → Combination of NOT NULL + UNIQUE.
    
*   **FOREIGN KEY** → Ensures referential integrity between tables.
    

 Example:If Age must always be positive, we can apply a CHECK (Age > 0) constraint.

5. **Installing SQL**
----------------------

To practice SQL, we need an RDBMS. Options:

*   **MySQL**
    
    *   Widely used, open-source, supported on all platforms.
        
    *   Tools: MySQL Server + MySQL Workbench (GUI).
        
*   **PostgreSQL**
    
    *   Advanced open-source RDBMS with powerful features.
        
    *   Tools: PostgreSQL + pgAdmin.
        
*   **SQLite**
    
    *   Lightweight, file-based, requires no server setup.
        
    *   Tools: DB Browser for SQLite.
        

Other commercial options: Oracle, SQL Server.

6. **Writing Your First SQL Query**
------------------------------------

The **SELECT statement** is the most basic and powerful SQL command.

Plain textANTLR4BashCC#CSSCoffeeScriptCMakeDartDjangoDockerEJSErlangGitGoGraphQLGroovyHTMLJavaJavaScriptJSONJSXKotlinLaTeXLessLuaMakefileMarkdownMATLABMarkupObjective-CPerlPHPPowerShell.propertiesProtocol BuffersPythonRRubySass (Sass)Sass (Scss)SchemeSQLShellSwiftSVGTSXTypeScriptWebAssemblyYAMLXML`   SELECT * FROM Employees;   `

*   **SELECT** → Tells SQL you want to retrieve data.
    
*   **\*** → Means "all columns".
    
*   **FROM Employees** → The table to get data from.
    

 Example Output:

EmpIDNameAgeDepartmentCity101Arjun28HRDelhi102Meena32ITMumbai103Rakesh26FinanceChennai

 Later, we can refine queries to select **specific columns**:

Plain textANTLR4BashCC#CSSCoffeeScriptCMakeDartDjangoDockerEJSErlangGitGoGraphQLGroovyHTMLJavaJavaScriptJSONJSXKotlinLaTeXLessLuaMakefileMarkdownMATLABMarkupObjective-CPerlPHPPowerShell.propertiesProtocol BuffersPythonRRubySass (Sass)Sass (Scss)SchemeSQLShellSwiftSVGTSXTypeScriptWebAssemblyYAMLXML`   SELECT Name, City FROM Employees;   `

Output:

NameCityArjunDelhiMeenaMumbaiRakeshChennai

7. **Summary of Stage 1**
--------------------------

*   SQL is the standard language for relational databases.
    
*   Databases store data; RDBMS enforces relationships between tables.
    
*   Data is stored in **tables** made of rows and columns.
    
*   **Primary keys** uniquely identify records, while **foreign keys** link tables.
    
*   Constraints enforce rules on data.
    
*   First SQL command: SELECT \* FROM table;