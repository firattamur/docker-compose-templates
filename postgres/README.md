# PostgreSQL and PgAdmin:

This directory contains a Docker Compose configuration for setting up a PostgreSQL database and PgAdmin, a popular web-based PostgreSQL database management tool.

## Services

- `postgresdb`: 
  
  - This service sets up a PostgreSQL database. By default, it uses the latest Postgres image from Docker Hub.
  
  - `username`: postgres
  - `password`: postgres
  
- `pgadmin`: 
  
  - This service sets up PgAdmin. By default, it uses the dpage/pgadmin4 image from Docker Hub.
  - `admin_email`: pgadmin@postgres.com
  - `admin_password`: pgadmin

## How to Use

1. Navigate into this directory: `cd docker-compose-templates/postgres`
2. Run Docker Compose: `docker-compose up -d`

By default, the PostgreSQL database will be accessible on port `5432` and PgAdmin will be accessible on port `5050`.

## Volumes

Two Docker volumes are created and used by these services:

- `pg-data`: This volume is used to persist the data of the PostgreSQL database.
- `pgadmin-data`: This volume is used to persist the data of PgAdmin.

## Customization

You can customize the configuration by modifying the `docker-compose.yml` file. For example, you can change the ports, the environment variables, or the Docker images used.

Remember to replace the default usernames, passwords, and email with secure ones if you're using this configuration in a production environment.

