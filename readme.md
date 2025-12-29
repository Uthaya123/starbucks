# Starbucks Web Registration with Database

This is a Starbucks coffee company website clone with user registration backed by a SQLite database and Node.js/Express backend.

## Quick Start

### 1. Install Dependencies

```bash
npm install
```

### 2. Start the Server

```bash
npm start
```

The server will run on `http://localhost:3000` and serve the website.

### 3. Open in Browser

Navigate to `http://localhost:3000`

## Features

- **User Registration**: Create accounts with email and password
- **Secure Password Storage**: Passwords hashed with bcrypt
- **SQLite Database**: Persistent user data storage
- **Email Validation**: Prevents duplicate registrations
- **CORS Enabled**: Frontend-backend communication

## API Endpoints

### POST /api/register
Register a new user.

**Request:**
```json
{
  "name": "John Doe",
  "email": "john@example.com",
  "password": "password123",
  "confirmPassword": "password123"
}
```

**Response (Success):**
```json
{
  "success": true,
  "message": "Account created successfully!",
  "userId": 1
}
```

### GET /api/health
Health check endpoint.

## Database

- **Type**: SQLite
- **File**: `starbucks.db` (auto-created)
- **Table**: `users` with id, name, email, password, createdAt

## Files

- `server.js` - Express backend with database logic
- `package.json` - Dependencies
- `registration.html` - Registration page
- `script.js` - Frontend form handlers
- `style.css` - Styling
- Original [YouTube tutorial](https://youtu.be/x_n2FGNsm0o)
