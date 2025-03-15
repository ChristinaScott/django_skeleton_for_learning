# Django Web App Skeleton for Learning

## Overview
This is a basic Django project structure intended for **exploring the default Django skeleton**. It provides a foundation for learning Django by allowing users to build upon its existing configuration. The project currently contains default settings but does not include any models, views, templates, or static files.

## Purpose
This repository is designed for **exploring the basic Django structure** and understanding how a Django project is set up. If you are new to Django, this setup can help you get started by adding apps, models, and views as you learn.

## Features
- Django-powered backend
- Basic project structure (settings, URL routing)
- No pre-built models, views, or templates

## Key Components of This Backend
### 1. `manage.py`
A command-line tool that helps manage the project. You use it for running the server, migrations, and other administrative tasks.

### 2. `config/settings.py`
Holds project settings such as database configuration, installed apps, middleware, and static file settings.

### 3. `config/urls.py`
Defines URL routing for the project. It maps incoming requests to specific views.

### 4. `wsgi.py` and `asgi.py`
These files allow the Django application to communicate with web servers like Gunicorn or Daphne for deployment.

### 5. `requirements.txt`
Lists all dependencies needed to run the project. Use `pip install -r requirements.txt` to install them.

## Starting an App
If you want to add functionality to this project, you should start by creating a Django app:
1. **Create a new app:**
   ```bash
   python manage.py startapp myapp
   ```
2. **Register the app in `config/settings.py`:**
   ```python
   INSTALLED_APPS = [
       ...
       'myapp',
   ]
   ```
3. **Define models in `myapp/models.py`**
   - This is where you define database tables as Python classes.

4. **Create views in `myapp/views.py`**
   - Views handle user requests and return responses.

5. **Set up URLs in `myapp/urls.py` and include them in `config/urls.py`**
   - This allows Django to route incoming requests properly.

6. **Run migrations:**
   ```bash
   python manage.py makemigrations
   python manage.py migrate
   ```

7. **Start the development server and test your app!**

## Installation
### Prerequisites
Ensure you have the following installed on your system:
- Python (>=3.x)
- pip (Python package manager)
- virtualenv (recommended)

### Setup Steps
1. **Clone the repository:**
   ```bash
   git clone <repository_url>
   cd web_app
   ```
2. **Create and activate a virtual environment:**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   ```
3. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```
4. **Apply migrations:**
   ```bash
   python manage.py migrate
   ```
5. **Run the development server:**
   ```bash
   python manage.py runserver
   ```
6. **Access the application:**
   Open your browser and go to `http://127.0.0.1:8000/`.
   Since no views or templates are defined yet, you will likely see a default Django page.

## Next Steps
To add functionality to this project, you can:
- Create a new app using:
  ```bash
  python manage.py startapp myapp
  ```
- Define models in `models.py`
- Create views in `views.py`
- Add templates and static files

## Contributing
If you are using this for learning, feel free to experiment and modify it as needed. Contributions are welcome!

## License
This project is licensed under the MIT License. See `LICENSE` for details.

---

Happy coding and exploring Django! 🚀





