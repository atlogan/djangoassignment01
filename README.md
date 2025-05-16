# Student Enrollment System

This Django-based Student Enrollment System helps educational institutions manage student records, course enrollments, and academic information efficiently.

## Prerequisites

- Python 3.8 or higher
- PostgreSQL database
- Git

## Project Setup

### 1. Clone the Repository

```bash
git clone https://github.com/atlogan/djangoassignment01
cd djangoassignment01
```

### 2. Create and Activate Virtual Environment

For Linux/macOS:
```bash
python -m venv venv
source venv/bin/activate
```

For Windows (PowerShell):
```powershell
PS> python -m venv venv
PS> .\venv\Scripts\Activate
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Environment Configuration

1. Create a `.env` file in the project root:
   ```bash
   cp .env.example .env
   ```

2. Open `.env` and update the following settings with your database credentials:
   ```
   SECRET_KEY=your_secret_key_here
   DEBUG=True
   DATABASE_URL=your_database_url
   ```

### 5. Database Setup

1. Apply migrations:
   ```bash
   python manage.py migrate
   ```

2. Create a superuser:
   ```bash
   python manage.py createsuperuser
   ```
   Follow the prompts to set username, email, and password.

### 6. Run Development Server

```bash
python manage.py runserver
```

The application will be available at `http://127.0.0.1:8000/`

Access the admin interface at `http://127.0.0.1:8000/admin/` using your superuser credentials.

## Project Structure

- `myapp/` - Main application directory containing models, views, and templates
- `mysite/` - Project configuration directory
- `requirements.txt` - Project dependencies
- `manage.py` - Django's command-line utility for administrative tasks

## Technology Stack

- Django 5.2.1
- PostgreSQL (via psycopg2-binary)
- django-environ 0.12.0 