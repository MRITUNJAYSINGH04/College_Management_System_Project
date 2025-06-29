🎓 Complete College Management System in PHP & MySQL

Description:
A fully-featured web-based college management system built using PHP and MySQL. This project centralizes the core administrative functions of a college or school — from student enrollment and attendance to fees, hostel management, transport, library, and online communication.

✅ Free Download & Installation Guide Included

Features:

Student & Staff Management

Attendance Tracking

Fee Ledger and Online Payments

Hostel & Transport Administration

Library Resource Management

Assignment Upload & Submission

Front Desk & Visitor Logging

SMS & Email Alerts

Zoom Meeting Integration

CMS for News & Announcements

Role-Based Access Control (ACL)

Tech Stack:

Backend: PHP 7.1+

Database: MySQL

Frontend: HTML, CSS, Bootstrap, JavaScript, AJAX

Tools: Composer, Laravel Artisan, Node.js (optional)

System Modules:

Student & Staff Profiles

Academic Calendar & Exam Scheduling

Role Management (Admin, Teacher, Accountant, etc.)

Website CMS

Real-Time Notifications

Assignment Portal

Visitor Management System

Zoom Integration

Transport Routes

Attendance Reports

Fee Receipt Generation

System Requirements:

PHP 7.1 or higher

Apache / Nginx with mod_rewrite

MySQL

PHP Extensions: openssl, pdo, mbstring, tokenizer, json, curl

Composer (for dependency management)

Node.js (for asset builds - optional)

Installation Guide:

Unzip the project into your web root (e.g., xampp/htdocs)

Create a .env file and configure:

APP_NAME=EduFirm
APP_ENV=local
APP_DEBUG=true
APP_URL=http://localhost

DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=college
DB_USERNAME=root
DB_PASSWORD=

Database Setup

Method 1 (Using Seeder):

Go to database/seeds/UsersTableSeeder.php

Set your admin name, email, and password

Run the following command in terminal:
php artisan migrate --seed

Method 2 (Manual Import):

Create a database named college in phpMyAdmin

Import the SQL file

Default login:
Email: superadmin@edufirm.com
Password: admin

Create an .htaccess file at the root with:

<IfModule mod_rewrite.c> RewriteEngine On RewriteRule ^(.*)$ public/$1 [L] </IfModule>
Delete any existing config cache:
bootstrap/cache/config.php

Visit your hosted URL

Login using Super Admin credentials (see Step 3)

Admin Login Details:

Email: superadmin@edufirm.com
Password: admin

FAQs:

Is this scalable for universities?
→ Yes, it’s scalable with proper optimization and server setup.

Can I use Nginx instead of Apache?
→ Yes, just configure proper rewrite rules.

Can I add more payment gateways?
→ Yes, integrate PayPal, Stripe, or Razorpay as needed.

Can I add more user roles?
→ Yes, ACL allows custom roles like HoD, Accountant, Librarian.

Can this integrate with an LMS?
→ Yes, via APIs or LTI depending on your LMS.

How do I secure this system?
→ Use strong passwords, SSL, updated PHP versions, and minimal DB privileges.

Conclusion:
The Complete College Management System in PHP & MySQL offers a unified, scalable platform for managing academics, administration, and financials in educational institutions. Say goodbye to spreadsheets and ledgers—go digital, go secure.

Feel free to fork this project, explore new features, and contribute improvements. For any help, refer to the installation steps or open an issue on GitHub.
