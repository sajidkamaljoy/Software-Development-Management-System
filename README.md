# Software Development Management System

A web app that supports a software team across the whole development process: project requests from clients, analysis, assignment, development, testing and documentation. Built with PHP, JavaScript and MySQL.

## Roles and what they do

| Role | Main screens |
|---|---|
| **Admin** | Register employees, assign people to work, approve pending leave requests |
| **Client** | Submit new project requirements and follow project titles and requests |
| **Manager** | Review project requests, assign developers and testers, schedule meetings, track work updates, handle leave |
| **Analyzer** | Work on requirements and prototypes, update requirements, request meetings |
| **Developer** | View assigned projects, upload completed work, request leave |
| **Tester** | Unit and integration test results, re-check requests |
| **Technical Writer** | Upload final documentation and post work updates |

## Structure

```
index.php          entry point
views/             pages per role (admin, Client, Manager, Analyzer, developer, Tester, TechnicalWriter)
models/            database access and business logic (db.php, projectinfomodel.php, taskinfomodel.php, ...)
models/controller/ request handlers
style/             CSS
assets/            prototypes, project documents and images
```

The code follows a simple MVC split.

## Tech stack

PHP, MySQL (`mysqli`), JavaScript, HTML and CSS.

## Run it locally

1. Install XAMPP, WAMP or any PHP and MySQL stack.
2. Copy the project into your web root (for example `htdocs/sdms`).
3. Create a MySQL database named `spma` and the tables the code expects (for example `projectinfo`, `taskinfo`, `meetinglist`). The SQL schema is not included in this repo.
4. Set your MySQL username and password in `models/db.php`.
5. Open `http://localhost/sdms/` in your browser.

## Credits

A team project. An earlier, file-based version of this system is in the `learning-web-technologies-fall2022-2023-sec-c` repo.
