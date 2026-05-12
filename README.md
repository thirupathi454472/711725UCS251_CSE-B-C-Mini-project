# README.md

````md
# Bank Account Management System in C

A simple Bank Account Management System developed in C using random-access files.  
This project allows users to create, update, search, delete, and transfer money between accounts.

---

# Features

- Create new bank accounts
- Update account balance
- Delete existing accounts
- Search accounts by last name
- Transfer money between accounts
- Export account details to a text file
- Random-access file handling using `fseek()` and `fwrite()`

---

# Technologies Used

- C Programming Language
- File Handling
- Structures
- Random Access Files

---

# File Structure

```text
project/
│
├── bank.c
├── credit.dat
├── accounts.txt
└── README.md
````

---

# Structure Used

```c
struct clientData
{
    unsigned int acctNum;
    char lastName[15];
    char firstName[10];
    char phone[15];
    double balance;
};
```

---

# Menu Options

```text
1 - Store formatted text file
2 - Update an account
3 - Add a new account
4 - Delete an account
5 - Search account by name
6 - Transfer money
7 - End program
```

---

# How to Compile

## GCC Compiler

```bash
gcc bank.c -o bank
```

---

# How to Run

## Windows

```bash
bank.exe
```

## Linux / Mac

```bash
./bank
```

---

# Functionalities

## 1. Add New Account

Creates a new account with:

* Account Number
* First Name
* Last Name
* Phone Number
* Balance

---

## 2. Update Account

Allows deposit or withdrawal from an account.

Example:

```text
Enter charge (+) or payment (-):
```

---

## 3. Delete Account

Deletes an account permanently from the file.

---

## 4. Search by Name

Searches account details using last name.

---

## 5. Transfer Money

Transfers balance from one account to another.

Validation included:

* Account existence check
* Insufficient balance check

---

## 6. Export Accounts

Generates:

```text
accounts.txt
```

Contains all account details in formatted form.

---

# Concepts Used

* Structures
* Functions
* File Handling
* Binary Files
* Random Access
* `fseek()`
* `fread()`
* `fwrite()`
* `rewind()`

---

# Future Improvements

* ATM Login System
* PIN Authentication
* Transaction History
* Admin Dashboard
* Password Encryption
* GUI Interface
* Database Integration

---

# Example Output

```text
========================
      BANK SYSTEM
========================
1 - Add account
2 - Update account
3 - Delete account
4 - Search account
5 - Transfer money
6 - Exit
========================
```

---

# Author

Thirupathi S

---

# License

This project is for educational purposes.

```
```
