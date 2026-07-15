# System Architecture

**Project:** FocusFlow  
**Document Version:** 1.0  
**Status:** Draft  
**Author:** Niranjana N Sajeev

---

# Table of Contents

1. Introduction
2. Architecture Goals
3. System Overview
4. Current Architecture (v1.x)
5. Future MERN Architecture
6. Module Architecture
7. Folder Structure
8. Data Flow
9. Component Architecture
10. Design Principles
11. Design Patterns
12. Technology Stack
13. Scalability Strategy
14. Security Architecture
15. Deployment Architecture
16. Revision History

---

# 1. Introduction

This document defines the overall software architecture of FocusFlow.

Its purpose is to describe how different parts of the application are organized, how they communicate, and how the architecture will evolve as the project grows.

The architecture is designed to support incremental development, allowing the application to transition smoothly from a simple JavaScript application to a scalable MERN stack platform.

---

# 2. Architecture Goals

The architecture is designed with the following objectives:

- Simplicity
- Scalability
- Maintainability
- Modularity
- Reusability
- Performance
- Security
- Extensibility

---

# 3. System Overview

## Version 1 (Current)

```text
Browser
    │
    ▼
HTML
    │
    ▼
CSS
    │
    ▼
JavaScript
    │
    ▼
LocalStorage
```

The application runs entirely inside the browser.

No backend server is required.

---

## Future Architecture

```text
User
   │
   ▼
React Frontend
   │
REST API
   │
Express.js
   │
Node.js
   │
MongoDB
```

This architecture enables:

- User accounts
- Cloud synchronization
- Multiple devices
- Secure authentication
- API integration

---

# 4. Current Architecture (Version 1.x)

The current version follows a client-side architecture.

Responsibilities:

### HTML

- Application structure
- Forms
- Dashboard
- Task list

---

### CSS

- Layout
- Responsive design
- Themes
- Styling

---

### JavaScript

- Task management
- Validation
- Event handling
- LocalStorage
- UI updates

---

### LocalStorage

Stores:

- Tasks
- Settings
- Theme preference

---

# 5. Future MERN Architecture

```text
Client (React)
        │
 REST API (HTTPS)
        │
Express.js Server
        │
Business Logic
        │
MongoDB Database
```

Responsibilities:

## React

- UI
- Routing
- State Management

---

## Express

- API
- Validation
- Authentication

---

## Node.js

- Server runtime
- Business logic

---

## MongoDB

Stores:

- Users
- Tasks
- Categories
- Focus Sessions
- Reports
- Settings

---

# 6. Module Architecture

FocusFlow is divided into independent modules.

```text
FocusFlow

│

├── Dashboard

├── Task Management

├── Productivity

├── Analytics

├── Accountability

├── Notifications

├── Profile

├── Settings

└── AI Assistant
```

Each module should have minimal dependency on others.

---

# 7. Folder Structure

## Current

```text
FocusFlow/

│

├── docs/

├── design/

├── assets/

│

├── src/

│   ├── css/

│   ├── js/

│   ├── data/

│   └── utils/

│

├── index.html

├── README.md

└── LICENSE
```

---

## Future React Structure

```text
src/

│

├── assets/

├── components/

├── pages/

├── layouts/

├── hooks/

├── context/

├── services/

├── api/

├── utils/

├── constants/

├── styles/

├── routes/

├── App.jsx

└── main.jsx
```

---

# 8. Data Flow

## Current

```text
User

↓

UI

↓

JavaScript

↓

Validation

↓

LocalStorage

↓

UI Update
```

---

## Future

```text
User

↓

React

↓

API Request

↓

Express

↓

MongoDB

↓

Response

↓

React

↓

Updated UI
```

---

# 9. Component Architecture

## Dashboard

Contains:

- Statistics Cards
- Search Bar
- Filter
- Progress Bar
- Task List

---

## Task Component

Contains:

- Title
- Description
- Category
- Priority
- Due Date
- Buttons

---

## Future Components

- Navbar
- Sidebar
- Modal
- Timer
- Charts
- Calendar
- Notifications

---

# 10. Design Principles

FocusFlow follows these architectural principles.

## Separation of Concerns

Each file should have one responsibility.

---

## Reusability

Components should be reusable whenever possible.

---

## Modularity

Features should be separated into modules.

---

## Scalability

Adding new modules should require minimal changes.

---

## Maintainability

Code should remain readable and well organized.

---

# 11. Design Patterns

The following software design patterns will be used.

## Current

- Modular JavaScript
- Event-driven Programming

---

## Future

- Component-Based Architecture (React)
- MVC Pattern
- Repository Pattern
- Service Layer
- Context API

---

# 12. Technology Stack

## Current

| Layer | Technology |
|--------|------------|
| Frontend | HTML5 |
| Styling | CSS3 |
| Logic | JavaScript |
| Storage | LocalStorage |

---

## Future

| Layer | Technology |
|--------|------------|
| Frontend | React |
| Backend | Node.js |
| Framework | Express.js |
| Database | MongoDB |
| Authentication | JWT |
| File Storage | Cloudinary (Planned) |

---

# 13. Scalability Strategy

FocusFlow is designed for gradual expansion.

Roadmap:

Version 1

↓

Task Management

↓

Version 2

↓

Productivity

↓

Version 3

↓

Cloud

↓

Version 4

↓

AI

Each version builds upon the previous one without requiring a complete redesign.

---

# 14. Security Architecture

## Current

- Browser-only storage
- No authentication

---

## Future

- JWT Authentication
- Password Hashing
- HTTPS
- Input Validation
- Protected Routes
- Authorization Middleware

---

# 15. Deployment Architecture

## Version 1

```text
Browser

↓

GitHub Pages
```

---

## Future

```text
Frontend

↓

Vercel

↓

Express API

↓

Render

↓

MongoDB Atlas
```

---

# Revision History

| Version | Description |
|----------|-------------|
| 1.0 | Initial architecture document |