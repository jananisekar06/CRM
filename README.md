# 🚀 CRM Management System

A full-stack **Customer Relationship Management (CRM) System** built using **React, Node.js, Express.js, and PostgreSQL**.

This CRM application provides role-based access and multiple business management modules such as Customers, Leads, Sales, Tasks, Employees, Attendance, Leave, Payroll, Invoices, Payments, Reports, AI Assistant, Notifications, Email, WhatsApp and more.

---

## 📌 Project Overview

The CRM Management System is designed to manage customer relationships, sales activities, employee operations, business communication, and administrative processes from a single platform.

The system uses:

* **React + Vite** for the frontend
* **Node.js + Express.js** for the backend
* **PostgreSQL** for database management
* **JWT** for authentication
* **bcrypt** for password hashing
* **Axios** for API communication
* **Tailwind CSS** for UI styling

---

## ✨ Features

### 🔐 Authentication

* User Registration
* User Login
* JWT Authentication
* Password Hashing
* Forgot Password
* Reset Password
* Protected Routes

### 👥 Customer Management

* Add Customers
* Update Customer Details
* Delete Customers
* View Customer Information
* Customer Experience Management
* Customer Portal

### 🎯 Lead Management

* Create Leads
* Assign Leads
* Lead Status Management
* Track Lead Progress
* Convert Leads into Customers

### 💼 Sales Management

* Sales Pipeline
* Deal Management
* Follow-up Management
* Meeting Scheduler
* Sales Tracking

### 📋 Task Management

* Create Tasks
* Assign Tasks
* Update Task Status
* Track Pending and Completed Tasks

### 👨‍💼 Employee Management

* Employee Management
* Attendance
* Leave Management
* Payroll Management
* Employee Profiles

### 💰 Finance

* Invoice Management
* Payment Management
* Finance Management
* Revenue Tracking

### 🎫 Support

* Ticket Management
* Customer Support
* Communication Management
* Notifications

### 🤖 AI Features

* AI Assistant
* AI Chatbot
* Analytics
* Reports

### 📢 Communication

* Email Management
* WhatsApp Integration
* Notifications
* Collaboration

### 📦 Business Management

* Inventory Management
* Vendor Management
* Campaign Management
* Subscription Management
* Multi-Company Management
* Multi-Language Support

### ⚙️ Administration

* Role-Based Access Control
* Super Admin Panel
* Settings
* Activity Logs
* Audit Logs
* Backup & Restore
* File Upload

---

## 👤 User Roles

The system supports role-based access for:

* **Super Admin**
* **Admin**
* **Sales Manager**
* **Sales Executive**
* **HR**
* **Support**
* **Customer**

Each role can access different modules according to the assigned permissions.

---

## 🛠️ Technologies Used

### Frontend

* React
* Vite
* Tailwind CSS
* React Router
* Axios
* React Icons
* Chart.js
* jsPDF
* XLSX

### Backend

* Node.js
* Express.js
* PostgreSQL
* JWT
* bcrypt
* Multer
* Nodemailer
* CORS
* dotenv

### Database

* PostgreSQL
* SQL
* JSONB

---

## 📂 Project Structure

```text
CRM-postgresql-role-based/
│
├── crm-frontend/
│   ├── src/
│   │   ├── components/
│   │   │   ├── Navbar.jsx
│   │   │   ├── Sidebar.jsx
│   │   │   └── ProtectedRoute.jsx
│   │   │
│   │   ├── pages/
│   │   │   ├── Login.jsx
│   │   │   ├── Dashboard.jsx
│   │   │   ├── Customers.jsx
│   │   │   ├── Leads.jsx
│   │   │   ├── Sales.jsx
│   │   │   ├── Tasks.jsx
│   │   │   ├── Employees.jsx
│   │   │   ├── Attendance.jsx
│   │   │   ├── Leave.jsx
│   │   │   ├── Payroll.jsx
│   │   │   ├── Invoice.jsx
│   │   │   ├── Payments.jsx
│   │   │   ├── Reports.jsx
│   │   │   ├── Analytics.jsx
│   │   │   ├── AI Assistant
│   │   │   ├── AI Chatbot
│   │   │   └── ...other modules
│   │   │
│   │   ├── config/
│   │   ├── App.jsx
│   │   ├── main.jsx
│   │   └── index.css
│   │
│   └── package.json
│
├── crm-backend/
│   ├── controllers/
│   ├── routes/
│   ├── middleware/
│   ├── config/
│   ├── db/
│   │   ├── schema.sql
│   │   ├── setup.js
│   │   └── seed.js
│   ├── uploads/
│   ├── server.js
│   ├── .env
│   └── package.json
│
└── README.md
```

---

## ⚙️ Installation & Setup

### 1. Clone the Repository

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
```

```bash
cd CRM-postgresql-role-based
```

---

## 🗄️ PostgreSQL Setup

Install PostgreSQL on your system.

Create the CRM database:

```sql
CREATE DATABASE crm_db;
```

Then configure the backend `.env` file:

```env
PORT=5000

JWT_SECRET=crm_secret_key

DB_HOST=localhost
DB_PORT=5432
DB_USER=postgres
DB_PASSWORD=your_postgresql_password
DB_NAME=crm_db
```

Replace `your_postgresql_password` with your PostgreSQL password.

---

## 🔧 Backend Setup

Open a terminal:

```bash
cd crm-backend
```

Install dependencies:

```bash
npm install
```

Create database tables:

```bash
npm run db:setup
```

Insert sample/demo data:

```bash
npm run db:seed
```

Start the backend:

```bash
npm run dev
```

Backend will run on:

```text
http://localhost:5000
```

---

## 💻 Frontend Setup

Open another terminal:

```bash
cd crm-frontend
```

Install dependencies:

```bash
npm install
```

Start the development server:

```bash
npm run dev
```

Frontend will run on:

```text
http://localhost:5173
```

---

## 🔑 Demo Login

After running the database seed:

```text
Email: admin@gmail.com
Password: 123456
```

> For production use, change the default credentials and configure secure environment variables.

---

## 🔄 Application Flow

```text
User Login
    ↓
JWT Authentication
    ↓
Role & Permission Validation
    ↓
Dashboard
    ↓
CRM Modules
    ↓
React Frontend
    ↓
Axios API Requests
    ↓
Node.js + Express Backend
    ↓
PostgreSQL Database
```

---

## 🗃️ Database

The application uses **PostgreSQL** as the primary database.

The database contains tables for different CRM modules including:

* Users
* Customers
* Leads
* Contacts
* Sales
* Tasks
* Meetings
* Follow-ups
* Employees
* Attendance
* Leave
* Payroll
* Tickets
* Invoices
* Payments
* Reports
* Notifications
* Inventory
* Vendors
* Campaigns
* Subscriptions
* Activity Logs
* Audit Logs
* And other CRM modules

---

## 🔒 Security

The application includes:

* JWT-based authentication
* Password hashing using bcrypt
* Role-based permissions
* Protected frontend routes
* Environment variable configuration
* Backend API validation
* Activity and audit logging

---

## 📊 Dashboard

The CRM dashboard provides important business information such as:

* Total Customers
* Total Leads
* Today's Meetings
* Pending Tasks
* Revenue
* New Tickets
* Employee Attendance
* Monthly Sales
* Analytics

---

## 🧪 Testing

To verify the application:

1. Start PostgreSQL.
2. Start the backend.
3. Start the frontend.
4. Login using the demo credentials.
5. Create a customer or lead.
6. Refresh the page.
7. Verify that the data remains stored in PostgreSQL.

---

## 🚀 Production Deployment

The application can be deployed using platforms such as:

### Frontend

* Vercel
* Netlify

### Backend

* Render
* Railway

### Database

* PostgreSQL hosting providers

Before deployment:

* Update database credentials
* Configure production environment variables
* Change JWT secret
* Remove default admin credentials
* Configure frontend/backend API URLs
* Enable appropriate CORS settings

---

## 📌 Important Notes

* Do not upload `.env` files containing passwords or secrets to GitHub.
* Add `.env` to `.gitignore`.
* Use strong passwords in production.
* Change the default admin password after setup.

---

## 👩‍💻 Project

**CRM Management System**

**Frontend:** React + Vite + Tailwind CSS
**Backend:** Node.js + Express.js
**Database:** PostgreSQL

---

## 📄 License

This project is developed for learning, development, and business application purposes.
