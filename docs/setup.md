# Setup

Follow these steps to set up the Task Manager App:

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