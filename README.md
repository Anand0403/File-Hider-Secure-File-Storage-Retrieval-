# File Hider – Secure File Storage & Retrieval  

## 📌 Overview  
This project implements a **secure file hiding and retrieval system** using **Java and MySQL**. It allows users to **hide files** by storing them in a **relational database** and later **retrieve (unhide)** them when needed. The system ensures **data security, controlled access, and efficient file handling**.  

---

## 🛠 Features  
### 1️⃣ Block Matching Algorithm  
The `hideFiles` function reads files from the system, converts them into binary format (`LONGBLOB`), and stores them securely in a MySQL database. The file is then deleted from the local storage to ensure privacy.  

### 2️⃣ Weighted Averaging Algorithm  
The `unhide` function retrieves hidden files from the database, reconstructs them, and saves them back to the system. OTP-based authentication is used to prevent unauthorized access.  

### 3️⃣ Security Mechanisms  
- **JDBC with Prepared Statements**: Prevents SQL Injection.  
- **JavaMail API for OTP Verification**: Ensures only authorized users can access stored files.  
- **File Lock Handling**: Addresses OS-level file lock issues to ensure smooth deletion after storage.  

---

## 🚀 Usage Instructions  
### 🔹 Prerequisites  
- Java 8+  
- MySQL Server  
- IntelliJ IDEA (or any Java IDE)  
- Maven (for dependency management)  

### 🔹 Setup & Installation  
#### 1️⃣ Clone the Repository  
```bash
git clone https://github.com/Anand0403/File-Hider-Secure-File-Storage-Retrieval-

