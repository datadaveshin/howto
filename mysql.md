# Start server:
`mysql.server start`

# Stop server:
`mysql.server stop`

# Start session from command line:
`mysql -u root -p`

# Show what databases exist
`SHOW DATABASES;`

# Connect to database
`USE <database>` ie. `USE sakila`

# Instructions from udemy course:
Steps to Install/Setup MySQL on Mac:

1. Install Homebrew through the Terminal
        --> Open terminal
        --> visit http://brew.sh/
        --> PASTE INTO TERMINAL: ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"

2. Install MySQL using Homebrew
        --> PASTE INTO TERMINAL: brew install mysql

3. Set your password
        PASTE THE FOLLOWING COMMANDS INTO TERMINAL
        --> PASTE INTO TERMINAL: mysql.server start
        --> PASTE INTO TERMINAL: mysql.server stop
        --> PASTE INTO TERMINAL: mysqld_safe --skip-grant-tables

    OPEN NEW TAB IN TERMINAL

        --> PASTE INTO TERMINAL: mysql -u root

    REPLACE 'password' WITH YOUR DESIRED PASSWORD WITHIN THE SINGLE QUOTES i.e. 'Pass1234!'
    THIS WILL BE WHAT YOU USE TO LOGIN TO MYSQL AND SEQUEL PRO MOVING FORWARD

        --> PASTE INTO TERMINAL (including semicolon): UPDATE mysql.user SET authentication_string=PASSWORD('password') WHERE User='root';
        --> PASTE INTO TERMINAL: FLUSH PRIVILEGES;

    CLOSE THIS TAB OF THE TERMINAL AND OPEN A NEW ONE

        --> PASTE INTO TERMINAL: mysql -u root -p

    You will be prompted to enter the password you set above: Enter password you set above without single quotes

    REPLACE 'password' WITH YOUR DESIRED PASSWORD WITHIN THE SINGLE QUOTES i.e. 'Pass1234!'

        --> PASTE INTO TERMINAL: ALTER USER 'root'@'localhost' IDENTIFIED BY 'password';

    YOU ARE DONE WITH THE TERMINAL!!!!

4. Download Sequel Pro
        --> http://www.sequelpro.com/download
        --> Download and open Application

5. Set Login in Sequel Pro
        --> Choose the 'Socket' option
        --> NAME: SQLforNEWBS
        --> USERNAME: root
        --> PASSWORD: enter password you set above without single quotes
        --> Before clicking 'Connect', click 'Save to Favorites'

6. Download and Install the Sakila DB
        --> Download the DB file from the 'Resources' Section of this lecture!
        --> Open the .zip file 
        --> Drag and Drop the file sakila-schema.sql into the 'Query' tab in Sequel Pro
              --> Select All 
              --> Click 'Run'
        --> Drag and Drop the file sakila-data.sql into the 'Query' tab in Sequel Pro
              --> Select All 
              --> Click 'Run'

Enjoy the course!!!
