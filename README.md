# React Frontend + Django Backend

A simple full-stack product management app built with React, Vite, Django, Django REST Framework, and SQLite.

## Features

- List, add, update, and delete products
- Product images stored in the Django `media/` directory
- REST API served from `/api/products/`
- React frontend with Bootstrap styling

## Project Structure

```text
backend/      Django project settings and URLs
products/     Product model, serializer, views, and API routes
frontend/     React + Vite frontend
media/        Uploaded product images
manage.py     Django management script
```

## Setup

Install backend dependencies:

```bash
pip install django djangorestframework django-cors-headers pillow
python manage.py migrate
python manage.py runserver
```

Install and run the frontend:

```bash
cd frontend
npm install
npm run dev
```

## Usage

- Backend API: `http://127.0.0.1:8000/api/products/`
- Frontend app: `http://localhost:5173/`

Use the frontend to manage products, or call the API directly for CRUD operations.
