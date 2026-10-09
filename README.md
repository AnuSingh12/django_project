# Django REST API User Authentication using JWT

## Overview
A REST API project for user authentication built using Django, Django REST Framework, and Simple JWT.

## Features
- User registration
- User login
- JWT access and refresh token generation
- JWT token verification
- Access token refresh
- SQLite database integration

## Tech Stack
- Python
- Django
- Django REST Framework
- djangorestframework-simplejwt
- SQLite

## Setup Instructions

1. Clone the repository:
   ```bash
   git clone YOUR_GITHUB_REPOSITORY_URL
   cd user-auth-jwt
   ```

2. Create and activate a virtual environment:
   ```bash
   python -m venv venv
   venv\Scripts\activate
   ```

3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

4. Apply database migrations:
   ```bash
   python manage.py migrate
   ```

5. Start the development server:
   ```bash
   python manage.py runserver
   ```

## API Endpoints

| Method | Endpoint | Purpose |
|---|---|---|
| POST | `/api/accounts/register/` | Register a user |
| POST | `/api/accounts/login/` | Login and generate JWT tokens |
| POST | `/api/accounts/token/verify/` | Verify a JWT token |
| POST | `/api/accounts/token/refresh/` | Refresh an access token |

## Registration Request

```json
{
  "username": "anu",
  "email": "anu@example.com",
  "password": "Anu@12345",
  "password2": "Anu@12345"
}
```

## Login Request

```json
{
  "username": "anu",
  "password": "Anu@12345"
}
```
