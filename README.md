# 🏦 Bank Management System (C++)

A simple **Bank Management System** built using **C++**, using file handling techniques.  
This project allows managing clients, performing transactions, and managing system users with permissions.

---

## 📌 Features

### 👥 Clients Management
- Show all clients list
- Add new client
- Update client information
- Delete client
- Find client by account number

### 💰 Transactions
- Deposit money
- Withdraw money
- Show total balances for all clients

### 👤 Users Management (Admin System)
- List all users
- Add new user
- Delete user (except Admin)
- Update user information
- Find user
- Permissions system for controlling access

---

## 🔐 Permissions System

Each user has a permissions value that determines what they can access.

Permissions include:
- List Clients
- Add Client
- Delete Client
- Update Client
- Find Client
- Transactions
- Manage Users  
- Full Access (`-1`)

---

## 🗂️ Data Storage

The project stores data in text files using a separator:

### Clients File
📄 `Clients.txt`

Format:
