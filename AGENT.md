# AGENT.md - Gamezone Development Guide

## Commands
- **Run dev server**: `python manage.py runserver` (from gamezone_env/)
- **Run tests**: `python manage.py test` (Django test runner)
- **Run single test**: `python manage.py test rentals.tests.TestClassName.test_method`
- **Migrations**: `python manage.py makemigrations` then `python manage.py migrate`
- **Install deps**: `pip install -r requirements.txt`

## Architecture
- **Framework**: Django 5.0.2 with SQLite (dev), PostgreSQL (prod)
- **Main project**: `gamezone_env/gamezone/` (settings, urls, wsgi)
- **Apps**: `rentals/` (main gaming equipment rental functionality)
- **Models**: Empty starter models in `rentals/models.py`
- **Database**: SQLite for development, migrations in `rentals/migrations/`

## Code Style
- **Python**: Follow PEP 8, use Django conventions
- **Models**: Use Django ORM, define in `rentals/models.py`
- **Views**: Class-based views preferred, in `rentals/views.py`
- **Templates**: Store in `rentals/templates/`
- **URLs**: App-level URLs in `rentals/urls.py`, main in `gamezone/urls.py`
- **Tests**: Use Django TestCase, write in `rentals/tests.py`

## Key Dependencies
- django-crispy-forms, django-allauth, Pillow, stripe, django-leaflet
