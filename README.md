# *TaskFlow*

**TaskFlow** is a Flask-based web application designed to manage user authentication and task management. It integrates with a MySQL database to store user credentials and task details.

## 🚀 Features

* User Registration and Login
* Secure Password Hashing
* Task Creation and Management
* Responsive Frontend with HTML/CSS
* Modular Code Structure using Blueprints

## 🗂️ Project Structure

```
full_extraction/
├── backend/
│   ├── __init__.py
│   ├── auth.py
│   ├── routes.py
│   └── templates/
│       ├── login.html
│       ├── signup.html
│       └── dashboard.html
├── config/
│   ├── __init__.py
│   └── db_config.py
├── run.py
└── requirements.txt
```

* `backend/`: Contains the main application logic and route definitions.
* `config/`: Holds configuration files, including database connection settings.
* `templates/`: HTML templates for rendering frontend pages.
* `run.py`: Entry point to start the Flask application.
* `requirements.txt`: Lists all Python dependencies.

## 🛠️ Installation

### Prerequisites

* Python 3.x
* MySQL Server

### Steps

1. **Clone the Repository**

   ```bash
   git clone https://github.com/yourusername/TaskFlow.git
   cd TaskFlow
   ```

2. **Set Up Virtual Environment**

   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install Dependencies**

   ```bash
   pip install -r requirements.txt
   ```

4. **Configure the Database**

   * Create a MySQL database named `taskflow`.
   * Update `config/db_config.py` with your MySQL credentials:

     ```python
     db_config = {
         'host': 'localhost',
         'user': 'your_username',
         'password': 'your_password',
         'database': 'taskflow'
     }
     ```

5. **Initialize the Database**

   * Run the SQL script provided in `database/schema.sql` to create necessary tables.

6. **Run the Application**

   ```bash
   python run.py
   ```

   Access the application at `http://127.0.0.1:5000/`.

## 🔐 Environment Variables

For enhanced security, especially in production, consider using environment variables to store sensitive information like the secret key and database credentials.

