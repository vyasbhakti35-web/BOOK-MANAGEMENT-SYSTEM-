# Software Requirements Specification (SRS)
## Project: Book Inventory Management System

### 1. Introduction
**Purpose:** This document describes the requirements for the Book Inventory Management System.  
**Scope:** The system allows users/admin to manage books using CRUD operations and store data in MongoDB.

### 2. Overall Description
**Target Users:** Bookstore owners, library staff, inventory managers.  
**User Goals:** Maintain accurate book records digitally.

### 3. System Features (Functional Requirements)
FR1. The system shall allow the user to add a new book (title, author, price, year).  
FR2. The system shall display a list of all books from the database.  
FR3. The system shall allow the user to update existing book details.  
FR4. The system shall allow the user to delete a book record.  
FR5. The system shall store all data persistently in MongoDB.

### 4. Non-Functional Requirements
NFR1. The UI shall be easy to use and responsive.  
NFR2. The server shall validate required inputs and return clear error messages.  
NFR3. The system shall respond within a reasonable time for normal operations.  
NFR4. The system shall maintain data consistency in MongoDB.

### 5. Constraints and Assumptions
- Requires Node.js and MongoDB.
- Internet connection is required if using MongoDB Atlas.
- Authentication is optional / future enhancement.

### 6. External Interface Requirements
**Frontend:** React + HTML/CSS/JS  
**Backend:** Node.js + Express   
**Database:** MongoDB (Mongoose)

### 7. Data Requirements
**Book fields:** title (required), author (required), price (required), publishedYear (optional), createdAt (auto)

### 8. API Requirements (Summary)
- GET /books
- POST /books
- PUT /books/:id
- DELETE /books/:id

### 9. Acceptance Criteria
- User can create, view, update, and delete a book successfully.
- Data persists after refresh/restart.
- Invalid input returns an error message.
