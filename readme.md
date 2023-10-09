# Project README

## Project Title

**Banking Management System**

## Table of Contents

- [Introduction](#introduction)
- [Requirements](#requirements)
  - [Python](#python)
- [Installation](#installation)
- [Usage](#usage)
  - [Importing Modules](#importing-modules)
- [Execution](#execution)
  - [Option 1](#option-1)
  - [Option 2](#option-2)
- [Features](#features)
  - [Employee](#employee)
    - [Create Bank Account](#create-bank-account)
    - [Close Bank Account](#close-bank-account)
    - [Create Admin Account](#create-admin-account)
    - [Close Admin Account](#close-admin-account)
    - [Display Account Summary](#display-account-summary)
    - [Exit](#exit)
  - [Customer](#customer)
    - [Deposit](#deposit)
    - [Withdraw](#withdraw)
    - [Change PIN](#change-pin)
    - [Close Account](#close-account)
    - [Check Balance](#check-balance)
    - [Exit](#exit-1)
- [Input and Output](#input-and-output)
- [Contributors](#contributors)
- [License](#license)

## Introduction

Banking Management System is a Python-based banking management system with a graphical user interface (GUI). It facilitates tasks for both employees and customers. Employees can create and manage bank accounts, including admin accounts, while customers can perform banking operations such as depositing, withdrawing, changing their PIN, and checking their account balance. The system ensures data integrity and security through authentication and validation mechanisms.

## Requirements

### Python

- Python 3.x is required for running this program.

## Installation

### Tkinter

Banking Management System relies on the Tkinter library for its graphical user interface. Tkinter is included with standard Python installations. No separate installation is necessary.

### Datetime

The Datetime module is part of Python's standard library and does not require external installation.

### OS

The OS module is also part of Python's standard library and does not need to be downloaded separately.

## Usage

### Importing Modules

To use Banking Management System, import the required modules in your Python script:

```python
import os
from datetime import date
import tkinter as tk
from tkinter import *
```

## Execution

### Option 1

1. Extract the provided zip file.
2. Navigate to the `mainProject.py` file.
3. Open the code in your preferred IDE or code editor (Python must be installed on your system).
4. Run the code.
5. You can now interact with the Python-based GUI program.

### Option 2

1. Extract the provided zip file.
2. Navigate to the directory containing the extracted folder.
3. Locate the `mainProject.py` file.
4. Open a command prompt in the folder by clicking on the location bar in Windows Explorer and typing `cmd`, then pressing Enter.
5. Execute the following command (Python must be pre-installed on your system):
   ```shell
   python mainProject.py
   ```

6. You can now interact with the Python-based GUI program.

## Features

### Employee

#### Create Bank Account

- Requires Admin ID and password authentication.
- Functionalities:
  - Create a bank account with details such as account type, name, gender, nationality, account number, PIN, KYC documents, date of birth, mobile number, and initial account balance.
  - Input data is validated based on various criteria, and appropriate error messages are displayed if data does not meet validation requirements.

#### Close Bank Account

- Allows deleting an account based on the specified account number.
- Verifies if the entered account number exists and throws an error if it doesn't.

#### Create Admin Account

- Requires Admin ID and password authentication.
- Functionalities:
  - Create a new admin account with an Admin ID and password.
  - Checks if the entered Admin ID already exists and ensures the password matches the confirm password.

#### Close Admin Account

- Deletes the admin account based on the specified Admin ID and password.
- Verifies if the entered Admin ID exists and ensures it is not the same as the currently logged-in admin.
- Validates the entered password associated with the Admin ID.

#### Display Account Summary

- Displays account details based on the entered account number.
- Verifies if the entered account number exists and throws an error if it doesn't.

#### Exit

- Returns to the admin login screen.

### Customer

#### Deposit

- Allows customers to deposit a valid amount into their account.
- Validates the deposit amount to ensure it is not negative, not greater than 25000, and maintains a minimum balance.

#### Withdraw

- Allows customers to withdraw a valid amount from their account.
- Validates the withdrawal amount to ensure it is not greater than the total balance, not negative, and maintains a minimum balance.

#### Change PIN

- Enables customers to change their PIN by entering a new PIN and confirming it.
- Validates the new PIN to ensure it is numeric and four digits long and that it matches the confirmation.

#### Close Account

- Requires customers to enter their PIN to verify their identity.
- Closes the customer's account if the entered PIN matches the one in the database.

#### Check Balance

- Displays the total balance of the customer's account.

#### Exit

- Returns to the customer login screen.

## Input and Output

For a detailed demonstration of the input and output of the program, you can watch the [YouTube Video](http://bit.ly/psc-project) provided with the permission of Prof. Mohd Zuhair.

## Contributors

1. 19BCE237 - Sakshi Sanghavi
2. 19BCE238 - Harshil Sanghvi
3. 19BCE245 - Aayush Shah

## License

Banking Management System is an open-source project developed solely for an innovative assignment in the "Programming for Scientific Computing" course. It is free to use, modify, and distribute as needed.
