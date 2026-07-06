# 🚀 Flask Blog Application

<p align="center">
  <img src="https://img.shields.io/badge/Flask-3.x-000000?style=for-the-badge&logo=flask&logoColor=white">
  <img src="https://img.shields.io/badge/Python-3.13+-3776AB?style=for-the-badge&logo=python&logoColor=white">
  <img src="https://img.shields.io/badge/SQLite-Database-003B57?style=for-the-badge&logo=sqlite&logoColor=white">
  <img src="https://img.shields.io/badge/Jinja2-Templates-B41717?style=for-the-badge">
  <img src="https://img.shields.io/badge/Docker-Ready-2496ED?style=for-the-badge&logo=docker&logoColor=white">
</p>

<p align="center">
A modern Flask blog application featuring authentication, CRUD operations, SQLite integration, and reusable Jinja templates.
</p>

---

# ✨ Features

✅ User Registration

✅ User Login & Logout

✅ Session Authentication

✅ Create Posts

✅ Edit Posts

✅ Delete Posts

✅ SQLite Database

✅ Responsive UI

✅ Bootstrap 5 Styling

✅ Docker Support

---

# 🛠️ Tech Stack

| Technology | Purpose |
|------------|---------|
| 🐍 Python | Backend |
| 🌶 Flask | Web Framework |
| 🗄 SQLite | Database |
| 🎨 Bootstrap 5 | UI Design |
| 📄 Jinja2 | Templates |
| 🐳 Docker | Containerization |

---

# 📂 Project Structure

```text
Flask-app/
│
├── app.py
├── dockerfile
├── pyproject.toml
├── README.md
│
├── flaskr/
│   ├── __init__.py
│   ├── auth.py
│   ├── blog.py
│   ├── db.py
│   ├── schema.sql
│   │
│   ├── static/
│   │   ├── style.css
│   │   ├── create.css
│   │   └── posts.css
│   │
│   └── templates/
│       ├── base.html
│       ├── auth/
│       │   ├── login.html
│       │   └── register.html
│       └── blog/
│           ├── create.html
│           ├── update.html
│           └── index.html
│
└── instance/
```

---

# 🌐 Application Routes

## 🏠 Home

| Method | Route | Description |
|---------|-------|-------------|
| GET | `/` | Blog Homepage |
| GET | `/hello` | Hello Flask Example |

---

## 🔐 Authentication

| Method | Route |
|---------|-------|
| GET / POST | `/auth/register` |
| GET / POST | `/auth/login` |
| GET | `/auth/logout` |

---

## 📝 Blog

| Method | Route |
|---------|-------|
| GET / POST | `/create` |
| GET / POST | `/<int:id>/update` |
| POST | `/<int:id>/delete` |

---

# ⚙️ Installation

## 1️⃣ Clone the Repository

```bash
git clone https://github.com/yourusername/flask-app.git
```

```bash
cd flask-app
```

---

## 2️⃣ Create Virtual Environment

Windows

```bash
python -m venv venv
```

```bash
venv\Scripts\activate
```

Linux / macOS

```bash
python3 -m venv venv
```

```bash
source venv/bin/activate
```

---

## 3️⃣ Install Dependencies

```bash
pip install -e .
```

---

## 4️⃣ Initialize Database

```bash
flask --app flaskr init-db
```

---

## 5️⃣ Run the Server

```bash
flask --app flaskr run --debug
```

Visit

```
http://127.0.0.1:5000
```

---

# 🐳 Docker

Build

```bash
docker build -f dockerfile -t flask-app .
```

Run

```bash
docker run --rm -p 5000:5000 flask-app
```

---

# 🗄 Database

The project uses **SQLite**.

Database schema:

```
flaskr/schema.sql
```

The generated database is stored inside:

```
instance/
```

---

# 👨‍💻 Author

**Ahmad**

📧 Email: irsheidahmad094@gmail.com

💼 GitHub: https://github.com/Ahmad-IR122

---

# ⭐ Support

If you found this project useful, consider giving it a ⭐ on GitHub.

---
