# internship
# Backend API for File Upload Application

This is a FastAPI-based backend for a file upload application with user authentication using JWT tokens.

## Features

- User registration and login
- JWT authentication
- File upload, retrieval, and deletion
- SQLite database storage

## Setup

1. Create a virtual environment:
   ```
   python -m venv venv
   ```

2. Activate the virtual environment:
   - Windows: `venv\Scripts\activate`
   - macOS/Linux: `source venv/bin/activate`

3. Install dependencies:
   ```
   pip install -r requirements.txt
   ```

4. Run the application:
   ```
   python run.py
   ```

The API will be available at http://localhost:8000

## API Documentation

Once the server is running, you can access:
- Interactive API documentation: http://localhost:8000/docs
- Alternative documentation: http://localhost:8000/redoc

## API Endpoints

### Authentication
- POST /register - Register a new user
- POST /token - Login and get access token

### Files
- POST /upload - Upload a file
- GET /files - Get all files for current user
- GET /files/{file_id} - Get specific file details
- DELETE /files/{file_id} - Delete a file
