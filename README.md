# Sports Gym Management System

A comprehensive gym management system built with PHP and MySQL, designed to help gym owners manage their facilities, members, and activities efficiently.

## Features

- User Management (Admin/Member roles)
- Session Booking System
- Equipment Management
- Event Management
- Achievement Tracking
- System Updates/Announcements
- Responsive Design

## Requirements

- XAMPP (Apache, MySQL, PHP)
- PHP 7.4 or higher
- MySQL 5.7 or higher
- Web browser (Chrome, Firefox, Safari, etc.)

## Installation Steps

1. **Install XAMPP**
   - Download and install XAMPP from [https://www.apachefriends.org/](https://www.apachefriends.org/)
   - Start Apache and MySQL services from XAMPP Control Panel

2. **Clone/Download Project**
   - Clone this repository or download the ZIP file
   - Extract the files to `C:\xampp\htdocs\sports-gym-management`

3. **Database Setup**
   - Open your web browser and go to `http://localhost/phpmyadmin`
   - Create a new database named `sports_gym_db`
   - Import the database file from `database/sports_gym_db.sql`
   - Click on the "Import" tab
   - Choose the file `sports_gym_db.sql`
   - Click "Go" to import the database

4. **Configure Database Connection**
   - Open `config/db_connect.php`
   - Verify the database credentials:
     ```php
     $host = 'localhost';
     $dbname = 'sports_gym_db';
     $username = 'root';
     $password = '';
     ```
   - These are the default XAMPP credentials, no changes needed if using default setup

5. **Access the Application**
   - Open your web browser
   - Go to `http://localhost/sports-gym-management`
   - Default admin credentials:
     - Username: `admin`
     - Password: `password`

## Project Structure

```
sports-gym-management/
├── assets/
│   ├── css/
│   ├── js/
│   └── images/
├── config/
│   └── db_connect.php
├── database/
│   └── sports_gym_db.sql
├── partials/
│   ├── header.php
│   └── footer.php
├── pages/
│   ├── admin/
│   │   ├── admin_dashboard.php
│   │   ├── admin_equipment.php
│   │   ├── admin_events.php
│   │   ├── admin_sessions.php
│   │   └── admin_users.php
│   ├── equipment.php
│   ├── events.php
│   ├── login.php
│   ├── profile.php
│   ├── register.php
│   └── sessions.php
├── index.php
└── README.md
```

## Troubleshooting

1. **Database Connection Issues**
   - Ensure MySQL service is running in XAMPP
   - Verify database credentials in `config/db_connect.php`
   - Check if database `sports_gym_db` exists

2. **Page Not Found**
   - Verify files are in the correct directory
   - Check Apache configuration in XAMPP
   - Ensure proper file permissions

3. **Login Issues**
   - Clear browser cache
   - Try using the default admin credentials
   - Check if session is enabled in PHP
