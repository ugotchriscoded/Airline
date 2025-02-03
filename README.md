<p align="center"><a href="https://laravel.com" target="_blank"><img src="https://raw.githubusercontent.com/laravel/art/master/logo-lockup/5%20SVG/2%20CMYK/1%20Full%20Color/laravel-logolockup-cmyk-red.svg" width="400" alt="Laravel Logo"></a></p>

# ✈️ Airline 🗺

## :bulb:Project description

I developed a system for an **aircraft** that allows the comprehensive management of **users**, **flights**, **reservations** and **destinations** with advanced functionalities such as secure **authentication through JWT**, **automatic management** of flights without **available** seats or that have exceeded the **deadline**.

### Aircraft Management:
- **CRUD** of aircraft **ONLY** by the **Admin**.
- Planes have a **name** and the **max number** of **seats**.

### Flight Management:
- **CRUD** of flights **ONLY** by the **Admin**.
- The **flight** has: *date, place of departure, arrival place and an assigned plane*.
- Automatically change the **status** of the **available flight** to *"false"* when the flight **runs out** of **available seats** or is **out of date**.
  
### Reservation Management:
- Create **flight** reservations **ONLY** if the **selected route exists** and there are **seats available** and the **date has NOT passed**.
- You can **ONLY** make **1 reservation** **per flight**. If you have booked it, you can ONLY **cancel** it.
- If there is **NO reservation**, the **option** to **reserve** appears.
- **ONLY** **Users** can reserve, **Guest** can only **view**.
- **Availability check** BEFORE **confirming** a reservation.

### User Query:
- See the **flights book** to a flight or **delete** from a flight.
- **ONLY** reserve **1 seat per flight**.
- See all his **future reservations** as **past**.
  
### Administrator Query:
- See **who has booked** on a **specific flight**.

## Requirements:
- **User Management:** *registration, authentication and role management* **(ADMIN, USER and GUEST)**.
- Generation and validation of **JWT tokens** for **secure sessions**.
- **70%** min coverage
- **ALL functionalities** must exist in **REST API** and **verified by Postman**.
- **JIRA** should be used for **epic user stories** and **tasks**.
- Flight **list sheet** with the **date organized** from **closest to furthest**. Only those available on another screen are the **past flights**, including the total seats on the plane and the seats still free.
- **Reserve button** to reserve and cancel **(BLADE)**
- The **administrator** **CANNOT** make reservations.

## :eye_speech_bubble: Working app

(insert screenshoots)

## :file_folder: Jira Backlog

(insert screenshoots)

## :paperclip: Installation requirements
:black_circle: XAMPP

:black_circle: Composer

:black_circle: Node.js (Installing NPM)

:black_circle: Xdebug 

:black_circle: Postman

> [!NOTE] 
If you can't install XAPP, you can also use another local server that supports MySQL and PHP.

## :scroll: Installation

### Step 1: Creating database

Creating a database in **Admin** **SQL**.

(insert screenshoot)

### Step 2: Cloning repository

```php
https://github.com/ugotchriscoded/Tolls-and-Vehicles
 ```

 ### Step 3: Putting everything up to date

In the *.env* file **remove** the *#* in these lines, enter the **name** of your **database** and **replace** *Laravel* with *sql*.

<p align="center"><img width="287" alt="image" src="https://github.com/user-attachments/assets/bdfec806-cdcc-4a05-a6bf-43a59cc7658e"></p>

### Server

To **run the server** enter this command:

```php
npm run dev
```

(insert screenshoot)

> [!WARNING]
> **DON'T work** on that terminal again, but you should keep it working. **DON'T KILL IT.**

To see the **running serve** enter the command:

```php
php artisan serve
```
(insert screenshoot)


> [!NOTE]
> If you press Control and click the link it should take you to the main offers.

## 📝 Documentation (Endpoints)


## :white_check_mark: Tests

> [!IMPORTANT]
>  Testing the project so we can check if it works correctly using this command:

```php
./vendor/bin/phpunit tests
```
(insert screenshoot)

### Coverage

Use this command:

```php
php artisan test --coverage
```

(insert screenshoot)

## Authors
Developed by **Valeria Dobado Gonzalez**:
- **Github**: *https://github.com/ugotchriscoded/ugotchriscoded*
- **Linkendin**: *https://www.linkedin.com/in/valeria-dobado-gonzález-262060328/*
  
## Languages
<a href='https://github.com/shivamkapasia0' target="_blank"><img alt='php' src='https://img.shields.io/badge/php-100000?style=for-the-badge&logo=php&logoColor=white&labelColor=000000&color=000000'/></a>
<a href='https://github.com/shivamkapasia0' target="_blank"><img alt='css3' src='https://img.shields.io/badge/css3-100000?style=for-the-badge&logo=css3&logoColor=white&labelColor=000000&color=000000'/></a>
<a href='https://github.com/shivamkapasia0' target="_blank"><img alt='json' src='https://img.shields.io/badge/JSON-100000?style=for-the-badge&logo=json&logoColor=white&labelColor=000000&color=000000'/></a>

## Tools
<a href='https://github.com/shivamkapasia0' target="_blank"><img alt='github' src='https://img.shields.io/badge/github-100000?style=for-the-badge&logo=github&logoColor=white&labelColor=000000&color=000000'/></a>
<a href='https://github.com/shivamkapasia0' target="_blank"><img alt='Laravel' src='https://img.shields.io/badge/Laravel-100000?style=for-the-badge&logo=Laravel&logoColor=white&labelColor=000000&color=000000'/></a>
<a href='https://github.com/shivamkapasia0' target="_blank"><img alt='Git' src='https://img.shields.io/badge/git-100000?style=for-the-badge&logo=Git&logoColor=white&labelColor=000000&color=000000'/></a>
<a href='https://github.com/shivamkapasia0' target="_blank"><img alt='MySql' src='https://img.shields.io/badge/my_sql-100000?style=for-the-badge&logo=MySql&logoColor=white&labelColor=000000&color=000000'/></a>
<a href='https://github.com/shivamkapasia0' target="_blank"><img alt='xampp' src='https://img.shields.io/badge/xampp-100000?style=for-the-badge&logo=xampp&logoColor=white&labelColor=000000&color=000000'/></a>
<a href='https://github.com/shivamkapasia0' target="_blank"><img alt='xampp' src='https://img.shields.io/badge/postman-100000?style=for-the-badge&logo=xampp&logoColor=white&labelColor=000000&color=000000'/></a>
<a href='https://github.com/shivamkapasia0' target="_blank"><img alt='Jira' src='https://img.shields.io/badge/Jira-100000?style=for-the-badge&logo=Jira&logoColor=white&labelColor=black&color=black'/></a>

## Thanks for reading!

Thanks for your attention, have a nice day! <3


