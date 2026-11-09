# Django with PostgreSQL (Dockerized)

A Django project wired to a PostgreSQL database and run with Docker Compose. Exercise from a Django book/course chapter on swapping SQLite for PostgreSQL in containers.

## Features

- Django project configured to use the `postgresql` backend
- Docker Compose services for the web app and a `postgres:13` database with a persistent volume

## Built with

- Django 4.0
- PostgreSQL with `psycopg2-binary`
- Docker / Docker Compose (Python 3.10 slim base image)

## Run it

```bash
docker-compose up
```

The web service starts the Django dev server on http://127.0.0.1:8000/ and connects to the `db` container. Learning project.

> Note: the Compose/settings use throwaway default Postgres credentials for local development only.
