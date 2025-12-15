🏠 Real Estate Management System (REMS) Full Description
The Real Estate Management System (REMS) is a comprehensive, web-based database management project designed to fully digitize the operations of a real estate agency. It streamlines the management of properties, agents, clients, and financial transactions through a centralized platform.


I. Technology Stack and Architecture
The system employs a full-stack architecture built for efficiency and security:
Backend: Leverages the Node.js runtime environment and the flexible Express.js web application framework for handling API routes and middleware.
Database: Uses MySQL as the Relational Database Management System (RDBMS) for storing structured data, accessed via the MySQL2 Client driver.
Frontend: Built with HTML5, CSS3, Vanilla JavaScript, and Bootstrap to provide a responsive, dynamic user interface without heavy frameworks.
Security: Implements JSON Web Tokens (JWT) to securely manage user sessions and authorization, and Bcrypt.js for hashing passwords to ensure data security.

II. Role-Based Access Control (RBAC)
The system logic is divided into three distinct user flows based on roles, ensuring appropriate access to features and data:
Admin (Agency): The superuser with full control. Can manage agents, properties, listings, transactions, and view global statistics like Total Sales and Agent Performance.
Agent: Represents agency employees. They manage their specific listings, schedule inspections, and track their sales and commissions.
Client (Buyer/Seller/Renter): The end-users who can browse listings, request inspections, and provide feedback on properties and agents.


III. Database Design (RDM and Normalization)
The database schema is meticulously designed and normalized to ensure high data integrity and efficiency.
Key Entities: The system utilizes 12 key entities: Agency, Agent, Client, Property, Property_Type, Location, Listing, Transaction, Payment, Contract, Inspection, and Feedback .
Normalization: The data model is fully normalized to the Third Normal Form (3NF). This process eliminated issues like repeating groups (1NF), partial dependencies (2NF), and transitive dependencies (3NF).



IV. Core Business Functionality
The application manages the entire property lifecycle and associated business operations:
Property Lifecycle: Tracks properties from acquisition, listing (with status), inspection requests, to transaction completion.
Financial Management: Records every Transaction (sale/rent), automatically calculates agent Commissions, and tracks individual Payments (amount, method, status) linked to transactions.
Operational Tracking: Manages client-booked Inspections (date, time, status) and records client Feedback (rating, comment).

V. Implementation and Setup
The project includes automation scripts for easy deployment:
setup-database.bat: Initializes the MySQL database and schema.
add-sample-data.bat: Populates the database with seed data for testing.
start-project.bat: Launches the Node.js server and client simultaneously.
