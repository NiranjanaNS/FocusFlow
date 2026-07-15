# Database Design

**Project:** FocusFlow  
**Document Version:** 1.0  
**Status:** Draft  
**Author:** Niranjana N Sajeev

---

# Table of Contents

1. Introduction
2. Database Objectives
3. Database Overview
4. Collections
5. Collection Schemas
6. Relationships
7. Entity Relationship Diagram (ERD)
8. Indexing Strategy
9. Validation Rules
10. Data Flow
11. Future Database Expansion
12. Revision History

---

# 1. Introduction

This document defines the database design for FocusFlow.

Although Version 1 stores data using the browser's LocalStorage, this database design is intended for the future MongoDB implementation. Designing the database early ensures scalability, consistency, and an easier transition to the MERN stack.

---

# 2. Database Objectives

The database should:

- Store user information securely.
- Organize productivity data efficiently.
- Support future feature expansion.
- Minimize data duplication.
- Maintain relationships between entities.
- Provide fast query performance.

---

# 3. Database Overview

## Version 1

```text
Browser
    │
    ▼
LocalStorage
```

---

## Future Version

```text
React
   │
   ▼
Express API
   │
   ▼
MongoDB
```

---

# 4. Collections

FocusFlow will use the following collections:

| Collection | Purpose |
|------------|---------|
| Users | User accounts |
| Tasks | Task information |
| Categories | Task categories |
| FocusSessions | Pomodoro sessions |
| Notes | Task notes |
| Attachments | Proof and uploaded files |
| Achievements | XP, badges, streaks |
| Reports | Analytics data |
| Settings | User preferences |

---

# 5. Collection Schemas

---

## Users Collection

```javascript
{
    _id: ObjectId,
    name: String,
    email: String,
    password: String,
    avatar: String,
    createdAt: Date,
    updatedAt: Date
}
```

### Description

Stores user account information.

---

## Tasks Collection

```javascript
{
    _id: ObjectId,
    userId: ObjectId,

    title: String,
    description: String,

    categoryId: ObjectId,

    priority: "Low | Medium | High",

    dueDate: Date,

    status: "Pending | Completed",

    createdAt: Date,
    updatedAt: Date
}
```

### Description

Stores every task created by users.

---

## Categories Collection

```javascript
{
    _id: ObjectId,
    userId: ObjectId,

    name: String,

    color: String,

    createdAt: Date
}
```

### Description

Stores user-defined categories.

Examples:

- Study
- Work
- Personal
- Health

---

## FocusSessions Collection

```javascript
{
    _id: ObjectId,

    userId: ObjectId,

    taskId: ObjectId,

    duration: Number,

    completed: Boolean,

    startedAt: Date,

    endedAt: Date
}
```

### Description

Stores Pomodoro and focus session data.

---

## Notes Collection

```javascript
{
    _id: ObjectId,

    taskId: ObjectId,

    userId: ObjectId,

    content: String,

    createdAt: Date
}
```

### Description

Stores notes linked to tasks.

---

## Attachments Collection

```javascript
{
    _id: ObjectId,

    taskId: ObjectId,

    userId: ObjectId,

    type: String,

    fileUrl: String,

    uploadedAt: Date
}
```

### Supported Types

- Image
- PDF
- Screenshot
- GitHub Link
- Document

---

## Achievements Collection

```javascript
{
    _id: ObjectId,

    userId: ObjectId,

    xp: Number,

    level: Number,

    streak: Number,

    badges: Array
}
```

### Description

Stores gamification data.

---

## Reports Collection

```javascript
{
    _id: ObjectId,

    userId: ObjectId,

    date: Date,

    completedTasks: Number,

    focusMinutes: Number,

    completionRate: Number
}
```

### Description

Stores productivity analytics.

---

## Settings Collection

```javascript
{
    _id: ObjectId,

    userId: ObjectId,

    theme: String,

    notifications: Boolean,

    language: String
}
```

---

# 6. Relationships

## User → Tasks

One user can create many tasks.

```text
User

1

│

├───────∞ Tasks
```

---

## Category → Tasks

One category can contain multiple tasks.

```text
Category

1

│

├───────∞ Tasks
```

---

## Task → Focus Sessions

One task can have many focus sessions.

```text
Task

1

│

├──────∞ Focus Sessions
```

---

## Task → Notes

```text
Task

1

│

├──────∞ Notes
```

---

## Task → Attachments

```text
Task

1

│

├──────∞ Attachments
```

---

## User → Reports

```text
User

1

│

├──────∞ Reports
```

---

# 7. Entity Relationship Diagram (ERD)

```text
                 +----------------+
                 |     Users      |
                 +----------------+
                        |
          +-------------+-------------+
          |                           |
          ▼                           ▼
     +----------+               +------------+
     |  Tasks   |               |  Reports   |
     +----------+               +------------+
          |
    +-----+-----+-----+
    |     |     |     |
    ▼     ▼     ▼     ▼
Categories Notes FocusSessions Attachments

          |
          ▼
Achievements
```

---

# 8. Indexing Strategy

To improve performance, indexes will be created for commonly queried fields.

## Users

- email (unique)

---

## Tasks

- userId
- categoryId
- dueDate
- status

---

## Focus Sessions

- userId
- taskId

---

## Reports

- userId
- date

---

# 9. Validation Rules

## Users

- Name is required.
- Email must be unique.
- Password must be encrypted.
- Email format must be valid.

---

## Tasks

- Title is required.
- Priority must be Low, Medium, or High.
- Due date cannot be before the creation date.
- Status must be Pending or Completed.

---

## Categories

- Name is required.
- Duplicate category names are not allowed for the same user.

---

## Notes

- Content cannot be empty.

---

## Attachments

- File type must be supported.
- File size must not exceed application limits.

---

# 10. Data Flow

## Version 1

```text
User

↓

Task Form

↓

JavaScript Object

↓

LocalStorage

↓

Dashboard
```

---

## Future Version

```text
User

↓

React Form

↓

API

↓

Validation

↓

MongoDB

↓

Dashboard
```

---

# 11. Future Database Expansion

Future versions may introduce additional collections.

## Planned Collections

- Notifications
- Teams
- Workspaces
- Calendars
- AI Insights
- Activity Logs
- Shared Projects

These collections are intentionally excluded from Version 1 to keep the initial implementation simple while allowing future growth.

---

# Revision History

| Version | Description |
|----------|-------------|
| 1.0 | Initial database design |