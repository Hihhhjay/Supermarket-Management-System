# 🛒 Supermarket-Management-System
This project implements a Java-based graphical e-commerce system using socket communication, consisting of a client and server. It supports user registration and login, product browsing, shopping cart management, order placement and tracking, as well as centralized management of inventory, order statuses, and admin accounts by administrators. All data is stored in an SQLite database, with front-end and back-end communication handled via JSON protocol.

---

# 🧰 Requirements

- Java JDK 8 or higher
- SQLite JDBC Driver (recommended version: 3.36.0.3)
- Operating Systems: Windows / macOS / Linux

📄 See `requirements.txt` for detailed setup.

---

# 🚀 How to Use

## 1. Download the SQLite JDBC Driver

Download the JAR from [https://github.com/xerial/sqlite-jdbc](https://github.com/xerial/sqlite-jdbc) and place it in your project directory.

---

## 2. Compile All Java Files

```bash
javac -cp .:sqlite-jdbc-3.36.0.3.jar *.java
```

> On Windows, use `;` instead of `:` in classpath.

---

## 3. Run the Server

```bash
java -cp .:sqlite-jdbc-3.36.0.3.jar Server
```

---

## 4. Launch the Client

```bash
java -cp .:sqlite-jdbc-3.36.0.3.jar Start
```

- The first time you run it, you’ll be prompted to create an admin account.
- After that, you can log in as admin or register as a user to start shopping.

---

# 👩‍💼 Admin Features

- Add / update / delete inventory items
- Change order statuses (Processing, Ready for pickup, etc.)
- Create new admin accounts

---

# 👤 User Features

- Register / login
- Browse inventory
- Add to cart, checkout, and delete items
- View order history and details

---

# 📦 Data Storage

All data is stored in `st_manage.db` using the following tables:
- `users`
- `inventory`
- `cart`
- `orders`
- `order_items`

---


