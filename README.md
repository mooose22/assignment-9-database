# FastAPI Calculator with PostgreSQL (Docker Compose)

## Overview
This project demonstrates how to set up a FastAPI application with PostgreSQL and pgAdmin using Docker Compose. It also includes SQL operations to create tables, insert data, query records, update values, and delete data.

## Setup Instructions

1. Clone the repository:
git clone <repo-link>
cd <repo-folder>

2. Run Docker Compose:
docker-compose up --build

3. Access services:
- FastAPI: http://localhost:8000
- pgAdmin: http://localhost:5050

## pgAdmin Login
- Email: admin@example.com
- Password: admin

## Database Connection (pgAdmin)
- Host: db
- Port: 5432
- Username: postgres
- Password: postgres
- Database: fastapi_db

## SQL Operations Performed

### Create Tables
Created two tables:
- users (stores user info)
- calculations (stores math operations linked to users)

### Insert Data
Inserted sample records into both tables.

### Query Data
- Retrieved all users
- Retrieved all calculations
- Performed a JOIN to combine users and calculations

### Update Data
Updated a calculation result using its ID.

### Delete Data
Deleted a calculation record and verified removal.

## Database Relationship
The project uses a one-to-many relationship:
- One user can have many calculations
- Each calculation belongs to one user via user_id

## Files Included
- docker-compose.yml
- Dockerfile
- main.py
- database_commands.sql
- README.md
