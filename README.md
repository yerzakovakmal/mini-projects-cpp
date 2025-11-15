# 📘 C++ Fundamental Projects Guide

This README contains step-by-step guides for four beginner-friendly C++ projects.  
Each project uses **fundamental C++ concepts**: variables, loops, conditionals, functions, arrays/vectors, structs/classes, and file I/O.

---

# 1️⃣ Student Management System

## 🎯 Goal
A console program to manage student records (ID, name, grades).  
Supports adding, listing, updating, deleting, and saving/loading data.

## 🧰 Concepts Used
- Variables & data types  
- Structs or classes  
- `std::vector`  
- Functions  
- Loops & conditionals  
- File I/O

## 🪜 Steps
1. Create a `Student` struct with: `id`, `name`, `vector<int> grades`.
2. Store students in a `vector<Student>`.
3. Create a menu with options:
   - Add student  
   - List students  
   - View student  
   - Update student  
   - Delete student  
   - Save to file  
   - Load from file
4. Write separate functions for each menu option.
5. Save data using a format like:  
   `id|name|grade1,grade2,grade3`
6. Load data by reading and splitting each line.
7. Validate input (unique ID, grade range).
8. Test all features.

---

# 2️⃣ Simple Banking App

## 🎯 Goal
A console banking system that lets users create accounts, deposit, withdraw, transfer money, and view history.

## 🧰 Concepts Used
- Classes & objects  
- Encapsulation  
- `std::vector`  
- Loops & conditionals  
- File I/O

## 🪜 Steps
1. Create an `Account` class with:
   - `id`, `owner`, `balance`  
   - `vector<string> history`
2. Add methods:
   - `deposit(amount)`  
   - `withdraw(amount)`  
   - `addHistory(text)`  
   - `printInfo()`
3. Store all accounts in a `vector<Account>`.
4. Create a menu:
   - Create account  
   - Deposit  
   - Withdraw  
   - Transfer  
   - Show balance  
   - Show history  
   - Save  
   - Load
5. Implement deposit/withdraw with balance checks.
6. Implement transfer between accounts.
7. Save accounts and history to a file.
8. Load them back into the program.
9. Test invalid inputs (negative amounts, missing accounts).

---

# 3️⃣ To-Do List CLI Program

## 🎯 Goal
A command-line program for managing to-do tasks (add, list, mark done, delete).

## 🧰 Concepts Used
- Structs  
- `std::vector`  
- Loops & conditionals  
- File I/O  
- Simple string parsing

## 🪜 Steps
1. Create a `Task` struct with:  
   `id`, `text`, `bool done`
2. Store tasks in a `vector<Task>`.
3. Create a menu:
   - Add task  
   - List tasks  
   - Mark done  
   - Delete task  
   - Save  
   - Load
4. Auto-increment task IDs.
5. Save tasks as:  
   `id|done|text`
6. Load by splitting each line.
7. Validate input (task ID must exist).
8. Test adding, marking, removing, saving, and loading.

---

# 4️⃣ Tic-Tac-Toe Game

## 🎯 Goal
A 3×3 Tic-Tac-Toe game in the console (Player X vs Player O).

## 🧰 Concepts Used
- Arrays or vectors  
- Functions  
- Loops & conditionals  
- Game logic (winner checking)

## 🪜 Steps
1. Create a 3×3 board using:  
   `char board[3][3]` or `vector<char> board(9)`
2. Write a function to print the board.
3. Write functions to check:
   - Winner  
   - Draw  
   - Valid move
4. Game loop:
   - Print board  
   - Ask current player for a move  
   - Validate input  
   - Update board  
   - Check win/draw  
5. Switch players every turn.
6. Print final result.
7. (Optional) Ask to play again.
8. Test all winning conditions and invalid moves.

---

# ✅ Final Notes
- Keep functions small and clear.  
- Validate all user input.  
- Compile with warnings enabled:  
  ```bash
  g++ main.cpp -o app -std=c++17 -Wall -Wextra
  ```
