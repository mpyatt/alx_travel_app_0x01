# 🧭 alx_travel_app_0x01

A Django-based API for managing travel listings and bookings, built with Django REST Framework and documented with Swagger.

## 📦 Project Structure

- `listings/` — App for Listings and Bookings models, views, serializers.
- `alx_travel_app/` — Main Django project configuration.
- `db.sqlite3` — SQLite database for local development.
- `requirements.txt` — Python dependencies.

## 🚀 Features

- CRUD operations for travel listings and bookings.
- RESTful API endpoints.
- Swagger UI documentation at `/swagger/`.
- SQLite for development (can be switched to MySQL).
- CORS and environment variable support.

## 📂 Endpoints

| Method | Endpoint         | Description               |
|--------|------------------|---------------------------|
| GET    | `/api/listings/` | List all listings         |
| POST   | `/api/listings/` | Create a new listing      |
| GET    | `/api/bookings/` | List all bookings         |
| POST   | `/api/bookings/` | Create a new booking      |

More available via the Swagger UI.

## 📄 Setup Instructions

### 1. Clone the Repository

```bash
git clone https://github.com/mpyatt/alx_travel_app_0x01.git
cd alx_travel_app_0x01/alx_travel_app
````

### 2. Create & Activate a Virtual Environment

```bash
python -m venv .venv
source .venv/bin/activate  # or .venv\Scripts\activate on Windows
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Run Migrations

```bash
python manage.py migrate
```

### 5. Run the Development Server

```bash
python manage.py runserver
```

Visit [http://127.0.0.1:8000/swagger/](http://127.0.0.1:8000/swagger/) for Swagger documentation.

## 🛠 Tech Stack

- Python 3.11+
- Django 4.2
- Django REST Framework
- drf-yasg (Swagger)
- SQLite (default) or MySQL (optional)
- Celery (optional for background tasks)

## ✅ Todo

- Add authentication and permissions
- Implement filtering and pagination
- Deploy to cloud (e.g., Heroku, Railway, Render)

## 📝 License

This project is for educational purposes under ALX SE program.
