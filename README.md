# Recipe App API

## About the project

Recipe App API is a REST API for managing recipes, ingredients, and tags.

The project was developed as part of the Udemy course
**Backend REST API with Python & Django - Advanced** and served as a practical
introduction to building REST APIs with Django REST Framework, PostgreSQL,
Docker, automated testing, and deployment-oriented configuration.

This is an educational project based on the course material rather than an
independently designed portfolio application.

## Features

- User registration and authentication
- Recipe creation and management
- Ingredients and tags
- Recipe image uploads
- REST API built with Django REST Framework
- OpenAPI schema and API documentation
- Automated tests
- PostgreSQL database
- Dockerized development environment
- GitHub Actions CI
- Deployment-oriented Docker configuration

## Tech stack

- Python 3.12
- Django 5.0
- Django REST Framework
- PostgreSQL
- drf-spectacular
- Docker and Docker Compose
- Git and GitHub
- GitHub Actions
- Flake8
- uWSGI

## API

The project provides a REST API for managing users, recipes, ingredients,
and tags.

### API documentation

The project uses drf-spectacular for OpenAPI schema generation and
interactive API documentation.

## Testing

The project includes automated tests for the API and application behavior.

Run the test suite with:

```bash
docker compose run --rm app sh -c "python manage.py test"
```

## Installation

### Requirements

- Docker
- Docker Compose

### Setup

Clone the repository and navigate to the project directory:

```bash
git clone https://github.com/rwiszowaty/recipe-app-api.git
cd recipe-app-api
```

Create a `.env` file based on `.env.sample` and set the required environment
variables.

Build and start the containers:

```bash
docker compose up --build
```

The application will be available at:

```text
http://localhost:8000/
```

## Docker

The application runs in Docker containers using Docker Compose.

The development environment consists of:

- Django application
- PostgreSQL database

Start the development environment with:

```bash
docker compose up
```

Stop the containers with:

```bash
docker compose down
```

The repository also contains a separate Docker Compose configuration intended
for deployment.

## CI

The project uses GitHub Actions for continuous integration.

The CI workflow performs automated checks for the application, including
code quality and tests.

## Project structure

```text
recipe-app-api/
├── .github/
│   └── workflows/
├── app/
├── proxy/
├── scripts/
├── .env.sample
├── docker-compose.yml
├── docker-compose-deploy.yml
├── Dockerfile
├── requirments.txt
└── requirments.dev.txt
```

## Course

This project was developed as part of the Udemy course:

**Backend REST API with Python & Django - Advanced**

The repository is included in my GitHub portfolio to demonstrate the
technologies and backend development concepts I practiced during the course.
