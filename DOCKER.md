# Local Docker Setup

## Overview
This setup provides Dockerized services for:
- ASP.NET Core API (backend)
- MySQL database
- React frontend (built and served by Nginx)

## Prerequisites
- Docker Desktop

## Setup
1. Copy the example environment file:
   - `copy .env.example .env`
2. Update `.env` values as needed.
3. Start services:
   - `docker compose --env-file .env up --build`

## Service URLs
- API: http://localhost:5000
- Frontend: http://localhost:5173

## Notes
- Database data persists in the `mysql_data` volume.
- Avoid committing real secrets; keep them in `.env` locally.
