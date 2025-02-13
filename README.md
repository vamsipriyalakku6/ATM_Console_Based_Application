# ATM_Console_Based_Application
## Overview
ATM_Console Based Application is a simple Python-based ATM system that allows users to perform basic banking operations such as withdrawing money, depositing money, generating a PIN, and viewing their account details.

## Features
- Withdraw money
- Deposit money
- Generate a new PIN
- View mini statements (account details)
- Exit the application

## Requirements
- Python 3.x

## Usage
1. Run the script in a Python environment.
2. Choose an option from the menu displayed:
   - 1: Withdraw money
   - 2: Deposit money
   - 3: Generate a PIN
   - 4: View Mini Statement
   - 5: Exit

## Account Structure
The application maintains accounts in a dictionary format with the following structure:
```python
accounts = {
    account_number: [balance, pin, email, username]
}
```
Example:
```python
accounts = {
    50001: [10000, 2002, "user1@gmail.com", "user1"],
    50002: [20000, 1234, "user2@gmail.com", "user2"],
    50003: [15000, None, "user3@gmail.com", "user3"]
}
```

## Functionality
### 1. Withdraw Money
- Users must enter their account number and PIN to withdraw money.
- The system checks for sufficient balance before processing the withdrawal.

### 2. Deposit Money
- Users must enter their account number and deposit an amount.

### 3. PIN Generation
- Users can set up a new PIN if one has not been created.
- If a PIN already exists, the system notifies the user.

### 4. Mini Statement
- Users can view their account details after entering their PIN.

### 5. Exit
- The program terminates and displays a thank-you message.

## Error Handling
- Invalid account number entries.
- Incorrect PIN entries.
- Insufficient balance during withdrawal.

## How to Run the Application
1. Save the Python script as `atm_application.py`.
2. Run the script using:
   ```sh
   python atm_application.py
   ```
3. Follow the on-screen instructions to interact with the application.

## Future Enhancements
- Add account creation functionality.
- Implement transaction history.
- Integrate with a database for persistent data storage.


