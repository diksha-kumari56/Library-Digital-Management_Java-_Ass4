# 📚 City Library Digital Management System

A Java-based **console application** for managing books, members, issuing and returning books, and storing data persistently using files.

This system uses **OOP concepts**, **Collections Framework**, **File Handling**, and **Comparable & Comparator** for sorting.

---

## ✨ Features

### 🟦 **Book Management**

* Add new books
* Store details: ID, title, author, category
* Mark books as issued / returned
* View sorted books (by Title or Author)
* Search books by:

  * Title
  * Author
  * Category

### 🟩 **Member Management**

* Add new members
* Store member details: ID, name, email
* Track list of issued book IDs

### 🟨 **Issue & Return**

* Issue a book to a member
* Return a book
* Prevent issuing already issued books
* Automatically update member’s issued book list


## 🧠 Technologies Used

* Java
* Collections (Map, List, Set, Comparator, Comparable)
* File Handling (BufferedReader, BufferedWriter)
* Exception Handling
* OOP Concepts

---

## 📁 Project Structure

```
LibraryManager
│
├── Book.java
├── Member.java
└── LibraryManager.java  (Main Class)
```

* **Book Class** → Represents a book, implements `Comparable`
* **Member Class** → Stores member data + issued books
* **LibraryManager** → Handles menu, operations, file handling

---

## 📦 Data Storage Format

### books.txt

```
bookId,title,author,category,isIssued
```

### members.txt

```
memberId,name,email,bookId1;bookId2;bookId3;
```

---

## ▶️ How to Run

1. Save all classes in a single file named

   ```
   LibraryManager.java
   ```
2. Compile the program

   ```
   javac LibraryManager.java
   ```
3. Run

   ```
   java LibraryManager
   ```

---

## 🖥️ Menu Options

```
===== City Library Digital Management System =====
1. Add Book
2. Add Member
3. Issue Book
4. Return Book
5. Search Books
6. Sort Books
7. Exit
```

---

## 🔍 Sample Outputs

### Adding a Book

```
Enter Book ID: 101
Enter Title: Java Programming
Enter Author: James Gosling
Enter Category: Programming
Book added successfully!
```

### Issuing a Book

```
Enter Book ID: 101
Enter Member ID: 10
Book issued successfully!
```

### Searching

```
Enter search keyword: java
Book ID: 101
Title: Java Programming
Author: James Gosling
Category: Programming
Issued: Yes
```

---
