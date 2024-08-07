```markdown
# Octapus Tech Test - Todo List Application

This is a Django-based Todo List application deployed using Docker. The application allows users to register, log in, and manage their tasks.

## Features

- User registration and authentication
- Create, update, and delete tasks
- Task list and detail views
- Dockerized deployment

## Prerequisites

- Docker
- Docker Compose

## Getting Started

### Clone the Repository

```sh
git clone https://github.com/yourusername/octapus_tech_test.git
cd octapus_tech_test
```

Demo Video
Watch the demo video to see the application in action: 

[![Demo Video](https://img.youtube.com/vi/MbAq3b-94Fo/0.jpg)](https://www.youtube.com/watch?v=MbAq3b-94Fo)


### Build and Run the Docker Containers

```sh
docker-compose up --build
```

This command will build the Docker images and start the containers.

### Apply Migrations

Once the containers are up and running, apply the database migrations:

```sh
docker-compose exec web python manage.py migrate
```


### Access the Application

- The application will be available at `http://localhost:8000`
- The Django admin interface will be available at `http://localhost:8000/admin`

## Project Structure

- `octapus_tech_test/` - Main Django project directory
- `todo/` - Django app for managing tasks
- `templates/` - HTML templates for the application
- `Dockerfile` - Docker configuration for the web service
- `docker-compose.yml` - Docker Compose configuration

## Usage

### Register

Navigate to `/todo/register/` to create a new account.

### Login

Navigate to `/todo/login/` to log in to your account.

### Manage Tasks

- View tasks: `/todo/`
- Create a new task: `/todo/create/`
- Update a task: `/todo/update/<task_id>/`
- Delete a task: `/todo/delete/<task_id>/`
