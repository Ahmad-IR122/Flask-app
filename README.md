# Flask Blog Application

A modern Flask blog app with user authentication, SQLite persistence, and clean Jinja2 templates.

## Highlights

- User registration and login/logout
- Session-based authentication
- Full blog CRUD (create, edit, delete)
- SQLite database with schema initialization
- Responsive HTML/CSS templates
- Docker support for containerized runs

## Tech Stack

- Python 3.13+
- Flask 3.x
- SQLite
- Jinja2
- HTML/CSS
- Docker

## Repository Structure

```text
Flask-app/
├── app.py
├── dockerfile
├── pyproject.toml
├── flaskr/
│   ├── __init__.py
│   ├── auth.py
│   ├── blog.py
│   ├── db.py
│   ├── schema.sql
│   ├── static/
│   └── templates/
└── instance/
```

## Quick Start

### 1) Clone

```bash
git clone https://github.com/Ahmad-IR122/Flask-app.git
cd Flask-app
```

### 2) Create virtual environment

**Windows (PowerShell)**

```powershell
python -m venv venv
venv\Scripts\Activate.ps1
```

**macOS/Linux**

```bash
python3 -m venv venv
source venv/bin/activate
```

### 3) Install dependencies

```bash
pip install -e .
```

### 4) Initialize database

```bash
flask --app flaskr init-db
```

### 5) Run the app

```bash
flask --app flaskr run --debug
```

Open your browser at:

```text
http://127.0.0.1:5000
```

## Main Routes

### General

- `GET /` — Blog homepage
- `GET /hello` — Example hello endpoint

### Authentication

- `GET, POST /auth/register`
- `GET, POST /auth/login`
- `GET /auth/logout`

### Blog

- `GET, POST /create`
- `GET, POST /<int:id>/update`
- `POST /<int:id>/delete`

## Docker

Build image:

```bash
docker build -f dockerfile -t flask-app .
```

Run container:

```bash
docker run --rm -p 5000:5000 flask-app
```

## Database Notes

- Schema file: `flaskr/schema.sql`
- SQLite DB file is created in: `instance/`

## Author

**Ahmad**

- GitHub: https://github.com/Ahmad-IR122
- Email: irsheidahmad094@gmail.com

## License

Add a `LICENSE` file (e.g., MIT) if you want to specify usage terms.

---

If this project helped you, consider giving it a ⭐ on GitHub.
