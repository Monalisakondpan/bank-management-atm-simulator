Project Overview
I developed a Bank Management System as a Java desktop application (not a website), using Swing for the graphical user interface (GUI), NetBeans IDE for development, and MySQL as the backend database. The project simulates the core functionalities of a real-world bank ATM system, allowing users to perform various banking operations through an interactive interface.

Technologies Used
Java: The main programming language for the application logic and GUI.
Swing: For building the desktop application's graphical user interface.
NetBeans: The IDE I used for designing, coding, and managing the project.
MySQL: The relational database used to store user data, transactions, and account information.
JDBC: Java Database Connectivity for connecting Java code to the MySQL database.

Project Structure
src/bank/management/system/: Contains all Java source files for the application.
icons/: Contains images used in the GUI (e.g., ATM and logo images).
nbproject/: NetBeans project configuration files.
build.xml: Ant build script for compiling and running the project.

Main Features & Flow
User Authentication
The application starts with a Login screen, where users enter their card number and PIN.
Credentials are checked against the MySQL database.
If authentication is successful, the user is taken to the main transaction menu.

User Registration (Sign Up)
New users can sign up by clicking the Sign Up button.

The sign-up process is divided into three steps:
SignupOne: Collects personal details (name, father's name, DOB, gender, email, marital status, address, etc.).
SignupTwo: Collects additional details (religion, category, income, education, occupation, PAN, Aadhar, senior citizen status, existing account).
SignupThree: Lets the user select account type, services, and generates a card number and PIN.
All details are stored in the database.

Main Transaction Menu
After login, users see the Transactions screen, which offers:
Deposit
Cash Withdrawal
Fast Cash (quick withdrawal of preset amounts)
Mini Statement
Pin Change
Balance Enquiry
Exit

Banking Operations
Deposit: Users can deposit money, which updates their balance in the database.
Withdrawl: Users can withdraw money, with checks for sufficient balance.
Fast Cash: Allows users to quickly withdraw preset amounts.
Mini Statement: Shows recent transactions and current balance.
Pin Change: Users can change their PIN, which updates all relevant tables in the database.
Balance Enquiry: Displays the current account balance.

Database Connectivity
All database operations are handled via a dedicated connection class, which establishes a connection to MySQL and provides a Statement object for executing SQL queries.
How the Application Works (Story Style)
Starting the App: I launch the application, which opens the login window.
Logging In or Signing Up:
If I already have an account, I enter my card number and PIN to log in.
If not, I click "Sign Up" and go through a three-step registration process, entering personal and account details.
After registration, the system generates a card number and PIN, which I can use to log in.
Performing Transactions:
Once logged in, I am presented with a menu of banking options.
I can deposit or withdraw money, check my balance, view a mini statement, change my PIN, or use fast cash for quick withdrawals.
Each operation updates or retrieves data from the MySQL database, ensuring data consistency and security.
Logging Out: I can exit the application at any time.
Is it an Application or Website?
This is a Java desktop application, not a website.
It runs as a standalone program on my computer, with a graphical interface built using Java Swing. All interactions happen within the application window, not in a web browser.

Tools Used
NetBeans IDE: For designing forms, writing code, and managing the project.
MySQL: For storing all user and transaction data.
Java Swing: For building the user interface.

Summary
I built a full-featured desktop banking application that simulates ATM operations, complete with user registration, authentication, and all essential banking transactions. The project demonstrates my skills in Java, GUI development, database integration, and application design using NetBeans and MySQL.
