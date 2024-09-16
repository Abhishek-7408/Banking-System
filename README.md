Banking System
Overview
This C++ project implements a simple banking system that allows users to perform basic banking operations such as opening an account, depositing and withdrawing money, checking balance, closing an account, and viewing all accounts. It demonstrates file handling for persistent data storage and exception handling for managing errors.

Features
Open an Account: Create a new bank account with an initial balance.
Balance Enquiry: Check the balance and details of an existing account.
Deposit: Add funds to an existing account.
Withdraw: Withdraw funds from an account with a check to prevent falling below a minimum balance.
Close an Account: Delete an existing account and remove it from the system.
Show All Accounts: Display details of all existing accounts.
Persistent Storage: Account data is saved to and loaded from a file (Bank.data) to maintain state between program runs.
Classes
Account

Manages individual account details, including account number, holder's name, and balance.
Provides methods to deposit and withdraw funds with error handling for insufficient funds.
Static methods and variables to manage account numbers.
Bank

Manages a collection of accounts using a map for fast lookups.
Handles operations such as opening, closing, depositing, withdrawing, and showing accounts.
Handles file I/O for saving and loading account data.
Exception Handling
InsufficientFunds: Custom exception class to handle scenarios where a withdrawal would result in a balance below the minimum required balance.
File Handling
Bank.data: File used for persistent storage of account data. The file is read at the start of the program and written to at the end, ensuring that all changes are saved.
