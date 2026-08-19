# ATM Interface using Flask

A web-based ATM simulation built with **Python, Flask, SQLite, HTML, CSS and Jinja2**. The project demonstrates core web-application concepts including authentication, session-based workflows, database-backed transactions and server-side template rendering.

## Overview

The application simulates common ATM operations through a browser-based interface:

- User login and logout
- Balance inquiry
- Cash deposits
- Cash withdrawals
- Transaction history
- Session-based user workflows

## Architecture

```text
Browser
   ↓
Flask Routes
   ↓
Application Logic
   ↓
SQLite Database
   ↓
Transaction / Account Data
```

The repository documentation describes Flask routes for authentication, dashboard access, deposits, withdrawals, balance checks and transaction history. fileciteturn9file0

## Tech Stack

- Python
- Flask
- SQLite
- Jinja2
- HTML / CSS

## Project Structure

```text
ATM-Interface-using-Flask-Framework/
├── app.py
├── setup_db.py
├── models.py
├── requirements.txt
├── templates/
│   ├── index.html
│   ├── login.html
│   └── dashboard.html
├── static/
│   └── styles.css
└── README.md
```

> The structure above reflects the project's existing README documentation. fileciteturn9file0

## Getting Started

### 1. Clone

```bash
git clone https://github.com/Jaswanth170/ATM-Interface-using-Flask-Framework.git
cd ATM-Interface-using-Flask-Framework
```

### 2. Create a virtual environment

```bash
python -m venv .venv
```

macOS / Linux:

```bash
source .venv/bin/activate
```

Windows:

```powershell
.venv\Scripts\activate
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Initialize the database

```bash
python setup_db.py
```

### 5. Run the application

```bash
python app.py
```

Then open:

```text
http://127.0.0.1:5000/
```

## API Routes

| Route | Method | Purpose |
|---|---|---|
| `/` | GET | Home page |
| `/login` | GET/POST | User authentication |
| `/logout` | GET | End session |
| `/dashboard` | GET | Account dashboard |
| `/deposit` | POST | Deposit funds |
| `/withdraw` | POST | Withdraw funds |
| `/balance` | GET | View balance |
| `/history` | GET | View transaction history |

These routes are documented by the repository's existing project specification. fileciteturn9file0

## Security Note

This is an educational ATM simulation and should **not** be treated as production banking software. A production financial application would require stronger controls such as secure password hashing, CSRF protection, authorization checks, transaction integrity, audit logging, secret management, rate limiting, secure cookie configuration and comprehensive security testing.

## Future Improvements

- Add automated tests for account and transaction flows.
- Add stronger input validation and error handling.
- Add CSRF protection and secure authentication practices.
- Add database migrations.
- Add Docker support.
- Add CI checks with GitHub Actions.
- Improve accessibility and responsive UI.

## Author

**Jaswanth ST**  
GitHub: [@Jaswanth170](https://github.com/Jaswanth170)
