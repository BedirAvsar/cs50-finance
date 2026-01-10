# CS50 Finance

A web-based stock trading simulator built with Python, Flask, and SQLite for Harvard’s CS50x course.

## 📺 Video Demo
TBA — Coming soon

## 📘 Description

CS50 Finance is a fully functional mini stock trading platform that allows users to register, log in, get real stock quotes, buy and sell shares, manage their portfolio, and view transaction history.

The project integrates:

- Real-time stock price lookup (via API)
- SQLite database for user accounts and transactions
- Secure user authentication
- Input validation and error handling
- Session management
- Dynamic portfolio calculation

This project replicates the core logic of an online brokerage system in a simplified and educational way.

---

## 🧩 Features

### ✔ User Authentication
- Register new accounts
- Secure password hashing
- Login/logout
- Session-based user tracking

### ✔ Quote Lookup
Users can search for real-time stock prices using an external API.

### ✔ Buy & Sell Stocks
- Validate symbol
- Validate shares
- Prevent invalid/negative values
- Update cash balance
- Insert transaction records

### ✔ Portfolio Overview
- Display current holdings
- Live price updates
- Total market value
- Available cash
- Grand total value

### ✔ Transaction History
- Timestamped logs
- Buy and sell operations
- Price + share amount

---

## 🗂 Project Structure
finance/
│
├── app.py              # Main Flask route handlers
├── helpers.py          # API lookup + custom utilities
├── finance.db          # SQLite database
│
├── static/
│   ├── styles.css
│   ├── favicon.ico
│
└── templates/
├── layout.html
├── index.html
├── quote.html
├── quoted.html
├── buy.html
├── sell.html
├── history.html
├── register.html
├── login.html
├── apology.html

---

## 💡 What I Learned

Developing CS50 Finance improved several key backend engineering skills:

- Flask routing, templates, sessions
- Using SQLite and SQL queries safely
- API integration and JSON parsing
- Server-side input validation
- Designing relational database schemas
- Managing state and persistent data
- Handling edge cases and user errors
- Debugging backend logic

This project strengthened my understanding of backend architecture and web application logic.

---

## ▶️ How to Run Locally

1. Install dependencies:
pip install -r requirements.txt

2. Start Flask server:
flask run

3. Visit in browser:
http://127.0.0.1:5000/
---

## 📜 Notes

This project is based on Harvard CS50x Week 9 (Flask), but heavily customized and extended by me.

---
