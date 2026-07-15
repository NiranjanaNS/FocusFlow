# Wireframes

**Project:** FocusFlow  
**Document Version:** 1.0  
**Status:** Draft  
**Author:** Niranjana N Sajeev

---

# Table of Contents

1. Introduction
2. Design Goals
3. Screen List
4. Navigation Flow
5. Screen Wireframes
6. Responsive Design
7. UI Components
8. Future Screens
9. Design Notes
10. Revision History

---

# 1. Introduction

This document describes the layout and structure of every screen in FocusFlow.

The purpose of these wireframes is to define:

- Screen layouts
- Component placement
- Navigation
- User interaction
- Information hierarchy

These are low-fidelity wireframes intended for planning before visual UI design.

---

# 2. Design Goals

FocusFlow follows these design principles:

- Simple
- Clean
- Minimal
- Responsive
- Accessible
- Distraction-free

The interface should help users focus on their work rather than overwhelm them with unnecessary elements.

---

# 3. Screen List

## Version 1.0

- Dashboard
- Add/Edit Task Modal
- Task List

---

## Version 2.0

- Pomodoro Screen
- Analytics Dashboard

---

## Version 3.0

- Login
- Signup
- Profile
- Settings

---

# 4. Navigation Flow

```text
Dashboard
    │
    ├──────────────┐
    │              │
    ▼              ▼
Task List      Add Task
    │              │
    └──────┬───────┘
           ▼
      Edit Task
           │
           ▼
     Complete Task
```

Future navigation:

```text
Dashboard
     │
 ┌───┼──────────────┐
 │   │              │
 ▼   ▼              ▼
Tasks Analytics Pomodoro
 │      │            │
 ▼      ▼            ▼
Profile Settings Reports
```

---

# 5. Screen Wireframes

---

## Dashboard

Purpose:

Displays an overview of productivity and tasks.

```text
---------------------------------------------------
                    FocusFlow
---------------------------------------------------

Search...

-----------------------------------
Total Tasks      12
Completed        7
Pending          5
Progress         58%
-----------------------------------

+ Add Task

-----------------------------------
Task List

☐ Learn React

☑ Complete HTML Assignment

☐ Buy Groceries

☑ Read Chapter 5

-----------------------------------
```

Components:

- Header
- Search Bar
- Statistics Cards
- Progress Bar
- Add Task Button
- Task List

---

## Add/Edit Task Modal

Purpose:

Create or modify tasks.

```text
------------------------------

Title

______________________

Description

______________________

Priority

[Dropdown]

Category

[Dropdown]

Due Date

[Date Picker]

[Save]   [Cancel]

------------------------------
```

Components:

- Input fields
- Dropdowns
- Date Picker
- Action Buttons

---

## Task Card

```text
----------------------------------

Task Title

Category

Priority

Due Date

[Complete]

[Edit]

[Delete]

----------------------------------
```

---

## Empty State

```text
--------------------------

No Tasks Found

Create your first task.

[Add Task]

--------------------------
```

---

## Search Results

```text
Search: React

-----------------------

Learn React

React Assignment

React Notes

-----------------------
```

---

# 6. Responsive Design

## Desktop

```text
------------------------------------

Header

Statistics Cards

Search

Task List

------------------------------------
```

---

## Tablet

```text
-------------------------

Header

Statistics

Search

Task List

-------------------------
```

---

## Mobile

```text
----------------

Header

Search

Statistics

Task List

Floating Add Button

----------------
```

---

# 7. UI Components

The application uses reusable UI components.

## Buttons

- Primary Button
- Secondary Button
- Danger Button

---

## Input Fields

- Text Input
- Textarea
- Date Picker
- Dropdown

---

## Cards

- Statistics Card
- Task Card

---

## Navigation

- Header
- Navigation Menu (Future)

---

## Indicators

- Progress Bar
- Priority Badge
- Category Badge

---

## Icons

Examples:

- Add
- Edit
- Delete
- Complete
- Search
- Filter

---

# 8. Future Screens

---

## Pomodoro

```text
------------------------

25:00

Start

Pause

Reset

Today's Focus Time

------------------------
```

---

## Analytics

```text
-------------------------

Weekly Report

Chart

Completion Rate

Category Analysis

Focus Hours

-------------------------
```

---

## Login

```text
---------------------

Email

Password

Login

Register

---------------------
```

---

## Signup

```text
----------------------

Name

Email

Password

Confirm Password

Register

----------------------
```

---

## Profile

```text
-----------------------

Avatar

Name

Email

Statistics

Achievements

-----------------------
```

---

## Settings

```text
----------------------

Theme

Notifications

Language

Account

Privacy

----------------------
```

---

# 9. Design Notes

The interface should prioritize clarity and ease of use.

Design decisions include:

- Minimal distractions
- Consistent spacing
- Large clickable buttons
- Clear typography
- Responsive layout
- Reusable components
- Accessible color contrast
- Dark mode support

Future visual design will be created in Figma before implementation.

---

# Revision History

| Version | Description |
|----------|-------------|
| 1.0 | Initial wireframe document |