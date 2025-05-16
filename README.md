**ATM Transaction System in C**
Overview
This project simulates an ATM transaction system using C programming. It covers functionalities like user authentication (PIN verification), deposit, withdrawal, balance checking, and even PIN changing. The project is modular, with multiple source files that each handle specific tasks. The program also uses file handling for storing user data and transaction records.

Features
User Authentication: Verifies user PIN with error handling for incorrect PIN attempts.

Deposit & Withdrawal: Allows users to deposit and withdraw money, with account balance updates.

Balance Check: Displays the user's current balance.

PIN Change: Provides functionality for the user to change their PIN.

File Handling: Stores user details, transaction records, and other essential data in files for persistence.

Modular Code: Divided into various files for better readability and maintenance.

Project Structure
graphql
Copy
Edit
ATM-Transaction-System/
│
├── mainscrre.c       # Main program that integrates all functionalities
├── balance.c         # Handles balance checking
├── deposit.c         # Handles deposit transactions
├── fastcash.c        # Implements fast cash withdrawal functionality
├── pinchange.c       # Allows users to change their PIN
├── pinwrong.c        # Handles incorrect PIN verification
├── tpins.c           # Manages PIN initialization
├── transfer.c        # Handles money transfer between accounts
├── withdraw.c        # Handles withdrawal transactions
└── user_data.txt     # File storing user data and transaction records
How It Works
Authentication: The user is prompted to enter their PIN. If the PIN is correct, they are given access to the main menu. If incorrect, they are asked to try again.

Main Menu: Once authenticated, the user can choose one of the following options:

Deposit: Add money to the account.

Withdraw: Withdraw money from the account.

Balance Check: View the current account balance.

PIN Change: Change the PIN for account security.

Fast Cash: A quick way to withdraw a preset amount.

Transfer: Transfer money to another account.

Transactions: For deposit and withdrawal, the program updates the balance and saves the new balance to the file. Transactions are recorded for future reference.

Getting Started
Prerequisites
A C compiler (e.g., GCC).

Basic knowledge of C programming and file handling.

Installation
Clone the repository:

bash
Copy
Edit
git clone https://github.com/yourusername/ATM-Transaction-System.git
Navigate to the project directory:

bash
Copy
Edit
cd ATM-Transaction-System
Compile the project using GCC:

bash
Copy
Edit
gcc -o atm mainscrre.c balance.c deposit.c fastcash.c pinchange.c pinwrong.c tpins.c transfer.c withdraw.c
Run the program:

bash
Copy
Edit
./atm
Usage
Login: Enter the PIN to access the system.

Main Menu: Once logged in, you can select from the following options:

Deposit: Deposit money into your account.

Withdraw: Withdraw money from your account.

Balance: Check your current account balance.

PIN Change: Change your PIN for security purposes.

Fast Cash: Quickly withdraw a preset amount.

Transfer: Transfer money to another account.

The program will save all transaction records and account details in a text file (user_data.txt).

Example Output
markdown
Copy
Edit
Welcome to ATM
Please enter your PIN: ****
Incorrect PIN. Try again.

Please enter your PIN: 1234
PIN verified successfully!

Main Menu:
1. Deposit
2. Withdraw
3. Balance
4. PIN Change
5. Fast Cash
6. Transfer
7. Exit
Choose an option: 1

Enter deposit amount: 500
Deposit successful! New balance: 500

Main Menu:
1. Deposit
2. Withdraw
3. Balance
4. PIN Change
5. Fast Cash
6. Transfer
7. Exit
Choose an option: 2

Enter withdrawal amount: 200
Withdrawal successful! New balance: 300
Code Explanation
mainscrre.c: Contains the main entry point and integrates all other functionalities.

balance.c: Responsible for displaying the current balance.

deposit.c: Handles the deposit functionality, updating the balance.

fastcash.c: Provides functionality for quick withdrawal of preset amounts.

pinchange.c: Allows the user to change their PIN.

pinwrong.c: Handles PIN verification and incorrect PIN attempts.

tpins.c: Manages the initial PIN setup.

transfer.c: Handles the functionality of transferring money between accounts.

withdraw.c: Manages the withdrawal process, ensuring sufficient balance.

Contributing
Feel free to fork the repository and submit pull requests for improvements or additional features.

Bugs & Issues
If you encounter any issues or bugs, please open an issue in the GitHub repository.
