# 🛒 Supermarket Billing System

![Java](https://img.shields.io/badge/Language-Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white)
![Swing](https://img.shields.io/badge/GUI-Java%20Swing-5382A1?style=flat-square)

A desktop billing system for a supermarket, built with **Java Swing**. It has three roles (**Manager**, **Cashier** and **Data Entry Operator**), and each one gets its own screen and permissions.

I built this to practice **object-oriented design and role-based flows** in a GUI app, with simple text files acting as the database.

---

## ✨ Features

### 👔 Manager
- Create and delete **Cashier** and **Data Entry Operator** accounts

### 🧾 Cashier
- Add products to a bill by **product ID and quantity**
- See the running **total** update live
- Enter the customer's name and phone number and **print the bill** (saved as `<customer name>.txt`)

### 📦 Data Entry Operator
- **Add products** with ID, name, quantity and price
- **Remove products** by ID
- View the full **product list**

### 🔐 Login
- One login screen with a "Login As" dropdown for all three roles

## 🚀 Run it

Run the app from the `Supermarket Billing System` folder, because it reads and writes its `.txt` files there.

```bash
cd "Supermarket Billing System"
javac -d out src/*.java
java -cp out Main
```

Or open the folder in **IntelliJ IDEA** and run `Main.java`.

### Demo manager login

| Role    | Username | Password |
| ------- | -------- | -------- |
| Manager | `admin`  | `1234`   |

Log in as the manager first and create Cashier / Data Entry Operator accounts from there.

## 🗃️ Data files

| File | Stores |
| ---- | ------ |
| `cashierDB.txt` | Cashier accounts |
| `dataEntryOperatorDB.txt` | Data entry operator accounts |
| `productList.txt` | Products (ID, name, quantity, price) |

## 📁 Project structure

```text
Supermarket Billing System/src/
├── Main.java               # Entry point
├── Login.java              # Login screen for all roles
├── Manager.java            # Account management
├── Cashier.java            # Billing screen
└── DataEntryOperator.java  # Product management
```

---

Made by **Abdullah Al Jubayer** · [GitHub](https://github.com/abdullahaljubayer-101) · [Portfolio](https://abdullahaljubayer.com)
