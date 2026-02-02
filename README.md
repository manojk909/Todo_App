# 📝 My TODO App (Flask)

A simple and clean **TODO web application** built using **Flask** and **Flask-SQLAlchemy**.  
This app allows users to **add, view, update, and delete TODO items**, with automatic date & time tracking.

---

## 🚀 Features

- Add TODO with **title** and **description**
- View all TODOs in a table format
- Automatic **date & time** creation
- Update existing TODOs
- Delete TODOs
- SQLite database (lightweight & file-based)
- Clean UI using **Bootstrap**
- Works seamlessly on **GitHub Codespaces**

---

## 🛠️ Tech Stack

- **Python 3**
- **Flask**
- **Flask-SQLAlchemy**
- **SQLite**
- **HTML / CSS / Bootstrap**

---

## 📂 Project Structure

```

Flask/
│
├── app.py
├── Procfile
├── requirements.txt
├── README.md
├── .gitignore
│
├── env/ # Virtual environment (ignored by git)
├── pycache/ # Python cache files
│
├── instance/
│ └── task.db # SQLite database
│
├── static/
│ ├── css/
│ │ └── style.css
│ └── js/
│ └── test.js
│
├── templates/
│ ├── base.html
│ ├── index.html
│ └── update.html
│
└── README.md
````

---

## ⚙️ Setup Instructions (Local / Codespaces)

### 1️⃣ Clone the repository
```bash
git clone <your-repository-url>
cd Flask
````

---

### 2️⃣ Create and activate a virtual environment

```bash
python -m venv env
source env/bin/activate
```

---

### 3️⃣ Install dependencies

```bash
pip install -r requirements.txt
```

---

### 4️⃣ Create database tables

```bash
python
```

```python
from app import app, db
with app.app_context():
    db.create_all()
```

Exit Python shell:

```bash
exit()
```

---

### 5️⃣ Run the application

```bash
python app.py
```

---

## 🌐 Access the Application

### 🔹 Local Machine

```
http://127.0.0.1:8000/
```

### 🔹 GitHub Codespaces

```
https://<your-codespace-name>-8000.app.github.dev/
```

### Routes

* `/` → Home page (Add TODO)
* `/show` → Display all TODOs

---

## 📸 Screenshot

<img width="1919" height="853" alt="image" src="https://github.com/user-attachments/assets/7bc5b6a2-519e-4bc9-9549-27d0cbc813fe" />


---

## 🧠 Learning Outcomes

* Flask routing and templates
* Application context in Flask
* SQLAlchemy ORM models
* CRUD operations
* Handling GET and POST requests
* Virtual environments and dependency management
* Working with GitHub Codespaces

---

## 🚧 Future Enhancements

* User authentication
* Mark TODO as completed
* Search & filter functionality
* Pagination
* REST API version
---

## 📄 License

This project is open-source and free to use for learning and educational purposes.
