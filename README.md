# 📈 Stock Trading Simulator  
*A web-based stock trading platform that simulates real-world brokerage operations including portfolio management, transactions, and real-time price retrieval.*

![Python](https://img.shields.io/badge/Python-3.x-blue)
![Flask](https://img.shields.io/badge/Flask-Web%20Framework-black)
![SQLite](https://img.shields.io/badge/SQLite-Database-lightgrey)
![HTML](https://img.shields.io/badge/Frontend-HTML%2FCSS-orange)

---

## The 'Why' & Real-World Use Case

Financial systems require accurate transaction handling, data consistency, and real-time data integration. This project simulates a simplified brokerage system, focusing on how users interact with financial assets such as stocks.

The application demonstrates core backend responsibilities such as **stateful user sessions, transactional integrity, portfolio tracking, and external API integration**, all of which are fundamental in fintech systems.

---

## Architecture & Technical Decisions

- **MVC-Inspired Structure**
  - `app.py` → routing & business logic
  - `templates/` → presentation layer (Jinja2)
  - `helpers.py` → reusable utilities

- **Server-Side Rendering**
  - Uses Flask + Jinja2 instead of SPA frameworks
  - Keeps logic simple and backend-focused

- **Database Design (SQLite)**
  - Users, transactions, and portfolio tracking
  - Ensures consistency in buy/sell operations

- **Session Management**
  - Flask session handling for authentication
  - Secure login system with hashed passwords

- **External API Integration**
  - Fetches real-time stock prices
  - Handles API failures and invalid inputs gracefully

- **Input Validation & Data Integrity**
  - Prevents invalid transactions
  - Ensures balance consistency

---

## Tech Stack

- **Backend:** Python, Flask  
- **Database:** SQLite  
- **Frontend:** HTML, CSS (Jinja2 templates)  
- **Authentication:** Session-based (Flask)  
- **Other:** CS50 helpers, external stock API  

---

## Getting Started

### Clone the repository
```bash id="3fd92k"
git clone https://github.com/BedirAvsar/stock-trading-simulator.git
cd stock-trading-simulator
```

### Create virtual environment
```bash id="92kds1"
python -m venv venv
source venv/bin/activate   # macOS / Linux
venv\Scripts\activate      # Windows
```

### Install dependencies
```bash id="kd02jd"
pip install -r requirements.txt
```

### Run the application
```bash id="p92md1"
flask run
```

---

## Usage / API Endpoints

This is a server-rendered web application.

### Core Features

| Feature | Description |
|--------|------------|
| Register/Login | User authentication system |
| Quote | Fetch real-time stock price |
| Buy | Purchase stock with balance validation |
| Sell | Sell owned stocks |
| Portfolio | View holdings and total balance |
| History | Transaction history |

### Example Flow

1. Register a new account  
2. Login  
3. Search stock symbol (e.g., AAPL)  
4. Buy shares  
5. View portfolio updates  
6. Sell shares  

---

## What I Learned

This project reflects a transition from simple scripting to **stateful backend system design**.

### Key Takeaways

- Designing a **transaction-based system**
- Handling **data consistency in financial operations**
- Working with **Flask request/response lifecycle**
- Implementing **authentication & session management**
- Integrating **external APIs reliably**

### Biggest Challenge

The most challenging part was ensuring **correct financial state management**, especially keeping user balance and stock holdings consistent across multiple transactions while preventing invalid operations.

---

This project demonstrates the ability to build a **real-world backend system**, focusing on correctness, structure, and maintainability rather than just functionality.
