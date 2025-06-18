# Class-Occupancy-Tracker
Classroom Occupancy Management System
A fully-featured, menu-driven C++ console application for managing classrooms, teachers, and students within a building. Designed as an academic OOP (Object-Oriented Programming) project, this system provides functionalities for handling room allocations, staff assignments, student management, and occupancy reporting through an interactive command-line interface.

Project Motivation
Managing classrooms in educational institutions can become complex when it comes to tracking room capacities, teacher assignments, student enrollments, and room occupancy statuses. This project was developed to:

Apply object-oriented programming principles (Inheritance, Polymorphism, Encapsulation)

Practice class composition and dynamic memory management in C++

Simulate a practical classroom management scenario within a building

Create a simple, user-friendly console-based management tool

Technologies Used
Language: C++ (Object-Oriented Programming)
Compiler: GCC / g++
User Interface: Console-based (command-line)

File Structure
Project/
│
├── 3.cpp → Complete source code implementation
└── README.txt → Project documentation

System Design Overview
Classes & Relationships:

Person (Abstract Base Class)

Attributes: name, id

Pure virtual function: displayInfo()

Student (inherits from Person)

Attribute: program

Implements displayInfo()

Teacher (inherits from Person)

Attribute: subject

Implements displayInfo()

Classroom

Attributes: roomNumber, capacity

Pointer to Teacher

Array of Students

Logs for activities (adding/removing students, assigning teachers)

Functions: addStudent, removeStudent, assignTeacher, transferStudent, displayDetails, save

Building

Attribute: name

Array of Classrooms

Functions: addClassroom, searchStudentById, searchTeacherById, transferStudent, displayAllClassrooms, showSummary, saveData

Key Features
✔ Add Classrooms
✔ Assign Teachers to Classrooms
✔ Add Students to Classrooms (with duplicate ID check and capacity limit)
✔ Remove Students by ID
✔ Transfer Students Between Classrooms
✔ Search for a Student or Teacher by ID (with room number display)
✔ Display Full Classroom Details (occupancy, students, teacher, activity logs)
✔ Show Building Summary (total occupancy percentage, room-wise status)
✔ Save Room Data in a formatted console display
✔ Simple, Interactive Menu-Driven Console Interface

How to Compile & Run
To Compile:
g++ 3.cpp -o classroom_system

To Run:
./classroom_system

Program Menu Options
Add Classroom

Assign Teacher

Add Student

Remove Student

Show All Classrooms

Search Student by ID

Search Teacher by ID

Transfer Student

Show Building Summary

Save Data

Exit

Example Functionalities
Add a Classroom: Enter room number and capacity.

Assign a Teacher: Enter room number, teacher’s name, ID, and subject.

Add a Student: Enter room number, student’s name, ID, and program.

Remove a Student: Enter room number and student ID.

Transfer a Student: Enter student ID, source room number, and destination room number.

Show Building Summary: Displays total students, total capacity, and occupancy percentage.

Save Data: Outputs current classroom and student records in a formatted display.

Sample Data Save Format
Room:101|Capacity:40|Students:12,Ali;14,Sana;|Teacher:22,Mr. Kamran

Occupancy Status Example
Classroom 101 [Capacity: 40, Occupied: 20, Status: Partially Occupied (50%)]
Occupancy: [##### ] 50%

Learning Outcomes
Practical application of Object-Oriented Programming concepts: Inheritance, Polymorphism, Encapsulation, Class composition

Dynamic memory management using pointers

Managing collections of objects using arrays

Interactive menu-driven programming structure in C++

Input validation and error handling

Implementation of validation checks for IDs and capacities

Limitations
No persistent file storage (data saving is displayed on the console only)

Fixed array sizes (can be improved via dynamic data structures such as vectors)

Console-only interaction (no graphical interface)


License
This project is open for educational use and practice purposes. No commercial distribution without prior permission.

Final Notes
This project is a solid demonstration of practical C++ object-oriented programming, implementing real-world academic management operations through classes, inheritance, and menu-driven interaction. It can be extended by adding file-based data storage, a GUI interface, or using dynamic data structures for more flexibility.

