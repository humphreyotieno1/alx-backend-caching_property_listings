# ALX Backend Caching - Property Listings

A Django project demonstrating caching with Redis and PostgreSQL in Docker.

## Setup

1. Clone the repository
2. Run `docker-compose up -d`
3. Run migrations: `python manage.py migrate`
4. Create a superuser: `python manage.py createsuperuser`
5. Run the development server: `python manage.py runserver`

## API Endpoints

- `GET /api/properties/` - List all properties (cached for 15 minutes)

## Features

- Dockerized PostgreSQL and Redis
- View-level caching
- Low-level queryset caching
- Cache invalidation using signals
- Redis cache metrics