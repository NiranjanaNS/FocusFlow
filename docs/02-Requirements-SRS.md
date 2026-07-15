# Software Requirements Specification (SRS)

**Project:** FocusFlow  
**Version:** 1.0  
**Document Version:** 1.0  
**Status:** Draft  
**Author:** Niranjana N Sajeev

---

# Table of Contents

1. Introduction
2. Overall Description
3. System Features
4. Functional Requirements
5. Non-Functional Requirements
6. User Interface Requirements
7. Data Requirements
8. Constraints
9. Assumptions
10. Future Enhancements
11. Acceptance Criteria

---

# 1. Introduction

## 1.1 Purpose

The purpose of this Software Requirements Specification (SRS) is to define the functional and non-functional requirements of the FocusFlow application.

This document serves as the primary reference for designing, developing, testing, and maintaining the application throughout its development lifecycle.

---

## 1.2 Scope

FocusFlow is a personal productivity platform designed to help users organize tasks, improve focus, monitor productivity, and track progress.

The initial version focuses on task management using LocalStorage, while future versions will evolve into a cloud-based MERN application with authentication, analytics, productivity tools, and AI-powered insights.

---

## 1.3 Objectives

The primary objectives are:

- Build a reliable task management application.
- Improve user productivity.
- Encourage consistent task completion.
- Track measurable progress.
- Develop scalable software architecture.
- Prepare for future cloud deployment.

---

## 1.4 Intended Audience

This document is intended for:

- Developers
- Designers
- Testers
- Future contributors
- Project owner

---

## 1.5 Definitions

| Term | Description |
|-------|-------------|
| Task | A unit of work created by the user |
| Dashboard | Main screen displaying statistics |
| Priority | Importance level of a task |
| Category | Group to which a task belongs |
| Pomodoro | Timed focus session |
| Streak | Consecutive productive days |
| Proof | Evidence showing task completion |

---

# 2. Overall Description

## 2.1 Product Perspective

FocusFlow begins as a browser-based task management application.

It will gradually evolve into a full-stack productivity platform capable of:

- Task Management
- Productivity Tracking
- Analytics
- Accountability
- Cloud Synchronization
- AI Assistance

---

## 2.2 Product Goals

The application aims to:

- Simplify task management.
- Encourage productivity.
- Reduce procrastination.
- Measure progress.
- Build productive habits.

---

## 2.3 User Classes

### Student

Needs assignment tracking and study planning.

### Developer

Needs project planning and coding sessions.

### Freelancer

Needs client task organization.

### Professional

Needs work planning and productivity monitoring.

---

## 2.4 Operating Environment

### Current

- Modern Web Browser
- HTML5
- CSS3
- JavaScript
- LocalStorage

### Future

- React
- Node.js
- Express.js
- MongoDB
- JWT Authentication

---

# 3. System Features

The system consists of several modules.

## Version 1

Task Management

- Create Task
- Edit Task
- Delete Task
- Complete Task
- Pending Task
- Search
- Filter
- Categories
- Priority
- Due Date

---

## Version 2

Productivity

- Pomodoro Timer
- Focus Mode
- Break Timer
- Daily Planner

---

## Version 3

Analytics

- Dashboard
- Charts
- Weekly Reports
- Monthly Reports

---

## Version 4

Accountability

- Proof Upload
- Notes
- Attachments

---

## Version 5

Cloud

- Login
- Signup
- Synchronization

---

## Version 6

AI

- Smart Suggestions
- Task Prioritization
- Productivity Coach

---

# 4. Functional Requirements

Each requirement has a unique identifier.

---

## Task Management

### FR-001

The system shall allow users to create a task.

---

### FR-002

The system shall allow users to edit existing tasks.

---

### FR-003

The system shall allow users to delete tasks.

---

### FR-004

The system shall allow users to mark tasks as completed.

---

### FR-005

The system shall allow users to mark completed tasks as pending.

---

### FR-006

The system shall automatically save tasks using LocalStorage.

---

### FR-007

The system shall automatically load saved tasks after page refresh.

---

### FR-008

The system shall allow users to assign a priority.

---

### FR-009

The system shall allow users to assign categories.

---

### FR-010

The system shall allow users to select due dates.

---

### FR-011

The system shall allow users to search tasks.

---

### FR-012

The system shall allow users to filter tasks.

---

### FR-013

The system shall allow users to sort tasks.

---

## Dashboard

### FR-014

Display total number of tasks.

---

### FR-015

Display completed tasks.

---

### FR-016

Display pending tasks.

---

### FR-017

Display completion progress.

---

## Productivity

### FR-018

The system shall provide a Pomodoro timer.

---

### FR-019

The system shall support focus mode.

---

### FR-020

The system shall record focus time.

---

## Analytics

### FR-021

Generate daily reports.

---

### FR-022

Generate weekly reports.

---

### FR-023

Generate monthly reports.

---

### FR-024

Display productivity charts.

---

## Accountability

### FR-025

Allow users to upload screenshots.

---

### FR-026

Allow users to attach notes.

---

### FR-027

Allow users to upload files.

---

### FR-028

Allow GitHub repository links.

---

## Authentication

### FR-029

Allow user registration.

---

### FR-030

Allow user login.

---

### FR-031

Allow secure logout.

---

### FR-032

Synchronize user data across devices.

---

## AI

### FR-033

Generate productivity insights.

---

### FR-034

Recommend task priorities.

---

### FR-035

Generate weekly summaries.

---

### FR-036

Suggest productivity improvements.

---

# 5. Non-Functional Requirements

## Performance

- Page load time should be less than 2 seconds.
- Search should complete within 500 milliseconds.

---

## Reliability

- Task data should not be lost after refresh.
- Saved tasks should persist between sessions.

---

## Scalability

The application architecture should support migration to MERN without major redesign.

---

## Maintainability

- Modular JavaScript
- Reusable functions
- Organized folder structure

---

## Security

Future versions shall include:

- Password hashing
- JWT Authentication
- Secure API communication

---

## Usability

- Easy to learn
- Minimal user interaction
- Responsive layout

---

## Accessibility

The application should:

- Support keyboard navigation.
- Maintain sufficient color contrast.
- Use semantic HTML.

---

# 6. User Interface Requirements

## Dashboard

Contains:

- Task statistics
- Progress bar
- Search
- Filters

---

## Task Form

Fields:

- Title
- Description
- Priority
- Category
- Due Date

Buttons:

- Save
- Cancel

---

## Task List

Displays:

- Task title
- Category
- Priority
- Due date
- Completion status

Actions:

- Edit
- Delete
- Complete

---

## Future Screens

- Login
- Signup
- Analytics
- Profile
- Settings
- Focus Mode

---

# 7. Data Requirements

## Task

| Field | Type |
|--------|------|
| id | String |
| title | String |
| description | String |
| priority | String |
| category | String |
| dueDate | Date |
| completed | Boolean |
| createdAt | Date |
| updatedAt | Date |

---

## User (Future)

| Field | Type |
|--------|------|
| id | String |
| name | String |
| email | String |
| password | String |

---

## Focus Session

| Field | Type |
|--------|------|
| id | String |
| taskId | String |
| duration | Number |
| completed | Boolean |

---

# 8. Constraints

Version 1 limitations:

- Browser only.
- LocalStorage only.
- No authentication.
- No cloud synchronization.
- No offline sync beyond LocalStorage.

---

# 9. Assumptions

The project assumes:

- Users have modern browsers.
- JavaScript is enabled.
- LocalStorage is available.
- Internet is required only for future cloud versions.

---

# 10. Future Enhancements

Planned enhancements include:

- MERN migration
- Cloud synchronization
- Team collaboration
- AI productivity assistant
- Notifications
- Calendar integration
- Gamification
- Smart reminders
- Mobile application

---

# 11. Acceptance Criteria

The Version 1 release will be considered complete when:

- Users can create tasks.
- Users can edit tasks.
- Users can delete tasks.
- Users can complete tasks.
- Tasks persist after refresh.
- Dashboard statistics update correctly.
- Search and filters work correctly.
- Responsive design works on desktop and mobile.
- No major functional bugs remain.

---

# Revision History

| Version | Date | Description |
|----------|------|-------------|
| 1.0 | Initial Draft | First SRS for FocusFlow |
