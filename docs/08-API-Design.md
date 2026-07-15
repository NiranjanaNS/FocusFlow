# API Design

**Project:** FocusFlow  
**Document Version:** 1.0  
**Status:** Draft  
**Author:** Niranjana N Sajeev

---

# Table of Contents

1. Introduction
2. API Overview
3. API Standards
4. Authentication
5. Task API
6. Category API
7. Focus Session API
8. Notes API
9. Attachment API
10. Analytics API
11. Settings API
12. AI API
13. Error Responses
14. HTTP Status Codes
15. API Versioning
16. Future APIs
17. Revision History

---

# 1. Introduction

This document defines the REST API for FocusFlow.

The API allows communication between the frontend and backend, enabling task management, productivity tracking, analytics, authentication, and future AI-powered features.

Although Version 1 uses LocalStorage, these APIs are designed for the future MERN implementation.

---

# 2. API Overview

Base URL

```
https://api.focusflow.com/api/v1
```

Development

```
http://localhost:5000/api/v1
```

Data Format

- JSON

Protocol

- HTTPS

Authentication

- JWT (Future)

---

# 3. API Standards

## Request

```http
POST /tasks
Content-Type: application/json
```

Example

```json
{
  "title": "Complete JavaScript Assignment",
  "priority": "High"
}
```

---

## Response

```json
{
  "success": true,
  "message": "Task created successfully",
  "data": {}
}
```

---

## Error Response

```json
{
  "success": false,
  "message": "Validation failed"
}
```

---

# 4. Authentication API

## Register

### Endpoint

```
POST /auth/register
```

Request

```json
{
  "name": "Niranjana",
  "email": "user@example.com",
  "password": "password123"
}
```

Response

```json
{
  "success": true,
  "message": "User registered successfully"
}
```

---

## Login

```
POST /auth/login
```

Request

```json
{
  "email": "user@example.com",
  "password": "password123"
}
```

Response

```json
{
  "token": "JWT_TOKEN"
}
```

---

## Logout

```
POST /auth/logout
```

---

## Current User

```
GET /auth/me
```

---

# 5. Task API

## Get All Tasks

```
GET /tasks
```

---

## Get Task by ID

```
GET /tasks/:id
```

---

## Create Task

```
POST /tasks
```

Request

```json
{
  "title": "Learn React",
  "description": "Finish hooks",
  "priority": "High",
  "category": "Study",
  "dueDate": "2026-08-01"
}
```

---

## Update Task

```
PUT /tasks/:id
```

---

## Delete Task

```
DELETE /tasks/:id
```

---

## Complete Task

```
PATCH /tasks/:id/complete
```

---

## Mark Pending

```
PATCH /tasks/:id/pending
```

---

## Search Tasks

```
GET /tasks/search?q=react
```

---

## Filter Tasks

```
GET /tasks?priority=High
```

---

## Sort Tasks

```
GET /tasks?sort=dueDate
```

---

# 6. Category API

## Get Categories

```
GET /categories
```

---

## Create Category

```
POST /categories
```

---

## Update Category

```
PUT /categories/:id
```

---

## Delete Category

```
DELETE /categories/:id
```

---

# 7. Focus Session API

## Start Session

```
POST /focus/start
```

---

## End Session

```
POST /focus/end
```

---

## Get History

```
GET /focus/history
```

---

## Get Statistics

```
GET /focus/statistics
```

---

# 8. Notes API

## Create Note

```
POST /notes
```

---

## Update Note

```
PUT /notes/:id
```

---

## Delete Note

```
DELETE /notes/:id
```

---

## Get Notes

```
GET /notes
```

---

# 9. Attachment API

## Upload File

```
POST /attachments
```

---

## Get Files

```
GET /attachments
```

---

## Delete File

```
DELETE /attachments/:id
```

---

# 10. Analytics API

## Dashboard

```
GET /analytics/dashboard
```

---

## Daily Report

```
GET /analytics/daily
```

---

## Weekly Report

```
GET /analytics/weekly
```

---

## Monthly Report

```
GET /analytics/monthly
```

---

## Category Analysis

```
GET /analytics/categories
```

---

# 11. Settings API

## Get Settings

```
GET /settings
```

---

## Update Settings

```
PUT /settings
```

---

# 12. AI API (Future)

## Productivity Suggestions

```
GET /ai/suggestions
```

---

## Smart Priorities

```
GET /ai/priorities
```

---

## Weekly Summary

```
GET /ai/weekly-summary
```

---

## Natural Language Task

```
POST /ai/create-task
```

Example

```json
{
  "text": "Study React tomorrow at 7 PM"
}
```

Response

```json
{
  "title": "Study React",
  "dueDate": "2026-08-01",
  "time": "19:00"
}
```

---

# 13. Error Responses

## Validation Error

```json
{
  "success": false,
  "message": "Title is required"
}
```

---

## Unauthorized

```json
{
  "success": false,
  "message": "Unauthorized"
}
```

---

## Not Found

```json
{
  "success": false,
  "message": "Task not found"
}
```

---

## Internal Server Error

```json
{
  "success": false,
  "message": "Something went wrong"
}
```

---

# 14. HTTP Status Codes

| Code | Meaning |
|------|---------|
| 200 | OK |
| 201 | Created |
| 204 | No Content |
| 400 | Bad Request |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |
| 409 | Conflict |
| 422 | Validation Error |
| 500 | Internal Server Error |

---

# 15. API Versioning

Current Version

```
/api/v1
```

Future versions

```
/api/v2
/api/v3
```

Versioning ensures backward compatibility when introducing breaking changes.

---

# 16. Future APIs

Planned endpoints include:

- Notifications
- Calendar
- Team Collaboration
- Shared Projects
- Activity Logs
- AI Chat Assistant
- Smart Scheduling
- Browser Notifications
- Mobile Sync

---

# Revision History

| Version | Description |
|----------|-------------|
| 1.0 | Initial API Design |