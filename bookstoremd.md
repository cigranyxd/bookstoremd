# Bookstore Management System

1. Introduction

The Bookstore Management System (BMS) is a web-based application designed to provide a
convenient and efficient platform for users to search for and purchase books online. It
facilitates both the user and the administrator, streamlining processes such as book inventory
management, order processing, and customer interactions. The system eliminates the need for
manual record-keeping, offering an automated and centralized platform to handle all
bookstore-related operations.

Project Background:
In traditional bookstores, managing inventory, sales, and customer data often requires
extensive manual effort. The use of spreadsheets and paper records can result in
inefficiencies, such as misplaced data, human error, and time-consuming tasks. This project
addresses these problems by digitizing the entire bookstore management process. By using the
BMS, administrators can easily add, remove, or update book records, while customers can
browse through categories, search for specific books, and complete orders online.

Objectives:

- Efficiency: To streamline bookstore operations, reducing the time and effort involved
    in managing book inventories and customer data.
- Automation: To minimize manual tasks, such as book categorization, sales tracking,
    and record maintenance, making the system more scalable.
- User-Friendly Interface: To provide a simple, intuitive interface for both the
    customers and administrators, ensuring ease of use and accessibility.
- Data Accuracy: To ensure data consistency and accuracy in book details, customer
    information, and order history, improving operational reliability.
- Scalability: To build a flexible system capable of handling increasing volumes of
    users and transactions as the bookstore grows.

Purpose of the Project:
The purpose of developing the BMS is to solve common problems related to manual
bookstore management. By transitioning from a paper-based system to a fully digital
environment, the BMS offers a solution to the tedious and error-prone manual processes. The
system allows admins to manage the bookstore from a single point, efficiently handling book
entries, categories, and customer orders. Additionally, it offers customers the convenience of
browsing and buying books from anywhere at any time, enhancing user experience.

Scope of the Project:
The BMS is designed for both small and large bookstores that require an efficient system to
manage book inventories and customer orders. The system can be extended in the future to
incorporate advanced features such as online payment, multiple language support, and
enhanced security measures. In its current form, the system focuses on core functionalities
such as book management, user authentication, shopping cart, and order processing.

Applicability:
This system is applicable to a variety of bookstores, whether physical stores transitioning to
digital or purely online bookstores. It allows customers to make purchases remotely, giving


bookstore owners a greater reach. The system can also be adapted to work for other
businesses that require inventory management, order processing, and customer interaction
platforms.

2. Requirement and Analysis

Problem Statement:
The current process of managing bookstores involves heavy reliance on paperwork and
manual entries. These processes are time-consuming, prone to human error, and inefficient
when dealing with large inventories and customer databases. Key problems include:

- Excessive paperwork that results in clutter and confusion.
- Time-consuming processes for managing book inventory and customer records.
- Limited scalability, making it hard to accommodate growing demand.
- Difficulty in tracking sales, generating reports, and managing customer data.
- Lack of an online platform where customers can browse and purchase books at their
    convenience.

System Requirements:
The system is divided into two primary modules: Admin and Client.

1. Admin Module: This module is designed for administrators who manage the
    bookstore’s backend operations. Its key functionalities include:
       o Adding and managing book categories.
       o Adding new books and updating existing ones.
       o Viewing customer messages and queries.
       o Managing customer data and processing orders.
2. Client Module: This module is designed for end-users or customers. Key
    functionalities include:
       o Viewing available books and categories.
       o Searching for specific books.
       o Adding selected books to the shopping cart.
       o Completing the order process through an easy-to-use interface.

Hardware Requirements:

- Operating System: Windows 7/8/10 or Linux (Ubuntu, CentOS).
- Processor: PC with Dual-core processor (2.20 GHz) or above.
- RAM: Minimum of 350 MB (512 MB recommended).
- Hard Disk Space: 45 MB available space or more on the system drive.

Software Requirements:

- Server Software: WAMP Server (or LAMP for Linux) to handle web hosting and
    database services.
- Database: MySQL for data storage, management, and retrieval.
- Browser: Any modern browser such as Mozilla Firefox, Google Chrome, or Microsoft
    Edge.
- Client-Side Tools: HTML, CSS, Bootstrap for front-end development; PHP for
    server-side scripting.


Planning and Scheduling:
The project follows a systematic planning and development cycle. The main phases and
timelines are as follows:


|Task Name| Duration| Start/End Date|
|-|-|-|
|Analysis| 8 Days|25/12/2018 - 01/01/|
|Design |9 Days |01/01/2019 - 09/01/|
|Coding |4 Weeks |10/01/2019 - 08/02/|
|Implementation |5 Days |08/02/2019 - 12/02/|
|Testing| 6 Days |12/02/2019 - 17/02/|
|Documentation |3 Weeks |18/02/2019 - 10/03/|

3. System Design

Overview:
The design phase is a critical part of the development process. It translates the project
requirements into a working model, allowing developers to visualize and plan the interaction
between the system components.

Data Flow Diagram (DFD): The DFD is used to represent the flow of data within the system.
In this project, we use both 0-level and 1st-level DFDs.

- 0 - Level DFD: This diagram provides an overview of the system. It represents the
    interactions between the admin, the customer, and the bookstore’s backend system.
- 1st-Level DFD: This diagram breaks down the components of the system, showing
    how customer orders are processed, how books are categorized, and how the admin
    manages the backend.

Entity-Relationship (ER) Diagram:
The ER diagram models the relationships between entities such as books, categories,
customers, and orders. It helps visualize how data is connected and ensures that all system
entities are properly mapped.

- Entities:
    o Books: Stores details such as book ID, name, price, category, description, and
       image.
    o Categories: Stores information about book categories.
    o Customers: Stores customer information such as name, address, and contact
       details.
    o Orders: Stores order information such as order ID, customer ID, and order
       details.

Database Structure: The database consists of several key tables, each representing a major
system entity. Some of the most important tables include:

- Admin Table: Stores admin login credentials.
- Books Table: Stores details about each book in the system.
- Category Table: Stores category names and IDs.


- Customer Table: Stores customer registration details.
- Orders Table: Stores details related to customer orders.
4. Testing and Implementation

Testing is an essential part of the system development lifecycle. It ensures that the system
functions as expected and identifies any bugs or issues that need to be resolved before
deployment.

Testing Approaches:

1. Black Box Testing:
    This approach focuses on testing the system's functionality without looking into the
    internal code structure. Testers provide input, check the output, and verify whether the
    system behaves as expected.
       o Test Case Example: Test user login functionality by providing valid and
          invalid credentials. Expected result: Successful login with correct credentials,
          error message for incorrect credentials.
2. White Box Testing:
    This approach involves testing the internal structure and logic of the system. It ensures
    that all internal paths, loops, and conditions are functioning correctly.
       o Test Case Example: Verify the correct implementation of loops in the book
          search functionality to ensure all books are correctly displayed.
3. Gray Box Testing:
    Gray box testing is a hybrid approach that tests the system from both an external and
    internal perspective. It combines the advantages of black-box and white-box testing to
    cover all critical aspects of the system.

Test Cases:

- Admin Login: Validate login functionality for the admin panel with various input
    combinations.
- Book Search: Test the accuracy and speed of the book search feature.
- Order Process: Ensure that the order processing workflow functions correctly from
    adding books to the cart to final order confirmation.

Implementation: The BMS was implemented using a combination of front-end and back-end
technologies. The front-end is built using HTML, CSS, and Bootstrap, providing a responsive
and user-friendly interface. The back-end, implemented in PHP, handles server-side
processing and communication with the MySQL database.

The implementation faced challenges, particularly in coordinating between the front-end and
back-end functionalities. The integration of database queries with the user interface required
careful planning to ensure data was properly displayed and managed.

5. Conclusion

The Bookstore Management System successfully streamlines bookstore operations by
providing an online platform for book management, customer interaction, and order


processing. While the system addresses many key problems related to manual operations, it
has some limitations that offer opportunities for future improvement.

Limitations:

- No Online Payment: Currently, the system does not support online payment
    processing. This feature could be added in future versions to enhance convenience for
    customers.
- Single-User Login: The system only allows one user to log in at a time. In the future,
    it could be improved to allow multiple concurrent users.
- No Multilingual Support: The system is designed only in English. Multilingual
    support could be added to expand its accessibility to a broader audience.

Future Scope:

- Help Module: A help module could be added to guide users in navigating the system
    and using its features.
- Payment Gateway Integration: Adding online payment options, such as credit card
    payments or integration with payment platforms like PayPal, will enhance the
    system’s functionality.
- Multilingual Support: Supporting multiple languages will allow the system to serve a
    more diverse user base.


###### This was edited by Boogdán Botond, and Orosz Dániel

