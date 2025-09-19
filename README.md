# Bank Management System - C++

A robust console-based bank management system written in C++ that demonstrates Object-Oriented Programming concepts, file handling, input validation, and cross-platform compatibility.

## ✨ Features

### 🏦 **Core Banking Operations**
- ✅ Create new bank accounts with unique account numbers
- ✅ Deposit money into accounts
- ✅ Withdraw money (with insufficient balance protection)
- ✅ Check account balance and details
- ✅ View all account holders list
- ✅ Modify existing account information
- ✅ Delete/close accounts

### 🛡️ **Security & Validation**
- ✅ **Unique Account Numbers**: Prevents duplicate account creation
- ✅ **Input Validation**: Menu input verification (1-8 only)
- ✅ **Balance Protection**: Prevents overdraft withdrawals
- ✅ **File Safety**: Proper file handling and error checking

### 🌍 **Cross-Platform Support**
- ✅ **Windows**: Uses `CLS` command
- ✅ **Linux/macOS**: Uses `clear` command
- ✅ **Automatic Detection**: No manual configuration needed

### 💾 **Data Persistence**
- ✅ Binary file storage (`account.dat`)
- ✅ Data persists between program sessions
- ✅ Efficient file operations

## 🚀 How to Run

### Method 1: Visual Studio (Windows)
1. Create a new **Console Application** project
2. Replace all default code with `bank_management.cpp`
3. Build and run (**Ctrl+F5**)

### Method 2: Command Line Compilation
```bash
# Windows (MinGW/GCC)
g++ -o bank_system.exe bank_management.cpp

# Linux/macOS
g++ -o bank_system bank_management.cpp
./bank_system
```

### Method 3: Online Compilers
- Copy the code to [Repl.it](https://replit.com), [OnlineGDB](https://onlinegdb.com), or similar platforms

## 📖 User Guide

### Main Menu Options
```
======================
BANK MANAGEMENT SYSTEM
======================
::MAIN MENU::

1. NEW ACCOUNT           - Create a new bank account
2. DEPOSIT AMOUNT        - Add money to an account
3. WITHDRAW AMOUNT       - Remove money from an account
4. BALANCE ENQUIRY       - Check account details
5. ALL ACCOUNT HOLDER LIST - View all accounts
6. CLOSE AN ACCOUNT      - Delete an account
7. MODIFY AN ACCOUNT     - Update account information
8. EXIT                  - Close the program
```

### 🆕 Creating Your First Account
```
Select Your Option (1-8): 1

Enter the Account No. : 1001
Enter the Name of the Account holder : John Doe
Enter Type of the Account (C/S) : S
Enter The Initial amount : 5000

Account Created Successfully!
```

### 🔄 Making a Deposit
```
Select Your Option (1-8): 2

Enter The account No. : 1001

Account No. : 1001
Account Holder Name : John Doe
Type of Account : S
Balance amount : 5000

TO DEPOSIT AMOUNT
Enter The amount to be deposited: 1500

Record Updated
```

### ⚠️ Error Handling Examples

**Duplicate Account Number:**
```
Enter the Account No. : 1001

ACCOUNT NUMBER ALREADY EXISTS!
Please choose a different account number.
Press any key to continue...
```

**Invalid Menu Input:**
```
Select Your Option (1-8): 9

INVALID INPUT! Please enter a number between 1-8.
Press any key to continue...
```

**Insufficient Balance:**
```
TO WITHDRAW AMOUNT
Enter The amount to be withdraw: 10000

Insufficience balance
```

## 📊 Account Types

| Type | Code | Description |
|------|------|-------------|
| **Savings** | `S` | Standard savings account |
| **Checking** | `C` | Standard checking account |

## 🗂️ File Structure

The program automatically creates these files:

```
📁 Program Directory/
├── 🗃️ account.dat     - Main database (binary format)
├── 🗃️ Temp.dat        - Temporary file for deletions
└── 💻 bank_management.cpp - Your source code
```

## 🔧 Technical Details

### Programming Concepts Demonstrated
- **Object-Oriented Programming**: Classes, encapsulation, methods
- **File I/O Operations**: Binary file handling, stream management
- **Input Validation**: Menu and data validation
- **Cross-Platform Code**: Preprocessor directives
- **Memory Management**: Proper resource cleanup
- **Error Handling**: File operations and user input

### System Requirements
- **Compiler**: GCC, Clang, MSVC, or any C++11 compatible compiler
- **Operating System**: Windows, Linux, macOS, or Unix-like systems
- **Permissions**: Write access to program directory
- **Memory**: Minimal (< 1MB)

## 🐛 Troubleshooting

### Common Issues & Solutions

**❌ "File could not be open" error**
- **Cause**: No write permissions or antivirus blocking
- **Solution**: Run as administrator or add folder to antivirus exclusions

**❌ Compilation errors**
- **Cause**: Missing C++ compiler or wrong compiler flags
- **Solution**: Install GCC/MinGW or use an IDE like Code::Blocks

**❌ Screen doesn't clear properly**
- **Cause**: System doesn't support the clear command
- **Solution**: Code automatically handles this, but you can modify `syst` variable if needed

**❌ Data disappears**
- **Cause**: `account.dat` file deleted or moved
- **Solution**: File is recreated automatically when you create new accounts

### Performance Notes
- **File Size**: Each account takes ~60 bytes of storage
- **Speed**: Can handle thousands of accounts efficiently
- **Limitations**: Single-user system (no concurrent access)

## 🎯 Future Enhancements

Potential improvements you could add:
- 🔐 Password/PIN protection for accounts
- 📧 Transaction history logging
- 💳 Different account types with interest calculations
- 🌐 Network support for multiple users
- 📱 GUI interface using Qt or similar framework
- 🗄️ Database integration (MySQL, SQLite)

## 📝 License

This project is for **educational purposes** and demonstrates C++ programming concepts. Feel free to use, modify, and distribute for learning and non-commercial purposes.

## 🤝 Contributing

Found a bug or want to improve the code? Contributions are welcome! This is a great project for learning C++ fundamentals.

---

**Happy Banking! 🏦💰**
