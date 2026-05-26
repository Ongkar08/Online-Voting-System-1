# Online Voting System

> A Java-based web application for conducting secure, transparent, and tamper-proof elections online.

## What is this?

Most voting systems are either paper-based or overly complex enterprise tools.
This project is a lightweight, full-stack Java application that brings the core
of a real election system — voter registration, admin control, live results —
into a clean, deployable web app.

---

## How it works

```
Voter                          Admin
  |                              |
  | Register / Login             | Login to Admin Panel
  |                              |
  | Browse Candidates            | Add Candidates
  |                              | Create Elections
  | Cast Vote                    | Monitor Progress
  |                              |
  | View Results                 | View Final Results
  |                              |
  └──────────── MySQL DB ────────┘
               (via JDBC)
```

---

## Stack

```
Frontend   →   HTML, CSS
Backend    →   Java, Java Servlets
Database   →   MySQL (JDBC)
Server     →   Apache Tomcat
```

---

## Run it locally

**Requirements**
- JDK installed
- Apache Tomcat
- MySQL

**Steps**

```bash
# 1. Clone
git clone https://github.com/Ongkar08/online-voting-system.git

# 2. Set up database
mysql -u root -p < schema.sql

# 3. Update DB config
# Edit db.properties with your MySQL credentials

# 4. Deploy
# Copy the .war file to Tomcat's webapps/ folder

# 5. Start Tomcat and open
# http://localhost:8080/online-voting-system
```

---

## Roles

**Voter**
- Register with credentials
- Log in and cast one vote per election
- View results once voting closes

**Admin**
- Create and manage elections
- Add and remove candidates
- Monitor live voting stats
- Ensure data integrity

---

## Security

- Password-based authentication for all users
- Role-based access control (voter vs admin)
- SQL constraints prevent duplicate or invalid votes
- All vote data stored securely in MySQL

---

## What's next

- [ ] 2FA — OTP-based login for voters
- [ ] Blockchain — immutable vote ledger
- [ ] Better UI — modern, responsive design overhaul

---

## Author

**Ongkar Pal** — [GitHub](https://github.com/Ongkar08) · [LinkedIn](https://linkedin.com/in/ongkarpal03) · [Codolio](https://codolio.com/profile/Ongkar08)
