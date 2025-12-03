# Student-Management-System
# ☕ Java Lab Assignment 3:  Student Management System

## Project Overview

This project implements an enhanced **Student Management System** in Java, focusing on key advanced concepts to ensure safe execution and a responsive user interface.







***

## ✨ Key Features Implemented

The system adheres to all assignment requirements, including the use of custom exceptions, multithreading, and Java wrapper classes.

### 1. Exception Handling (`try-catch-finally` and Custom Exception)
* **Custom Exception:** Implements `StudentNotFoundException` (a static nested class) to handle cases where a student record cannot be processed or located.
* **Input Validation:** Uses `try-catch` blocks to handle runtime errors like `InputMismatchException` (for non-numeric input) and performs logical validation for invalid marks (outside 0-100 range) and empty required fields (Name/Course).
* **Resource Management:** The `finally` block ensures the `Scanner` resource is always closed.

### 2. Multithreading for Responsiveness
* **Loader Thread:** The `Loader` class implements the `Runnable` interface to simulate a data processing delay (3 seconds).
* **Responsive UI Simulation:** A new `Thread` is created and joined (`loadingThread.join()`) to simulate a "Loading..... Done." status, ensuring the application remains responsive during the simulated background task.

### 3. Wrapper Classes and Autoboxing
* The `Student` class uses **Wrapper Classes** (`Integer` for roll number, `Double` for marks) instead of primitives.
* **Autoboxing** is demonstrated when taking primitive inputs from the `Scanner` (`int` to `Integer` and `double` to `Double`) before creating the `Student` object.

***
   
4.  **Input:** Follow the on-screen prompts to enter the student details (Roll No, Name, Email, Course, Marks). The program will demonstrate the loading thread and display the calculated grade upon successful input.

***

| **Name** | Sanchit Yadav |
| **Roll Number** | 2401010162 |
