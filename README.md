# 1. INSTALLING REQUIRED ENVIRONMENTS

*Note: The installation guide below is applicable for the Windows operating system.*

## 1.1 Install XAMPP - Including Apache, PHP, MySQL

1. Download and install the XAMPP software package from [XAMPP Installers and Downloads](https://www.apachefriends.org/index.html).

2. After installation, open the XAMPP Control Panel to manage services.

![XAMPP](https://github.com/TruongLeDuy123/intern_assignment/blob/main/readme%20source/img/xampp1.png)

3. The XAMPP Control Panel will display services such as:

   - **Apache:** Web server service.
   - **MySQL:** Database management system.
   - (Other services if available).
4. Start Apache and MySQL through the XAMPP Control Panel (Actions Start on the XAMPP Control Panel).

5. Open a web browser and check the URL http://localhost:3000.

![XAMPP](https://github.com/TruongLeDuy123/intern_assignment/blob/main/readme%20source/img/xampp2.png)
**Note:** Adjust the port according to your device.

## 1.2 Install Composer

1. Download and run the Composer-Setup.exe file to install Composer on your computer via the link: [Composer](https://getcomposer.org/)

2. After installation, check the installation via the Windows Command Line or Git Bash with the command 'composer'.

![Composer Installation Success](https://github.com/TruongLeDuy123/intern_assignment/blob/main/readme%20source/img/composer1.png)
*Composer Installation Success*

## 1.3 Install Related Extensions on VS Code

Install 2 PHP support extensions for VS Code as follows:

![Extension](https://github.com/TruongLeDuy123/intern_assignment/blob/main/readme%20source/img/extension1.png)
![Extension](https://github.com/TruongLeDuy123/intern_assignment/blob/main/readme%20source/img/extension2.png)

# 2. SETUP PROJECT AND RUN
## 2.1. Setup Project:
### 2.1.1. Setup Data on MySQL via XAMPP

In the XAMPP Control Panel, run the Admin mode of MySQL after 'starting' MySQL by clicking the Admin button on the XAMPP Control Panel.

![](https://github.com/TruongLeDuy123/intern_assignment/blob/main/readme%20source/img/xampp3.png)

On the browser, with the URL localhost, the screen will appear as follows:

![](https://github.com/TruongLeDuy123/intern_assignment/blob/main/readme%20source/img/phpadmin1.png)

Create a new database with the following steps:
1. Select "Mới", then enter the database name and choose "Tạo" to create a new Database.

![](https://github.com/TruongLeDuy123/intern_assignment/blob/main/readme%20source/img/phpadmin2.png)

2. After successfully creating the database, select the SQL item on the taskbar to import the data file downloaded from (https://drive.google.com/file/d/17pX4tQc3gcno2J1r1P4EzyMucTg8AO45/view?usp=sharing). Then, select "Thực hiện" to execute the SQL commands.

![](https://github.com/TruongLeDuy123/intern_assignment/blob/main/readme%20source/img/phpadmin3.png)

The database, after being successfully imported, will have a structure with 6 tables as follows:

![](https://github.com/TruongLeDuy123/intern_assignment/blob/main/readme%20source/img/phpadmin4.png)

### 2.1.2. Setup Source Code of the Project

Clone the project from the team's Github Repository: [Intern_Assignment](https://github.com/TruongLeDuy123/intern_assignment)

![](https://github.com/TruongLeDuy123/intern_assignment/blob/main/readme%20source/img/setup1.png)

### 2.1.3. Setup file .env
Rename the .env.example file to .env. Then, add a few more parameters as follows:
- **MAIL_MAILER**=smtp
- **MAIL_HOST**=smtp.gmail.com
- **MAIL_PORT**=587
- **MAIL_USERNAME**=your_email
- **MAIL_PASSWORD**="your_password"
- **MAIL_ENCRYPTION**=tls
- **MAIL_FROM_ADDRESS**="your_email"
- **MAIL_FROM_NAME**="${APP_NAME}"
- **WEATHER_API_KEY:** get API from https://www.weatherapi.com (Create a new account and get a new api key)

To get Mail Password, you can:
1. Create a gmail account OR login with the gmail account.
2. Go to your Google Account.
3. Select Security Tab.
4. Move to  "Signing in to Google", Setup the 2 Step Verification (You may need to sign in and verify your account) and make to ON and then you will get an options for App Password as shown below. Select App Passwords. You may need to sign in. 
![](https://github.com/TruongLeDuy123/intern_assignment/blob/main/readme%20source/img/step1.png)

5. At the bottom, choose Select app and choose the app you using and then Select device and choose the device you’re using and then Generate.
![](https://github.com/TruongLeDuy123/intern_assignment/blob/main/readme%20source/img/step2.png)

On Select app: Select as Mail & on Select Device: Other (Custom Name) Eg: myWebsiteApplicationName.

6. Follow the instructions to enter the App Password. The App Password is the 16-character code in the yellow bar on your device.

![](https://github.com/TruongLeDuy123/intern_assignment/blob/main/readme%20source/img/step3.png)
Note: Copy your 16-Digital App Password and save it for your further use.
7. Tap Done.

## 2.2. Run the Web Application

In the VS Code Terminal, run the command 'php artisan serve' to start running the web application. The URL of the web application when started will be displayed on the terminal. Hold down the Ctrl key and click on the URL to open the web application in the browser.

![](https://github.com/TruongLeDuy123/intern_assignment/blob/main/readme%20source/img/setup2.png)

The web application after starting:

![](https://github.com/TruongLeDuy123/intern_assignment/blob/main/readme%20source/img/web1.png)

# Link demo
Access to this (https://drive.google.com/file/d/10LEg-9Zi3JUrQN0ggkx_7EELY5or9j0O/view?usp=sharing) for my demo
