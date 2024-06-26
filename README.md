# JTDV Admin System

![JTDV Security Agency](jtdv-admin-dashboard.png?raw=true "JTDV Security Agency")

### <a href="https://jtdv.tech/login.php">LIVE DEMO</a>

## System Description

Employee, Company, and Secretary Accounts are created through the JTDV Admin System. It also keeps track of personnel who have been allocated to a given firm. It is also responsible for accepting or denying an employee's request for leave. This also manages to track an employee's infractions and notify them.

## Guide to install in your local machine.

### 1. Make sure you have XAMPP installed! 🚀

To begin, you must first download and install xampp on your local computer. Simply click the config and then the PHP(php.ini) file once it has been installed.

Search for ```;extension=openssl``` and scroll down a little to find the code below. Make sure you format it according to these guidelines.

```;extension=pdo_firebird``` <br/>
```extension=pdo_mysql```<br/>
```;extension=pdo_oci```<br/>
```extension=pdo_odbc```<br/>
```extension=pdo_pgsql```<br/>
```extension=pdo_sqlite```<br/>

### 2. Install Composer.exe 🚀 <a href="https://getcomposer.org/download/">(click me)</a> 

### 3. Clone the repo! 🚀
Go to this link and clone or download <br/>
```https://github.com/imfizz/latest-payroll-design.git``` and place it inside xampp/htdocs

### 4. Import Database in Xampp 🚀

You may find database inside the cloned repository. Try to import this in xampp server.
1. Run Apache and Mysql in Xampp
2. Go to ```localhost/phpmyadmin```
3. Create Database named ```payroll```
4. Click import and locate the given database in the cloned repository.


### 5. Install Packages 🚀

Open your command prompt and type ```cd``` and drag the folder of the cloned repository.<br/>
Type ```composer install``` and hit enter to install the packages needed.


### 6. Last Step! 🚀

In the root directory of the cloned repository, create ```.env``` file and type this <br/>

```E_USERNAME=youremailaddress``` <br/>
```E_PASSWORD=youremailpassword```

Run your xampp server and go to this link <br>
Admin: ```localhost/foldername/login.php``` <br>
Employee: ```localhost/foldername/m_login.php```


🚀 BOOM you may use the system now.


### Helpers: 😎✨
To find the credentials of admin in the database, go to table `secret_diary`

To find the credentials of employee in the database, go to table `secret_diarye`. you can use `les soriano` account.

If you want to deploy the database choose `jtdvpayroll.sql`

