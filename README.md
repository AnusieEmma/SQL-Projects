Library Management System (LibraryDB)
A robust, relational SQL database schema designed to manage library operations, including inventory tracking, member registration, book borrowing, and staff management.
📌 Project Overview
This project implements a fully normalized relational database (RDBMS) for a library. It handles complex relationships, such as many-to-many links between books and authors, and tracks the lifecycle of a book from reservation to borrowing and eventual return.
🚀 Features
Inventory Management: Track books, publishers, and available copies.
Member & Staff Tracking: Separate tables for library patrons and employees.
Many-to-Many Relationships: Handles books with multiple authors and authors with multiple books.
Transaction Logs: Tracks borrowing history, due dates, and fines.
Reservation System: Allows members to put a "hold" on books.
Data Integrity: Uses Primary Keys, Foreign Keys, and Unique constraints to ensure data accuracy.
📊 Database Schema
The database consists of the following tables:
Books: Stores title, ISBN, category, and stock levels.
Authors: Stores author names.
BookAuthors: Junction table linking Books and Authors.
Members: Profiles of people registered to borrow books.
Staff: Library employees managing transactions.
BorrowRecords: Records of which book was borrowed by whom, including fine tracking.
Reservations: Tracking "hold" requests for books.
🛠️ Requirements
MySQL (v8.0+) or MariaDB.
A SQL client like MySQL Workbench, DBeaver, or the Command Line Interface (CLI).
