# 🍔 Food Ordering App

A responsive web-based Food Ordering Application built using **HTML**, **CSS**, **Java (Servlets)**, and **MySQL**. Users can register, browse restaurants, view menus, place orders, and store order information in a relational database.

---

## 🧰 Tech Stack

- **Frontend**: HTML, CSS
- **Backend**: Java (Servlets + JDBC)  
- **Database**: MySQL  
- **Server**: Apache Tomcat  
- **IDE**: Eclipse

---

## 🚀 Features

- 🧑‍💻 User Registration & Login  
- 🏪 View Restaurants and Menus  
- 🍴 Place Food Orders  
- 🧾 View Order Summary  
- 🗃️ MySQL database integration  
- 📦 Order History (optional feature)  
- 🧑‍🍳 Admin Panel (optional enhancement)

---

## 🗃️ Database Schema

1. **Users Table**
   - `id` (INT, PK)
   - `name` (VARCHAR)
   - `email` (VARCHAR)
   - `phone` (VARCHAR)
   - `password` (VARCHAR)

2. **Restaurants Table**
   - `id` (INT, PK)
   - `name` (VARCHAR)
   - `location` (VARCHAR)

3. **Items Table**
   - `id` (INT, PK)
   - `name` (VARCHAR)
   - `price` (DECIMAL)
   - `restaurant_id` (FK → Restaurants.id)

4. **Orders Table**
   - `id` (INT, PK)
   - `user_id` (FK → Users.id)
   - `item_id` (FK → Items.id)
   - `quantity` (INT)
   - `order_date` (DATETIME)

---

## 🛠️ Setup Instructions

### ✅ Prerequisites
- JDK installed (Java 8 or later)
- Eclipse IDE
- Apache Tomcat (9.x or later)
- MySQL Server (with MySQL Workbench)

### 📥 Clone Repository

```bash
git clone https://github.com/your-username/food-ordering-app.git
