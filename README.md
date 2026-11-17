🎓 Student Management System
A Student Management System built using FastAPI, Python, HTML, CSS, Jinja2 Templates, and SQLite. This web application helps manage student records efficiently through a user-friendly and responsive interface.

The system provides complete CRUD (Create, Read, Update, Delete) functionality, allowing users to add, view, update, and delete student information stored in a SQLite database. It also includes data validation using Pydantic models to ensure accurate student records.

🚀 Features
👨‍🎓 Student Management
Add new student records
View all students
View individual student details
Update student information
Delete student records
📋 Student Information
Each student record contains:

Student Name
Age
Gender
Course
Marks
Profile Image URL
Student Status (Active / Inactive)
✅ Data Validation
Age validation (1-100)
Marks validation (0-100)
Status validation (0 or 1)
Required field validation using Pydantic
🗄️ Database Management
SQLite database integration
Automatic table creation
Persistent data storage
Efficient record retrieval
🎨 User Interface
Responsive design
Simple and clean UI
Easy navigation
Dynamic HTML rendering using Jinja2 Templates
🛠️ Technologies Used
Backend
FastAPI
Python
Pydantic
Frontend
HTML5
CSS3
Jinja2 Templates
Database
SQLite3
📂 Project Structure
students-management-system/
│
├── main.py
├── students.db
│
├── templates/
│   ├── Home.html
│   ├── add-student.html
│   ├── single-std.html
│   └── update_std.html
│
├── static/
│   ├── css/
│   └── images/
│
└── README.md
🔄 CRUD Operations
➕ Create Student
Route
GET /students/add
POST /students/add
Description
Allows users to add a new student record to the database.

📖 Read Student Records
View All Students
GET /
View Single Student
GET /students/{student_id}
Description
Displays all students or a specific student's details.

✏️ Update Student
Route
GET /students/update/{student_id}
POST /students/update/{student_id}
Description
Allows editing and updating existing student information.

❌ Delete Student
Route
POST /students/delete/{student_id}
Description
Deletes a student record from the database.

🗃️ Database Schema
CREATE TABLE students(
    id INTEGER PRIMARY KEY AUTOINCREMENT,
    name TEXT NOT NULL,
    age INTEGER NOT NULL,
    course TEXT NOT NULL,
    marks INTEGER NOT NULL,
    image TEXT,
    gender TEXT NOT NULL,
    status INTEGER
);
📊 Student Attributes
Field	Type	Description
id	Integer	Unique Student ID
name	Text	Student Name
age	Integer	Student Age
course	Text	Course Name
marks	Integer	Student Marks
image	Text	Profile Image URL
gender	Text	Gender
status	Integer	Active (1) / Inactive (0)
▶️ Installation & Setup
Clone the Repository
git clone https://github.com/Gandla-Navya24/students-management-system.git
cd students-management-system
Create Virtual Environment
python -m venv venv
Activate Environment
Windows
venv\Scripts\activate
Mac/Linux
source venv/bin/activate
Install Dependencies
pip install fastapi uvicorn jinja2 python-multipart
Run the Application
uvicorn main:app --reload
Open Browser
http://127.0.0.1:8000
🎯 Learning Objectives
This project demonstrates:

FastAPI fundamentals
CRUD Operations
SQLite database integration
Pydantic validation
Jinja2 template rendering
Form handling in FastAPI
Responsive web design using HTML & CSS
📸 Application Workflow
Add Student
Save Data in SQLite Database
View Student List
View Student Details
Update Student Information
Delete Student Records
Display Updated Results
🤝 Contributing
Contributions are welcome. Feel free to fork the repository, create a new branch, and submit a pull request.

📄 License
This project is developed for educational and learning purposes.
