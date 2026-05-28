

# 🍽️ Chirag Eatery - AI Food Ordering Chatbot

An AI-powered food ordering chatbot built using **FastAPI**, **Dialogflow**, and **MySQL**.

This chatbot allows users to:
- Place food orders
- Remove items from orders
- Track existing orders
- Automatically calculate total bills

---

# 🚀 Features

✅ AI-powered chatbot using Dialogflow  
✅ FastAPI backend API  
✅ MySQL database integration  
✅ Add/remove food items from orders  
✅ Track order status  
✅ Automatic total bill calculation  
✅ REST API webhook support  

---

# 🛠️ Tech Stack

- Python
- FastAPI
- Dialogflow
- MySQL
- Uvicorn
- REST APIs

---

# 📂 Project Structure

```bash
chirag-eatery-chatbot/
│
├── backend/
│   ├── db_helper.py
│   ├── generic_helper.py
│   ├── main.py
│   ├── requirements.txt
│   └── venv/
│
├── db/
│   └── chirag_eatery.sql
│
├── dialogflow_assets/
│   └── training_phrases.txt
│
├── frontend/
│   ├── home.html
│   ├── styles.css
│   ├── banner.jpg
│   ├── menu1.jpg
│   ├── menu2.jpg
│   └── menu3.jpg
│
└── README.md
```

---

# ⚙️ Installation

## 1️⃣ Clone Repository

```bash
git clone https://github.com/your-username/chirag-eatery-chatbot.git
```

---

## 2️⃣ Navigate to Project Folder

```bash
cd chirag-eatery-chatbot
```

---

## 3️⃣ Create Virtual Environment

```bash
python -m venv venv
```

### Activate Virtual Environment

#### Windows

```bash
venv\Scripts\activate
```

#### Linux / Mac

```bash
source venv/bin/activate
```

---

## 4️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

---

# 🗄️ Database Setup

## Create Database

```sql
CREATE DATABASE chirag_eatery;
```

---

## Import SQL File

```bash
mysql -u root -p chirag_eatery < chirag_eatery.sql
```

---

# 🔧 Configure Database Connection

Open `db_helper.py` and update MySQL credentials:

```python
cnx = mysql.connector.connect(
    host="localhost",
    user="root",
    password="YOUR_PASSWORD",
    database="chirag_eatery",
    auth_plugin='mysql_native_password'
)
```

---

# ▶️ Run FastAPI Server

```bash
uvicorn main:app --reload
```

Server will start on:

```bash
http://127.0.0.1:8000
```

---

# 🤖 Dialogflow Setup

1. Create a Dialogflow agent
2. Create intents using training phrases from:

```bash
dialogflow_assets/training_phrases.txt
```

3. Enable webhook
4. Add webhook URL:

```bash
http://your-server-url/
```

---

# 📌 Available Food Items

- Pizza
- Pav Bhaji
- Chole Bhature
- Mango Lassi
- Masala Dosa
- Biryani
- Vada Pav
- Rava Dosa
- Samosa

---

# 💬 Example Commands

## Place Order

```text
I want 2 pizzas and 1 mango lassi
```

## Remove Item

```text
Remove pizza from my order
```

## Track Order

```text
Track my order
```

---



# 📈 Future Improvements

- Payment gateway integration
- Live order tracking
- Admin dashboard
- User authentication
- Docker deployment
- Cloud deployment

---

# 👨‍💻 Author

## Chirag Verma

- LinkedIn: https://linkedin.com/in/chiragverma565

---

# ⭐ Support

If you like this project, give it a ⭐ on GitHub.

---
