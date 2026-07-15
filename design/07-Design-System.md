# FocusFlow – Design System

**Project:** FocusFlow  
**Version:** 1.0  
**Status:** Draft

---

# 1. Purpose

The FocusFlow Design System defines reusable UI components, interaction patterns, visual standards, and design rules used throughout the application.

Its goals are to:

- Maintain consistency
- Improve usability
- Speed up development
- Simplify maintenance
- Ensure accessibility
- Support future scalability

This document acts as the single source of truth for both designers and developers.

---

# 2. Foundations

The design system is built on:

- Brand Identity
- Color System
- Typography
- Spacing & Grid
- Accessibility Guidelines

Every component must follow these foundations.

---

# 3. Design Principles

Every component should be:

- Consistent
- Reusable
- Accessible
- Responsive
- Predictable
- Minimal
- Easy to understand

---

# 4. Border Radius

| Component | Radius |
|-----------|--------:|
| Buttons | 12 px |
| Inputs | 12 px |
| Cards | 16 px |
| Modals | 24 px |
| Badges | 999 px |
| Avatar | 50% |

---

# 5. Elevation

## Level 0

No shadow

Used for:

- Navigation
- Backgrounds

---

## Level 1

Small Shadow

Used for:

- Cards
- Inputs

---

## Level 2

Medium Shadow

Used for:

- Dropdowns
- Floating Buttons
- Popovers

---

## Level 3

Large Shadow

Used for:

- Dialogs
- Modals

---

# 6. Buttons

## Primary

Purpose

Main action

Examples

- Create Task
- Save
- Login

States

- Default
- Hover
- Active
- Focus
- Disabled
- Loading

---

## Secondary

Purpose

Alternative action

Examples

- Cancel
- Edit
- View

---

## Outline

Purpose

Less important actions.

---

## Danger

Purpose

Delete

Remove

Reset

---

## Success

Purpose

Complete Task

Confirm

Approve

---

# 7. Inputs

Supported Fields

- Text
- Search
- Email
- Password
- Number
- Date
- Time
- Textarea

Each input includes

- Label
- Placeholder
- Helper Text
- Error Message
- Success State

---

# 8. Search Component

Includes

- Search Icon
- Clear Button
- Keyboard Shortcut
- Filter Button

---

# 9. Dropdown

Supports

- Single Select
- Multi Select
- Search
- Groups

---

# 10. Checkbox

States

- Default
- Hover
- Checked
- Disabled

---

# 11. Radio Button

Used for

- Priority
- Theme
- Settings

---

# 12. Toggle Switch

Used for

- Dark Mode
- Notifications
- Auto Save
- Focus Mode

---

# 13. Cards

## Task Card

Displays

- Title
- Description
- Category
- Priority
- Due Date
- Status
- Actions

---

## Statistics Card

Displays

- Metric
- Icon
- Trend
- Percentage

---

## Analytics Card

Displays

- Chart
- Title
- Summary

---

## Profile Card

Displays

- Avatar
- Name
- Email
- Productivity Score

---

# 14. Badges

Types

- Low
- Medium
- High
- Completed
- Pending
- Overdue

---

# 15. Navigation

Desktop

- Sidebar

Contains

- Dashboard
- Tasks
- Calendar
- Analytics
- Pomodoro
- Profile
- Settings

---

Mobile

Bottom Navigation

Maximum five items.

---

# 16. Top Bar

Contains

- Logo
- Search
- Notifications
- User Avatar

---

# 17. Sidebar

States

Expanded

Collapsed

---

# 18. Modals

Supported

- Add Task
- Edit Task
- Delete Confirmation
- Settings
- Profile

---

# 19. Toast Notifications

Types

- Success
- Warning
- Error
- Info

Position

Top Right

Auto dismiss after 4 seconds.

---

# 20. Alerts

Used for

- Errors
- Warnings
- Information

---

# 21. Progress Components

- Progress Bar
- Circular Progress
- Daily Goal
- Weekly Goal

---

# 22. Charts

Supported

- Line Chart
- Bar Chart
- Pie Chart
- Area Chart

---

# 23. Empty States

Each empty state contains

- Illustration
- Title
- Description
- Primary Action

---

# 24. Loading States

Use

- Skeleton Loaders
- Progress Indicators
- Spinners

Avoid layout shifts.

---

# 25. Tables

Features

- Sorting
- Filtering
- Pagination
- Responsive Layout

---

# 26. Calendar Components

Views

- Daily
- Weekly
- Monthly

---

# 27. Accessibility

All interactive components must support

- Keyboard navigation
- Screen readers
- Focus indicators
- ARIA labels
- WCAG AA compliance

---

# 28. Responsive Rules

Desktop

Sidebar

Tablet

Collapsed Sidebar

Mobile

Bottom Navigation

Cards stack vertically.

---

# 29. Animation

Duration

Fast

150 ms

Normal

250 ms

Slow

350 ms

Animation Principles

- Smooth
- Subtle
- Purposeful

Avoid excessive motion.

---

# 30. Icon System

Recommended Library

Lucide Icons

Sizes

16 px

20 px

24 px

32 px

---

# 31. Component Naming

Examples

ButtonPrimary

TaskCard

SearchInput

SidebarItem

StatisticsCard

ProgressRing

CalendarCard

Keep naming consistent between Figma and React.

---

# 32. Design Tokens

Use tokens for:

Colors

Spacing

Typography

Radius

Shadows

Animations

Never hardcode design values in components.

---

# 33. Future Components

Planned additions

- AI Chat Panel
- Voice Input
- Productivity Coach
- Team Workspace
- Kanban Board
- Timeline View
- Habit Tracker
- Goal Dashboard

---

# 34. Summary

The FocusFlow Design System provides a reusable foundation for building a consistent, scalable, and accessible user interface. Every screen and component should follow this system to ensure a unified experience across the application.