# Mergington High School Activities

A super simple website application that allows students to view and sign up for extracurricular activities.

## Features

- View all available extracurricular activities
- Filter activities by:
  - Category (Sports, Arts, Academic, Community, Technology)
  - Day of the week
  - Time (Before School, After School, Weekend)
  - Difficulty level (Beginner, Intermediate, Advanced)
- Search for specific activities
- Teacher authentication system
- Register students for activities (teacher only)
- Responsive design for mobile and desktop

## Authentication

The website includes a teacher login system that allows:
- Teachers to login with username and password
- Session persistence across page reloads
- Access control for student registration

## Development Guide

For detailed setup and development instructions, please refer to our [Development Guide](../docs/how-to-develop.md).

## API Endpoints

The website utilizes the following key endpoints:
- GET `/activities` - Retrieve all activities (supports filters for category, day, time, and difficulty)
- POST `/activities/{activity_name}/signup` - Register a student for an activity
- POST `/auth/login` - Authenticate teachers
- GET `/auth/check-session` - Validate teacher session

> **Note:** All data is stored in memory and will reset when the server restarts.
