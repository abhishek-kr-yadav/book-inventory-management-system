# BookVault - Book Inventory Management System (NoSQL Project)

A Book Inventory Management System built using **MongoDB**, demonstrating practical implementation of NoSQL database operations for storing, managing, searching, and organizing book information[cite: 2, 3]. 

Developed as part of the BCA (Data Science & AI) curriculum at BBD University[cite: 2].

---

## 📌 Project Overview
**BookVault** uses a MongoDB database named `library` containing a collection called `books` with 30 book records[cite: 3]. Each record includes details such as:
* `bookId`[cite: 2, 16]
* `title`[cite: 2, 16]
* `author`[cite: 2, 16]
* `category`[cite: 2, 16]
* `price`[cite: 2, 16]
* `year` (Publication Year)[cite: 2, 16]
* `rating`[cite: 2, 16]

---

## 🛠️ MongoDB Operations Implemented
This project covers a wide range of MongoDB queries and aggregation pipelines:

1. **Database & Collection Management**[cite: 4, 27]
   * `use library` – Switch to or create the database[cite: 4, 27].
   * `db.createCollection("books")` – Create the books collection[cite: 4, 27].

2. **Data Insertion**[cite: 16, 27]
   * `db.books.insertMany([...])` – Insert multiple book documents simultaneously[cite: 16, 27].

3. **Retrieval & Projection**[cite: 17, 18, 27]
   * `db.books.find()` – Retrieve all book records[cite: 17, 27].
   * **Projection:** Display specific fields (e.g., showing only titles and authors)[cite: 18, 27].

4. **Filtering & Comparison Operators**[cite: 19, 20, 21, 27]
   * Filter by category (e.g., "Fantasy")[cite: 19, 27].
   * Filter using comparison operators like `$gt`, `$lt`, `$gte`, and `$lte` (e.g., ratings above 8, prices below ₹400, publication years between 2000 and 2020)[cite: 19, 20, 21, 27].

5. **Sorting & Limiting Results**[cite: 22, 23, 27]
   * `sort({ price: -1 })` – Sort books from most expensive to least expensive[cite: 22, 27].
   * `.limit(5)` – Retrieve top-rated results (e.g., top 5 highest-rated books)[cite: 23, 27].

6. **Data Updates**[cite: 25, 27]
   * `db.books.updateOne()` – Modify specific document properties (e.g., updating a book's price)[cite: 25, 27].

7. **Aggregation Framework**[cite: 26, 27]
   * `db.books.aggregate([...])` – Utilize stages like `$_id` grouping (`$group`), counting (`$sum`), and sorting to analyze the total number of books available in each category[cite: 26, 27].

---

## 🚀 Getting Started

To run these queries locally:
1. Ensure you have **MongoDB** and **MongoDB Compass** or `mongosh` installed[cite: 4].
2. Open your MongoDB shell or Compass terminal[cite: 4].
3. Copy and execute the queries provided in the project documentation to recreate the database, collection, and test records[cite: 4].

---

## 📝 Author
* **Abhishek Kr. Yadav** (Roll No: `1250258019`)[cite: 2]
* **Department:** BCA (Data Science & AI)[cite: 2]
* **Institution:** BBD University (School of Computer Application)[cite: 2]
* **Submitted To:** Mr. Harendra Singh[cite: 2]
