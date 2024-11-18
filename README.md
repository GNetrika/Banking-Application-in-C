Bank Management System in C
Overview
This project is a simple Bank Management System implemented in C. It allows users to create an account, log in to their account, check their balance, deposit and withdraw money, and change their password. Each user’s data is stored in a separate text file, named after their phone number. The program demonstrates basic file handling, user input, and struct usage in C.

Features
Create a New Account: Users can create a new account by providing their personal information such as name, father's name, mother's name, address, Aadhar number, account number, phone number, and password. The initial balance is set to zero.

Login to an Existing Account: Users can log in to their account using their phone number and password.

Check Balance: Once logged in, users can check their current account balance.

Add Cash: Users can deposit money into their account, which updates their balance.

Withdraw Cash: Users can withdraw money from their account, provided the amount is a multiple of 500 and less than or equal to the balance.

Change Password: Users can change their account password after entering the old password.

Exit: Users can exit the application.

Code Structure
The program uses a struct user to store user details such as name, father's name, mother's name, address, Aadhar number, account number, phone number, password, and balance.

It uses file handling to save and retrieve user data. Each user's data is stored in a separate text file named after their phone number.

A do-while loop is used to repeatedly show the main menu and perform operations until the user chooses to exit.

How to Compile and Run
Compile the Program: Use the GCC compiler to compile the program.

bash
Copy code
gcc -o bank_management_system bank_management_system.c
Run the Executable: Run the compiled program.

bash
Copy code
./bank_management_system
Sample Run
markdown
Copy code
--------------------------------------------
**********BANK MANAGEMENT SYSTEM**********
      **********WELCOME***********
---------------------------------------------

---------------------------------------------
1. Create a new account
2. Login to your account
3. Exit
---------------------------------------------

Please enter your choice: 1

Enter your name: JohnDoe
Enter your father name: RobertDoe
Enter your mother name: MaryDoe
Enter your address: 123MainSt
Enter your Aadhar number: 123456789012
Enter your account number: 987654321
Enter your phone number: 1234567890
Enter your password: password123

Successfully registered
Improvements and Considerations
Security: Passwords are stored in plain text, which is not secure. Consider using encryption to store passwords.
Data Validation: Currently, the program does not perform rigorous input validation. Adding checks for valid input (e.g., valid phone numbers, Aadhar numbers) would improve reliability.
Concurrency: The system is not designed for concurrent access, so only one user should operate it at a time to avoid data corruption.
Error Handling: Enhance error handling, especially for file operations, to manage cases where files cannot be opened or read.
Conclusion
This Bank Management System provides a basic framework for understanding file operations, user authentication, and account management in C. It serves as a good starting point for learning and can be expanded with additional features and security measures for more robust applications.






