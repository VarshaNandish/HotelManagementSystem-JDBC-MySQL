# 🏨 Hotel Management System (Java + JDBC + MySQL)

A simple console-based Hotel Management System built using **Java**, connected to **MySQL** via **JDBC**. The application allows hotel staff to perform essential operations like reserving rooms, viewing all reservations, updating guest details, and deleting records.

---

## 📋 Features

- Reserve a Room (Guest Name, Room Number, Contact)
- View All Reservations in a tabular format
- Get Room Number by Reservation ID and Guest Name
- Update Reservation Details
- Delete Reservation
- Exit the Application Gracefully

---

## 🛠 Technologies Used

- Java (JDK 8+)
- JDBC (Java Database Connectivity)
- MySQL (Database)
- IntelliJ IDEA 

---

## 🗃️ Database Schema (MySQL)

```
CREATE DATABASE hotel_db;

USE hotel_db;

CREATE TABLE reservations (
    reservation_id INT AUTO_INCREMENT PRIMARY KEY,
    guest_name VARCHAR(100),
    room_number INT,
    contact_number VARCHAR(15),
    reservation_date TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);
```

---

## 🚀 How to Run

1. Clone this repository or download the ZIP.
2. Open the project in IntelliJ or any Java IDE.
3. Make sure MySQL is installed and running.
4. Update the DB credentials in `HotelManagementSystem.java`:

```
private static final String url = "jdbc:mysql://localhost:3306/hotel_db";
private static final String username = "root";
private static final String password = "your_password";
```

5. Run the `HotelManagementSystem.java` file.

---

## 💡 Future Enhancements

- Add check-in/check-out date fields
- Create a separate Room table to manage availability
- Implement login system for admin/staff
- GUI interface using JavaFX or Swing

---

## 👩‍💻 Created by
Varsha S P

Java Developer | Learner | Enthusiast

---

## 📄 License

---

This project is for educational/demo purposes only. 
This project is open-source and free to use for learning or modification.

