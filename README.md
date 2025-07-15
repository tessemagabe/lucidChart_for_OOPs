<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Library Management System - README</title>
    <style>
        body {
            font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol";
            line-height: 1.6;
            color: #24292e;
            max-width: 900px;
            margin: 20px auto;
            padding: 0 20px;
            background-color: #f6f8fa;
        }
        h1, h2, h3 {
            border-bottom: 1px solid #eaecef;
            padding-bottom: 0.3em;
            margin-top: 24px;
            margin-bottom: 16px;
            font-weight: 600;
            line-height: 1.25;
        }
        h1 { font-size: 2em; }
        h2 { font-size: 1.5em; }
        h3 { font-size: 1.25em; }
        img {
            max-width: 100%;
            height: auto;
            display: block;
            margin: 20px 0;
            border: 1px solid #eaecef;
            box-shadow: 0 1px 3px rgba(27,31,35,.075);
        }
        p {
            margin-bottom: 16px;
        }
        ul {
            list-style-type: disc;
            margin-left: 20px;
            margin-bottom: 16px;
        }
        code {
            font-family: SFMono-Regular, Consolas, "Liberation Mono", Menlo, Courier, monospace;
            background-color: rgba(27,31,35,.05);
            border-radius: 3px;
            padding: 0.2em 0.4em;
        }
        pre {
            background-color: rgba(27,31,35,.05);
            border-radius: 3px;
            padding: 16px;
            overflow: auto;
        }
    </style>
</head>
<body>

    <h1>Library Management System</h1>

    <p>This repository contains the design and process flows for a Library Management System, visualized using Lucidchart. The aim of this system is to streamline the core operations of a library, including book management, member services, and the search/borrowing workflow.</p>

    <h2>Overview</h2>

    <p>The Library Management System is designed to provide efficient interfaces for both library staff (Librarian) and library users (Member). The system facilitates:</p>
    <ul>
        <li><strong>User Authentication:</strong> Secure login for both librarians and members.</li>
        <li><strong>Core Library Operations:</strong> Managing books, members, and book issuance.</li>
        <li><strong>Member Services:</strong> Accessing account details, searching for books, and managing borrowing.</li>
    </ul>

    <h2>Process Flow Diagrams</h2>

    <p>The following flowcharts detail the key processes within the Library Management System:</p>

    <h3>1. Main System Flow</h3>

    <p>This flowchart provides a high-level overview of the entire Library Management System, illustrating the initial entry points for both librarians and members, and their respective primary functionalities.</p>

    <img src="image_fa38da.png" alt="Main Library Management System Flowchart">

    <ul>
        <li><strong>Key Paths:</strong>
            <ul>
                <li><strong>Librarian Path:</strong> Login, then access to 'Manage Books' and 'Manage Members', and the ability to 'Issue Books' after checking availability and notifying the user.</li>
                <li><strong>Member Path:</strong> Login, then access to 'My Account' and 'Search' functionalities.</li>
            </ul>
        </li>
    </ul>

    <h3>2. Manage Books Workflow</h3>

    <p>This detailed flowchart illustrates the process for managing books within the system, focusing on inventory updates and ordering.</p>

    <img src="image_fa3c22.png" alt="Manage Books Flowchart">

    <ul>
        <li><strong>Key Processes:</strong>
            <ul>
                <li>Initiates from a successful login.</li>
                <li>Allows librarians to 'Search for books' and check 'Book available?'.</li>
                <li>If a book is not available, it can be 'Add Book'.</li>
                <li>'Update Transaction' and 'Update' steps are included.</li>
                <li>Includes a 'Check for Low Stock' decision, leading to 'Order Books' or 'Stock Updated' pathways.</li>
                <li>Concludes with 'Logout'.</li>
            </ul>
        </li>
    </ul>

    <h3>3. Search-Borrow Workflow</h3>

    <p>This flowchart details the process a member undergoes to search for and borrow a book, including scenarios for book unavailability and inter-branch transfers.</p>

    <img src="image_fa3be0.png" alt="Search-Borrow Workflow Flowchart">

    <ul>
        <li><strong>Key Processes:</strong>
            <ul>
                <li>Starts with a successful login, leading to 'Access Library System' and 'My Account' or 'Search for Book'.</li>
                <li>Includes a 'Book Available?' decision.</li>
                <li>If a book is not available, the system checks 'Available at Other Branch?', with options to 'Notify User of Unavailability' or 'Request Inter-Branch Transfer'.</li>
                <li>Successfully available books proceed to 'Borrow Book', 'Confirm Borrowing Details', and 'Complete Borrowing Procedure'.</li>
                <li>Ends with 'Logout'.</li>
            </ul>
        </li>
    </ul>

</body>
</html>
