# mysql-utils
A repo with utils regarding MySQL

## Windows

1.Install Chocolatey Windows package manager from https://chocolatey.org/install


Open the PowerShell as Admin

2.To install MySQL
>choco install mysql

your connection data will be: 
- user = 'root'
- psq = ''

3.To install MySQL-WorkBench
>choco install mysql.workbench

## Mac OS

1. Make sure you have installed brew, if not, run the following command and follow the instructions:

>/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"

2. Run the following command to instal MySql

>brew install mysql

3. Start MySQL service: 
>brew services start mysql

4. Additionaly you can run the following command to enable security features and setup a password:

>mysql_secure_installation

5. Download MySQL Workbench from the follwing link: https://dev.mysql.com/downloads/workbench/

6. The process to install MySQL Workbench is to drag and drop it into your apps folder. After that you should be able to run it.


## Usefull commands

CREATE USER 'ironhacker'@'localhost' IDENTIFIED BY '1r0nh4ck3r';

GRANT ALL PRIVILEGES ON *.* TO 'ironhacker'@'localhost';

FLUSH PRIVILEGES;

to delete a user
>DROP USER 'username'@'localhost';
