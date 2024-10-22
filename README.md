# Banking System Java Project

This project is a basic banking system developed in Java. It provides a simple GUI for managing customer accounts, performing deposits and withdrawals, and printing customer balances. The system is designed for educational purposes and includes functionality to open new accounts, search and delete customers, and customize the interface.

## System Architecture

The project follows a simple client-side desktop application architecture built using Java Swing components for the user interface.

### Main Components:
- **Account Management**: Allows for creating, deleting, and searching customer accounts.
- **Transaction Management**: Supports depositing and withdrawing money from accounts.
- **Customer Information**: Displays individual customer details or a list of all customers.
- **Printing Module**: Allows printing of customer account balance reports.
- **Customization**: Enables users to change the background color and the look-and-feel of the GUI.

## Features and Functionality

### 1. Account Management
The system provides options to create new customer accounts, delete accounts, and search for accounts.

#### Key Actions:
- **Open New Account**: Opens a form to create a new account by entering account details (Account No, Name, Deposit Amount).
- **Delete Customer**: Allows the user to delete a customer record by entering the account number.
- **Search Customer**:
  - By account number or name.
  - Displays customer information like account number, name, last transaction date, and current balance.

### 2. Transaction Management
The system allows for deposits and withdrawals to be made in customer accounts.

#### Key Actions:
- **Deposit Money**: Users can enter an account number and deposit amount to increase the balance.
- **Withdraw Money**: Users can enter an account number and withdrawal amount. The system checks if the account has sufficient funds before completing the transaction.

### 3. Customer Information Display
The system supports two ways to view customer information:
- **View One by One**: Displays customer details one record at a time.
- **View All Customers**: Shows a list of all customer accounts in a table format.

### 4. Printing Customer Balance
Users can print a customer’s balance report:
- The system prompts for an account number.
- It retrieves the account details and sends them to the printer for printing.

### 5. Interface Customization
- Users can change the background color using a color picker.
- The look-and-feel of the application can be changed between different styles (e.g., Metal, Motif, Windows).

## Core Methods Overview

### `actionPerformed(ActionEvent ae)`
- Handles various user actions, including opening new accounts, depositing money, withdrawing money, deleting customers, and printing customer balance reports.

### `openChildWindow(String title)`
- Checks if a specific child window (e.g., "Create New Account") is already open; if not, it opens the corresponding window.

### `populateArray()`
- Reads all records from the database file (`Bank.dat`) and stores them in an array for searching and displaying customer information.

### `findRec(String rec)`
- Searches for a customer account by matching the account number with records in the array.

### `makeRecordPrint(int rec)`
- Prepares and formats the customer account details for printing, including the account number, name, last transaction, and current balance.

### `printRecord(String rec)`
- Sends the formatted customer balance information to the printer for printing.

### `getAccountNo()`
- Prompts the user to input an account number to retrieve and print the customer’s balance.

### `changeLookAndFeel(int val)`
- Updates the look-and-feel of the GUI based on the selected option (e.g., Metal, Motif, Windows styles).

### `quitApp()`
- Closes the application after displaying a confirmation dialog to the user. If the user confirms, the program terminates and releases system resources.

### `itemStateChanged(ItemEvent e)`
- Changes the layout of the application interface when a new look-and-feel option is selected by the user.

### `printCustomerReport()`
- Prepares and prints the customer’s balance report, including account details and transaction history.

### `closeAllWindows()`
- Closes all open internal windows within the application.

## How to Run the Project

1. **Clone the repository** or download the source code.
2. Open the project in your preferred IDE.
3. Compile the Java files and run the main class:
```cmd
javac Splash.java
java Splash
```
   
5. The GUI will launch, and you can start managing customer accounts.
   
## Requirements
Java: Version 8 or above
IDE: Any Java-compatible IDE like IntelliJ, Eclipse, or NetBeans

## License
This project is for educational use only. All rights to the code and system are reserved by Muhammad Wasif Javed.
   
