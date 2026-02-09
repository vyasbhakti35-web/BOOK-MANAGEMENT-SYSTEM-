# Test Cases – Book Inventory Management System

## Test Case 1: Add Book (Valid)
**Steps:**
1. Open the app.
2. Fill Title, Author, Price (and Year if available).
3. Click Add/Submit.
**Expected Result:** Book appears in the list and is saved in MongoDB.

## Test Case 2: Add Book (Missing Required Field)
**Steps:**
1. Leave Title empty.
2. Click Add/Submit.
**Expected Result:** Error message shown and book is not saved.

## Test Case 3: View Books
**Steps:**
1. Open the app or refresh the page.
**Expected Result:** All books load from database and display correctly.

## Test Case 4: Update Book
**Steps:**
1. Click Edit on a book.
2. Change Price or Title.
3. Save.
**Expected Result:** Updated values display and persist in database.

## Test Case 5: Delete Book
**Steps:**
1. Click Delete on a book.
2. Confirm (if prompt exists).
**Expected Result:** Book is removed from UI and deleted from MongoDB.

## Test Case 6: Persistence Check
**Steps:**
1. Add a book.
2. Refresh page / restart server.
**Expected Result:** Book still exists (data persisted).
