ELS STUDY BUDDY DATABASE

Ozan Umut Güney, 200302109
Ethem Kesim, 210302205 
Emre Çubuk, 220302393
Contents



1. Project Overview
The ELS Study Buddy Database is designed to manage and organize the resources, classrooms, language levels, professors, students, and tutors associated with an English Language School (ELS). The database comprises several tables, each serving a specific purpose within the school's ecosystem.

2. Methodology
2.1 Tables
1.	books

Purpose: To store information about the books used in the study programs.
Columns:
•	book_id (int, Primary Key): Unique identifier for each book.
•	title (varchar(100)): Title of the book.
•	language_level_id (int, Foreign Key): References the language level associated with the book.
 
2.	classrooms

•	Purpose: To store details about the classrooms available for use.
•	Columns:
•	classroom_id (int, Primary Key): Unique identifier for each classroom.
•	capacity (int): The capacity of the classroom in terms of student accommodation.
 
3.	languagelevel

•	Purpose: To define the different language proficiency levels.
•	Columns:
•	language_level_id (int, Primary Key): Unique identifier for each language level.
•	level_name (varchar(100)): Name or description of the language level (e.g., Beginner, Intermediate, Advanced).
 
4.	professors

•	Purpose: To store information about the professors teaching at the school.
•	Columns:
•	professor_id (int, Primary Key): Unique identifier for each professor.
•	FirstName (varchar(100)): First name of the professor.
•	MiddleName (varchar(100)): Middle name of the professor.
•	LastName (varchar(100)): Last name of the professor.
•	Email (varchar(100)): Email of professor.
•	Phone (varchar(100)): Phone of professor.
•	Adress (varchar(100)): Adress of professor.
 

5.	students

•	Purpose: To store information about the students enrolled in the school.
•	Columns:
•	student_id (int, Primary Key): Unique identifier for each student.
•	FirstName (varchar(100)): First name of the student.
•	MiddleName (varchar(100)): Middle name of the student.
•	LastName (varchar(100)): Last name of the student.
•	Email (varchar(100)): Email of student.
•	Phone (varchar(100)): Phone of student.
•	Address (varchar(100)): Address of student.
•	language_level_id (int, Foreign Key): References the language level associated with the students.
 

6.	tutors

•	Purpose: To store information about the tutors who assist students with their studies.
•	Columns:
•	tutor_id (int, Primary Key): Unique identifier for each tutor.
•	FirstName (varchar(100)): First name of the tutor.
•	MiddleName (varchar(100)): Middle name of the tutor.
•	LastName (varchar(100)): Last name of the tutor.
•	Email (varchar(100)): Email of tutor.
•	Phone (varchar(100)): Phone of tutor.
•	Address (varchar(100)): Address of tutor.
•	language_level_id (int, Foreign Key): References the language level associated with the tutors.
 
2.2 Relationships
•	The books table is related to the languagelevel table through the language_level_id.
•	The professors table is related to the languagelevel table through the language_level_id.
•	The students table is related to the languagelevel table through the language_level_id.
•	The tutors table is related to the languagelevel table through the language_level_id.
2.3 Er Diagram
 


3. Conclusion
This database schema helps in managing the educational resources efficiently, organizing classroom allocations, and tracking both student progress and professor and tutor assignments within the IUS English Language School.
