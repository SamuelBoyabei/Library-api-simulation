README

Library Management API Simulation

Project Description

This project is a simulation of a simple Library Management API developed using Python and asynchronous programming techniques. The system demonstrates how an Application Programming Interface (API) can be used to manage common library operations such as viewing available books, borrowing books, and returning borrowed books.

The project does not require a web server or database. Instead, it uses Python classes and asynchronous functions to simulate API behavior in a simple and understandable manner.

---

Features

- View all books available in the library
- Borrow a book using its ID
- Return a borrowed book
- Check book availability status
- Simulate multiple users accessing the system simultaneously
- Demonstrate asynchronous programming using "asyncio"

---

Technologies Used

- Python 3
- Object-Oriented Programming (OOP)
- Asyncio Library
- Type Annotations

---

API Endpoints Simulated

1. Get Books

Method: GET

Function: "get_books()"

Purpose:
Returns a list of all books stored in the library system together with their availability status.

---

2. Borrow Book

Method: POST

Function: "borrow_book(book_id)"

Purpose:
Allows a user to borrow a book by providing the book ID. The system verifies whether the book is available before processing the request.

---

3. Return Book

Method: POST

Function: "return_book(book_id)"

Purpose:
Allows users to return previously borrowed books and updates the availability status accordingly.

---

How the System Works

The system stores book information in a list of dictionaries. Each dictionary contains:

- Book ID
- Book Title
- Availability Status

When a user borrows a book, the availability status changes from "True" to "False".

When a user returns a book, the availability status changes from "False" to "True".

The system uses asynchronous programming to simulate multiple users interacting with the API simultaneously.

---

Running the Program

1. Open the project in Visual Studio Code.
2. Ensure Python 3 is installed.
3. Save the source code as "library_api.py".
4. Open the terminal.
5. Run the command:

python library_api.py

6. The program will display the results of multiple simulated user requests.

---

Sample Output

===== SIMULATING MULTIPLE USERS =====

[API] Fetching all books...
[API] Borrowing book ID 2...
[API] Borrowing book ID 3...
[API] Returning book ID 2...

[
 {'id': 1, 'title': 'Introduction to Programming', 'available': True},
 {'id': 2, 'title': 'Computer Networks', 'available': False},
 {'id': 3, 'title': 'Data Structures and Algorithms', 'available': False},
 {'id': 4, 'title': 'Software Engineering', 'available': True},
 {'id': 5, 'title': 'Artificial Intelligence', 'available': True}
]

{'message': 'Book borrowed successfully'}
{'message': 'Book borrowed successfully'}
{'message': 'Book returned successfully'}

---

Future Improvements

- User Authentication System
- Book Search Functionality
- Due Date Tracking
- Fine Calculation for Late Returns
- Database Integration
- Web-Based API using FastAPI or Flask

---

