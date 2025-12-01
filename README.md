# 🏢 StaffSync

**StaffSync** is a robust **Employee Management System** architected using **Java Swing** and **MySQL**.
It is designed to streamline human resource operations, facilitating efficient **workforce administration, payroll processing, and attendance tracking**.
The application bridges the gap between management and staff, offering a secure, intuitive interface for data-driven decision-making and organizational transparency.

## 🌟 Key Features

### 👤 Employee Portal

* **Self-Service Dashboard** – View personal employment details and job status.
* **Leave Management** – Submit leave requests and track approval status in real-time.
* **Salary Insights** – Access monthly salary slips and payment history.
* **Attendance Logs** – Review daily clock-in/clock-out records and total work hours.
* **Profile Maintenance** – Update contact details and educational qualifications.
* **Secure Authentication** – Encrypted login for data privacy.

### 🛠️ Administrative Suite

* **Workforce Oversight** – Onboard new hires and manage existing employee records.
* **Payroll Administration** – Automate salary calculations based on attendance and grade.
* **Attendance Monitoring** – Track daily presence and identify absenteeism trends.
* **Leave Arbitration** – Review, approve, or reject employee leave applications.
* **Record Retrieval** – Advanced search functionality to locate personnel by ID or Department.
* **System Configuration** – Manage department structures and job roles.

## 🖥️ Technology Stack

* **Frontend/UI:** Java Swing (AWT/Swing Components)
* **Backend Logic:** Core Java (OOP Principles)
* **Database:** MySQL (Relational Data Management)
* **Connectivity:** JDBC (Java Database Connectivity)
* **IDE:** IntelliJ IDEA / Eclipse

## 🚀 Installation & Setup

### Prerequisites

* **Java Development Kit (JDK) 8+**
* **MySQL Server 8.0+**
* **IDE:** IntelliJ IDEA / VS Code / Eclipse

### Steps

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/](https://github.com/)[YourUsername]/StaffSync.git
    ```

2.  **Import project** into your preferred Java IDE.

3.  **Configure the Database:**
    * Open your MySQL Command Line or Workbench.
    * Create the database: `CREATE DATABASE EMPLOYEEDB;`

4.  **Initialize Schema:**
    * Run the provided SQL script located in `src/database/schema.sql` to create necessary tables.

5.  **Update Configuration:**
    * Navigate to `src/Conn.java`.
    * Update the database credentials:
        ```java
        c = DriverManager.getConnection("jdbc:mysql:///EMPLOYEEDB", "root", "YOUR_PASSWORD");
        ```

6.  **Launch Application:**
    * Run `Splash.java` to start the application.

## 📂 Database Structure

* **LOGIN** → Stores admin credentials and access levels.
* **EMPLOYEE** → Primary repository for personnel data (ID, Name, Role, Education, Contact).
* **ATTENDANCE** → Tracks daily work logs mapped to Employee IDs.
* **LEAVE_REQUESTS** → Manages leave applications, dates, and approval states.
* **SALARY** → Stores compensation data, tax deductions, and net pay calculations.

## 🔮 Future Roadmap

* **PDF Report Generation** (Salary Slips & Certificates)
* **Biometric Integration** for automated attendance
* **Dark Mode UI** for better accessibility
* **Data Analytics Dashboard** (Visual charts for attrition and performance)

## 👨‍💻 Author

**[Your Name]**
