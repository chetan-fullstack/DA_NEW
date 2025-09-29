 **Lecture 1 – Task (Introduction to SQL)**
=============================================

### **Task 1: Install & Setup**

*   Install any one RDBMS of your choice:
    
    *   MySQL (with MySQL Workbench), OR
        
    *   PostgreSQL (with pgAdmin), OR
        
    *   SQLite (with DB Browser).
        

### **Task 2: Create a Database**

*   Create a database named **SchoolDB** (or any name you like).
    

Plain textANTLR4BashCC#CSSCoffeeScriptCMakeDartDjangoDockerEJSErlangGitGoGraphQLGroovyHTMLJavaJavaScriptJSONJSXKotlinLaTeXLessLuaMakefileMarkdownMATLABMarkupObjective-CPerlPHPPowerShell.propertiesProtocol BuffersPythonRRubySass (Sass)Sass (Scss)SchemeSQLShellSwiftSVGTSXTypeScriptWebAssemblyYAMLXML`   CREATE DATABASE SchoolDB;   `

### **Task 3: Create a Table**

*   Inside SchoolDB, create a table called **Students** with the following columns:
    
    *   StudentID → INT, Primary Key
        
    *   Name → VARCHAR(50), NOT NULL
        
    *   Age → INT, must be greater than 0
        
    *   City → VARCHAR(50), DEFAULT 'Unknown'
        

### **Task 4: Insert Records**

*   Insert at least 5 student records into the Students table.(Use your own names, ages, and cities).
    

### **Task 5: Run Your First Query**

*   Write a query to display **all records** from the Students table.
    

Plain textANTLR4BashCC#CSSCoffeeScriptCMakeDartDjangoDockerEJSErlangGitGoGraphQLGroovyHTMLJavaJavaScriptJSONJSXKotlinLaTeXLessLuaMakefileMarkdownMATLABMarkupObjective-CPerlPHPPowerShell.propertiesProtocol BuffersPythonRRubySass (Sass)Sass (Scss)SchemeSQLShellSwiftSVGTSXTypeScriptWebAssemblyYAMLXML`   SELECT * FROM Students;   `

 By completing this, students will:

*   Understand database creation.
    
*   Learn how to define tables, columns, and constraints.
    
*   Insert and view real data.