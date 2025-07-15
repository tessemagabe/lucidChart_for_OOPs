# Library Management System

This repository contains the design and process flows for a Library Management System, visualized using Lucidchart. The aim of this system is to streamline the core operations of a library, including book management, member services, and the search/borrowing workflow.

## Overview

The Library Management System is designed to provide efficient interfaces for both library staff (Librarian) and library users (Member). The system facilitates:

* **User Authentication:** Secure login for both librarians and members.
* **Core Library Operations:** Managing books, members, and book issuance.
* **Member Services:** Accessing account details, searching for books, and managing borrowing.

## Process Flow Diagrams

The following flowcharts detail the key processes within the Library Management System:

### 1. Main System Flow

This flowchart provides a high-level overview of the entire Library Management System, illustrating the initial entry points for both librarians and members, and their respective primary functionalities.

<img src="image_fa38da.png" alt="Main Library Management System Flowchart" style="max-width: 100%; height: auto; display: block; margin: 20px 0; border: 1px solid #eaecef; box-shadow: 0 1px 3px rgba(27,31,35,.075);">

* **Key Paths:**
    * **Librarian Path:** Login, then access to 'Manage Books' and 'Manage Members', and the ability to 'Issue Books' after checking availability and notifying the user.
    * **Member Path:** Login, then access to 'My Account' and 'Search' functionalities.

### 2. Manage Books Workflow

This detailed flowchart illustrates the process for managing books within the system, focusing on inventory updates and ordering.

<img src="image_fa3c22.png" alt="Manage Books Flowchart" style="max-width: 100%; height: auto; display: block; margin: 20px 0; border: 1px solid #eaecef; box-shadow: 0 1px 3px rgba(27,31,35,.075);">

* **Key Processes:**
    * Initiates from a successful login.
    * Allows librarians to 'Search for books' and check 'Book available?'.
    * If a book is not available, it can be 'Add Book'.
    * 'Update Transaction' and 'Update' steps are included.
    * Includes a 'Check for Low Stock' decision, leading to 'Order Books' or 'Stock Updated' pathways.
    * Concludes with 'Logout'.

### 3. Search-Borrow Workflow

This flowchart details the process a member undergoes to search for and borrow a book, including scenarios for book unavailability and inter-branch transfers.

<img src="image_fa3be0.png" alt="Search-Borrow Workflow Flowchart" style="max-width: 100%; height: auto; display: block; margin: 20px 0; border: 1px solid #eaecef; box-shadow: 0 1px 3px rgba(27,31,35,.075);">

* **Key Processes:**
    * Starts with a successful login, leading to 'Access Library System' and 'My Account' or 'Search for Book'.
    * Includes a 'Book Available?' decision.
    * If a book is not available, the system checks 'Available at Other Branch?', with options to 'Notify User of Unavailability' or 'Request Inter-Branch Transfer'.
    * Successfully available books proceed to 'Borrow Book', 'Confirm Borrowing Details', and 'Complete Borrowing Procedure'.
    * Ends with 'Logout'.
