# 🗓️ Java Swing Appointment System

A desktop-based Java application with a modern dark-themed GUI, built using Swing and MySQL. This app supports user authentication, resource management, and appointment booking — ideal for admin-controlled environments like clinics, service centers, or labs.

---

## 📋 Table of Contents

* [Overview](#overview)
* [Features](#features)
* [Screenshots](#screenshots)
* [Technologies Used](#technologies-used)
* [Prerequisites](#prerequisites)
* [Installation](#installation)
* [Usage](#usage)
* [Database Configuration](#database-configuration)
* [Project Structure](#project-structure)
* [Troubleshooting](#troubleshooting)
* [License](#license)
* [Contact](#contact)

---

## 🔍 Overview

This Java Swing application offers:

* A secure **login system**
* Admin panel for **resource & appointment management**
* User panel to **view and book time slots**
* **MySQL** as the backend for persistent data
* Smooth, intuitive GUI with **Swing** components

---

## ✨ Features

* 🔐 **Login System** with role-based access (Admin/User)
* 🗂️ **Admin Dashboard** to view, add, or delete resources
* 🧳️ **Appointment Booking System** for end-users
* 💡 **Dark-themed Java Swing GUI**
* ✅ Input validation and user feedback
* 👥 **MySQL-backed persistence**

---

## 📸 Screenshots

---

## 🛠 Technologies Used

| Tech          | Purpose                        |
| ------------- | ------------------------------ |
| Java (Swing)  | GUI and core application logic |
| JDBC          | Connect Java with MySQL        |
| MySQL         | Backend database               |
| IntelliJ IDEA | Recommended IDE                |

---

## 📋 Prerequisites

* Java Development Kit (JDK) 8 or higher
  [Download Java](https://www.oracle.com/java/technologies/javase-jdk8-downloads.html)

* MySQL Community Server
  [Download MySQL](https://dev.mysql.com/downloads/mysql/)

* An IDE like IntelliJ or Eclipse (recommended)

---

## 🚀 Installation

### 🔧 Option 1: Run from Source

1. **Clone the Repository**

```bash
git clone https://github.com/Unmesh30/java-gui-app.git
cd java-gui-app
```

2. **Open in IntelliJ or Eclipse**

   * Choose "Open Project"
   * Set `Main.java` as the run configuration

3. **Update MySQL credentials** in:
   `src/com/appointment/DatabaseConnection.java`

```java
String url = "jdbc:mysql://localhost:3306/appointment_system";
String username = "root";
String password = "your_password";
```

4. **Run the App**

   * Right-click `Main.java` → Run
   * The Login screen will appear

---

## 🧠 Usage

### Default Accounts (you can add manually):

| Role  | Username | Password |
| ----- | -------- | -------- |
| Admin | admin    | admin123 |
| User  | user1    | user123  |

You can insert these into the `users` table directly via MySQL or Workbench.

### App Behavior:

* **Admin Login** ➞ Manage Resources & View Appointments
* **User Login** ➞ View Slots & Book Appointments
* **Logout** ➞ Returns to login screen

---

## 🗾 Database Configuration

### 1. Import SQL File

1. Open MySQL Workbench or CLI
2. Run `appointment_system.sql` (in project root)
3. It will:

   * Create a database named `appointment_system`
   * Set up the required tables (`users`, `appointments`, etc.)

### 2. Table Structure (example)

| Table          | Description                        |
| -------------- | ---------------------------------- |
| `users`        | Stores usernames, passwords, roles |
| `resources`    | List of bookable resources         |
| `appointments` | Tracks who booked what & when      |

---

## 🧱 Project Structure

```
java-gui-app/
├── appointment_system.sql
└── AppointmentSystem/
    └── src/com/appointment/
        ├── Main.java
        ├── LoginFrame.java
        ├── UserFrame.java
        ├── AdminFrame.java
        ├── BookingFrame.java
        ├── DatabaseConnection.java
        ├── Appointment.java
        ├── User.java
        ├── Resource.java
        └── SwingUtilities.java
```

---

## 🚯 Troubleshooting

| Issue                          | Solution                                                            |
| ------------------------------ | ------------------------------------------------------------------- |
| App not launching              | Ensure you are running `Main.java` and not individual frames        |
| DB connection fails            | Check `DatabaseConnection.java` credentials and if MySQL is running |
| Tables not found               | Ensure `appointment_system.sql` was executed correctly              |
| GUI looks weird on macOS/Linux | Swing L\&F varies; UI still works as expected                       |

---

## 📄 License

This project is released under the [MIT License](LICENSE).
Use it freely for academic, personal, or commercial projects.

---

## 📞 Contact

**Unmesh Achar**
📧 [unmeshachar02@gmail.com](mailto:unmeshachar02@gmail.com)
🔗 [GitHub Profile](https://github.com/Unmesh30)
📘 [Project Repository](https://github.com/Unmesh30/java-gui-app)

---

🙏 *If you found this useful, please ⭐ star the repository and share it!*
🚩 **Jai Siya Ram | Jai Hanuman Ji Ki Jai**
