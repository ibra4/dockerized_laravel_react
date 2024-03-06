# Dockerized Laravel 10 with Nginx, React 18, MySQL 8, MongoDB 7, and PHPMyAdmin

This repository provides a Dockerized setup for running

- Laravel `^10.10`
- PHP `8.3`
- Nginx
- React `18.2.0`
- Node `18`
- MySQL `8.1`
- MongoDB `7.0`
- PHPMyAdmin

## Prerequisites

Make sure you have the following installed on your system:

- Docker
- docker-compose

## Getting Started

- Clone this repository to your local machine
  ```sh
  git clone https://github.com/ibra4/dockerized_laravel_react
  ```
- Navigate to the cloned repository
  ```sh
  cd dockerized_laravel_react
  ```
- Configure your environment variables
  ```sh
  cp .env.example .env
  ```
- Build and start the Docker containers
  ```sh
  docker-compose up --build -d
  ```
  This command will build the Docker images and start the containers in detached mode

## Access application

- The React application is available at http://localhost:3000.
- The Backend application is available at http://localhost:8000.
- PHPMyAdmin is available at http://localhost:8080.
- Mongo Database is running on port `27027`
- Mysql Database is running on port `3306`

# Configuration

- PHP configuration:

  configuration files can be found in the [./docker/php](./docker/php) directory.

- Nginx configuration:

  configuration files can be found in the [./docker/nginx](./docker/nginx) directory.

- MySQL configuration:

  configuration can be found in the [./docker/mysql](./docker/mysql) directory.

- PHPMyAdmin configuration:

  configuration can be found in the [./docker/phpmyadmin](./docker/phpmyadmin) directory.
