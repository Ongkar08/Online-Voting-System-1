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
