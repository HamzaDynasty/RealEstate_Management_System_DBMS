# 🏠 Real Estate Management System (REMS)

A modern full-stack Real Estate Management System designed to digitize and automate the complete workflow of a real estate agency. The system provides centralized management for properties, agents, clients, listings, inspections, contracts, transactions, and financial records through a secure and responsive web platform.

---

# ✨ Project Overview

The Real Estate Management System (REMS) is a database-driven web application that streamlines real estate operations by replacing traditional manual processes with a centralized digital solution.

The platform supports:
- Property management
- Client and agent management
- Property listings
- Inspection scheduling
- Transaction tracking
- Payment management
- Commission calculations
- Feedback and rating systems

The system is designed with scalability, security, and performance in mind, making it suitable for both academic and real-world implementations.

---

# 🛠️ Technology Stack

## 🔹 Backend
The backend is developed using:

- **Node.js**
- **Express.js**

These technologies handle:
- REST API routes
- Middleware processing
- Authentication
- Database communication
- Business logic

---

## 🔹 Database
The system uses:

- **MySQL**
- **MySQL2 Driver**

The relational database stores all structured data securely and efficiently.

---

## 🔹 Frontend
The frontend interface is built using:

- HTML5
- CSS3
- Vanilla JavaScript
- Bootstrap

This creates a clean, responsive, and interactive user experience without relying on heavy frontend frameworks.

---

## 🔹 Security Features

The application implements industry-standard security practices:

- 🔐 **JWT Authentication**
  - Secure user sessions
  - Protected routes
  - Role-based authorization

- 🔒 **Bcrypt.js**
  - Password hashing
  - Secure credential storage

---

# 👥 Role-Based Access Control (RBAC)

The system contains three separate user roles with different permissions and workflows.

---

## 🏢 Admin (Agency)

The Admin acts as the superuser and has complete system access.

### Admin Features
- Manage agents
- Manage clients
- Manage property listings
- Track transactions
- Monitor payments
- View global statistics
- Analyze agent performance
- Manage contracts and inspections

---

## 🧑‍💼 Agent

Agents manage real estate operations assigned to them.

### Agent Features
- Add and manage listings
- Schedule inspections
- View assigned properties
- Track commissions
- Monitor sales and rentals
- Update listing statuses

---

## 🧑 Client (Buyer / Seller / Renter)

Clients interact with the platform to explore and request properties.

### Client Features
- Browse properties
- Request inspections
- View listing details
- Submit feedback and ratings
- Track transactions

---

# 🗄️ Database Design

The database schema is fully normalized and designed for maximum efficiency and data integrity.

---

## 📌 Core Entities

The system includes the following major entities:

1. Agency  
2. Agent  
3. Client  
4. Property  
5. Property_Type  
6. Location  
7. Listing  
8. Transaction  
9. Payment  
10. Contract  
11. Inspection  
12. Feedback  

---

# 📊 Database Normalization

The database follows the **Third Normal Form (3NF)**.

### ✅ 1NF
- Removed repeating groups
- Ensured atomic values

### ✅ 2NF
- Eliminated partial dependencies

### ✅ 3NF
- Removed transitive dependencies
- Improved consistency and integrity

This normalization reduces redundancy and improves query performance.

---

# ⚙️ Core Business Functionality

The application handles the complete property lifecycle.

---

## 🏡 Property Management
- Add new properties
- Assign property types
- Manage listing status
- Update property availability

---

## 📅 Inspection Management
Clients can request property inspections.

The system tracks:
- Inspection dates
- Time slots
- Approval status
- Assigned agents

---

## 💰 Financial Management

The system records and manages:

- Sales transactions
- Rental transactions
- Payment history
- Payment methods
- Payment statuses
- Agent commissions

Commission calculations are automatically processed based on completed transactions.

---

## ⭐ Feedback System

Clients can provide:
- Ratings
- Reviews
- Feedback comments

This improves transparency and service quality.

---

# 🚀 Setup and Deployment

The project includes automation scripts for quick setup and deployment.

---

## 📂 Setup Scripts

### 🔹 setup-database.bat
Initializes:
- MySQL database
- Tables
- Schema
- Relationships

---

### 🔹 add-sample-data.bat
Populates the database with:
- Sample agents
- Clients
- Listings
- Transactions
- Demo records

---

### 🔹 start-project.bat
Automatically starts:
- Node.js backend server
- Frontend client

---

# ▶️ How to Run the Project

## Step 1 — Install Dependencies

```bash
npm install
