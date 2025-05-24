# Final-lab-task-2

This portfolio demonstrates my understanding of MySQL database creation using a simplified student assignment submission system. It goes over how to create tables that show students, assignments, and their contributions step-by-step. In order to create a completely effective relational schema, this exercise uses data types, relationships, and constraints such as primary keys, foreign keys, and composite keys.

# 1. Create the student table:
Define username as a VARCHAR(50)
Set username as the Primary Key
# 2. Create the assignment table:
Define shortname as a VARCHAR(50) and set it as the Primary Key
Define due_date as a DATE NOT NULL
Define url as a VARCHAR(255), which can be null
# 3. Create the submission table:
Define username and shortname both as VARCHAR(50)
Define version as an INT
Define submit_date as a DATE NOT NULL
Define data as TEXT
Set a composite primary key of (username, shortname, version)
Add foreign keys referencing the student and assignment tables

Table Relationships
# 1. student table
Primary Key: username
Relationships:
One-to-Many with submission: One student (username) can have many submissions.
# 2. assignment table
Primary Key: shortname
Relationships:
One-to-Many with submission: One assignment (shortname) can have many submissions.
# 3. submission table
Composite Primary Key: (username, shortname, version)
Relationships:
Many-to-One with student: Each submission belongs to one student.
Many-to-One with assignment: Each submission is for one assignment.
This models a Many-to-Many relationship between students and assignments, with version tracking multiple submissions.

# Screenshots
# Student Query Statemen

![a](https://github.com/user-attachments/assets/d15e368e-82b0-40ae-bf4f-9c9b57e76048)
- Assignment Query Statement

![b](https://github.com/user-attachments/assets/7b669136-19ff-4dbe-934d-afe4622b205d)
- Submission Query Statement

![c](https://github.com/user-attachments/assets/7358d93f-59a3-4809-80e6-2b10d87d6c15)
- Student Table

![d](https://github.com/user-attachments/assets/21ca737f-e2e2-47dd-9030-438e5b20d312)
- Assignment Table

![e](https://github.com/user-attachments/assets/60388e86-db82-4db8-8de0-4900fb9fefb1)
- Submission Table

![f](https://github.com/user-attachments/assets/ae30fbd4-3e33-4821-8aa5-b8fdab29fb53)
- ER Diagram

![g](https://github.com/user-attachments/assets/1bc1eb03-08fd-41ac-960d-b30dd81179ea)
- Relational Tables

![h](https://github.com/user-attachments/assets/917eb482-1d4c-4035-8e8a-ef2e35b23fb3)
- Sql copy of the database and table structures

![i](https://github.com/user-attachments/assets/bf657df0-490d-444d-89b2-09b8e43ea13d)











