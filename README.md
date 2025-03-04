# Task Manager App

A lightweight Flask application for organizing tasks with user authentication.

## Features

- User registration and login
- Create, read, update, and delete tasks
- User authentication with Flask-Login
- Password hashing with Flask-Bcrypt
- SQLite database for storing user and task data

## Setup

1. Clone the repository:
    ```sh
    git clone https://github.com/2arry/task_manager.git
    cd task_manager
    ```

2. Create a virtual environment and activate it:
    ```sh
    python -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    ```

3. Install the required packages:
    ```sh
    pip install -r requirements.txt
    ```

4. Create the SQLite database:
    ```sh
    python
    >>> from app import db
    >>> db.create_all()
    >>> exit()
    ```

5. Run the Flask app:
    ```sh
    python app.py
    ```

6. Open your web browser and navigate to `http://127.0.0.1:5000`.

## Directory Structure

```
task_manager/
│
├── app.py
├── config.py
├── forms.py
├── models.py
├── routes.py
├── templates/
│   ├── base.html
│   ├── index.html
│   ├── login.html
│   └── register.html
└── README.md
```

## License

This project is licensed under the MIT License.
