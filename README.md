# Stock Trading Simulator

A web-based stock trading simulator built with **Python**, **Flask**, and **SQLite**, replicating the core logic of an online brokerage system. This project was developed as part of Harvard’s CS50x and extended with additional backend improvements.

---

## 📸 Screenshots
_coming soon_

---

## 🚀 Features

### **User Authentication**
- Register/login/logout  
- Secure password hashing  
- Session-based user state

### **Stock Quote Lookup**
- Query real-time stock prices via API  
- Handles invalid symbols gracefully

### **Buying & Selling Stocks**
- Input validation  
- Balance updates  
- Transaction logging  
- Prevents invalid/negative share counts  

### **Portfolio Dashboard**
- Live prices  
- Total value calculation  
- Cash balance  
- Market value breakdown

### **Transaction History**
- Timestamped logs  
- Buy/sell operations  
- Share count + price tracking  

---

## 🗂 Project Structure

```
finance/
│
├── app.py              # Main Flask route handlers
├── helpers.py          # API lookup + utilities
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
```

---

## ⚙️ Installation & Setup

### 1️⃣ Clone the repo
```bash
git clone https://github.com/BedirAvsar/cs50-finance
cd cs50-finance
```

### 2️⃣ Create a virtual environment
```bash
python3 -m venv venv
source venv/bin/activate  # macOS/Linux
venv\Scripts\activate     # Windows
```

### 3️⃣ Install dependencies
```bash
pip install -r requirements.txt
```

### 4️⃣ Set your API key  
Create `.env` file:

```
API_KEY=your_api_key_here
```

### 5️⃣ Run the app
```bash
flask run
```

---

## 🧠 How It Works (Backend Flow)

1. User logs in → session created  
2. User searches stock quote → API request  
3. Buy/sell operation validated  
4. SQLite updates:
   - cash balance  
   - shares table  
   - transaction logs  
5. Portfolio recalculates live market value  
6. History stores all actions  

---

## 💡 What I Learned

This project strengthened several key backend skills:

- Flask routing, sessions, templates  
- SQL queries and database schema design  
- JSON parsing and API integration  
- Error handling & edge case management  
- Authentication logic and stateful design  
- Debugging request flow and logic consistency  

---

## 📄 Note
This project is based on Harvard CS50x Week 9 but includes custom improvements and refactoring.
