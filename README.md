# 🏦 Bank Management System 

A console-based **Bank Management System** developed in **C++**, using **file handling** and a **user authentication system with permissions (bitwise access control)**.

This project simulates real banking operations such as managing clients, handling transactions, and controlling system users with secure access levels.

---

## 📌 Features

### 👥 Clients Management
- Show all clients list  
- Add new client  
- Update client information  
- Delete client  
- Find client by account number  

---

### 💰 Transactions System
- Deposit money  
- Withdraw money  
- View total balances of all clients  

---

### 👤 Users Management (Admin System)
- Show all users  
- Add new user  
- Delete user (**Admin user is protected**)  
- Update user information  
- Find user by username  
- Assign permissions per user  

---

### 🔐 Authentication System
- Login screen (Username + Password)  
- Session stored in `CurrentUser`  
- Login retry until valid credentials  
- Logout returns to login screen  

---

## 🔐 Permissions System (Bitwise Control)

Each user has an **integer permission value** that controls system access.

### 🧠 Permission Values

| Permission        | Value |
|------------------|------|
| Show Clients     | 1    |
| Add Client       | 2    |
| Delete Client    | 4    |
| Update Client    | 8    |
| Find Client      | 16   |
| Transactions     | 32   |
| Manage Users     | 64   |
| Full Access      | -1   |

---

### ⚙️ Permission Check Logic

Access is verified using bitwise AND:

```cpp
(CurrentUser.Permissions & Permission) == Permission
