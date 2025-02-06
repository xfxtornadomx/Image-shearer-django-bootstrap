# Django Project Setup

This guide will walk you through the steps to set up and run the Django development server on port `8000`.

---

## Table of Contents

1. [Prerequisites](#prerequisites)
2. [Installation](#installation)
3. [Running the Django Server](#running-the-django-server)
4. [Stopping the Server](#stopping-the-server)
5. [Additional Commands](#additional-commands)
6. [Troubleshooting](#troubleshooting)
7. [Support](#support)

---

## Prerequisites

Before you begin, ensure you have the following installed:

- **Python 3.x**: Download and install Python from [python.org](https://www.python.org/downloads/).
- **pip**: Python's package manager (usually comes pre-installed with Python).

---

## Installation

### 1. Clone the Repository

If you haven't already, clone the repository to your local machine:

```bash
git clone https://github.com/xfxtornadomx/Image-shearer-django-bootstrap.git
cd your-repo
```

### 2. Set Up a Virtual Environment (Optional but Recommended)

Create and activate a virtual environment to isolate dependencies:

#### On macOS/Linux:

```bash
python -m venv venv
source venv/bin/activate
```

#### On Windows:

```bash
python -m venv venv
venv\Scripts\activate
```

### 3. Install Dependencies

Install the required Python packages using pip:

```bash
pip install -r requirements.txt
```

---

## Running the Django Server

### 1. Apply Database Migrations

Run the following command to apply any pending database migrations:

```bash
python manage.py migrate
```

### 2. Run the Development Server

Start the Django development server on port 8000:

```bash
python manage.py runserver 8000
```

### 3. Access the Application

Open your web browser and navigate to:

```
http://127.0.0.1:8000/
```

You should see the Django application running.

---

## Stopping the Server

To stop the development server, press `Ctrl + C` in the terminal where the server is running.

---

## Additional Commands

### Create a Superuser

To access the Django admin panel, create a superuser:

```bash
python manage.py createsuperuser
```

Follow the prompts to set a username, email, and password.

### Run Tests

To run the project's test suite:

```bash
python manage.py test
```

### Collect Static Files

If your project uses static files, run:

```bash
python manage.py collectstatic
```

---

## License

This project is licensed under the MIT License.
