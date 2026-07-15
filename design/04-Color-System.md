# FocusFlow – Color System

**Project:** FocusFlow  
**Document Version:** 1.0  
**Status:** Draft

---

# 1. Purpose

The FocusFlow color system establishes a consistent visual language for the application.

The objectives are:

- Improve readability
- Guide user attention
- Communicate status clearly
- Support accessibility
- Maintain consistency across all screens
- Enable both Light and Dark themes

---

# 2. Brand Personality

The colors should make users feel:

- Focused
- Calm
- Productive
- Modern
- Professional
- Trustworthy

Avoid colors that create unnecessary stress or visual noise.

---

# 3. Primary Brand Colors

## Primary

Indigo

HEX

#4F46E5

Usage

- Primary Buttons
- Active Navigation
- Links
- Selected Items
- Highlights

---

## Secondary

Cyan

HEX

#06B6D4

Usage

- Charts
- Focus Timer
- Analytics
- Secondary Actions

---

## Accent

Purple

HEX

#7C3AED

Usage

- Premium Features
- AI Features
- Badges
- Special Highlights

---

# 4. Semantic Colors

## Success

HEX

#22C55E

Used for:

- Completed Tasks
- Success Messages
- Positive Statistics
- Completed Progress

---

## Warning

HEX

#F59E0B

Used for:

- Upcoming Deadlines
- Medium Priority
- Alerts

---

## Error

HEX

#EF4444

Used for:

- Delete Buttons
- Validation Errors
- Failed Operations
- High Priority Tasks

---

## Information

HEX

#3B82F6

Used for:

- Notifications
- Tips
- Information Cards

---

# 5. Neutral Palette

## Background

#F8FAFC

Main application background.

---

## Surface

#FFFFFF

Cards
Dialogs
Sidebar
Navbar

---

## Border

#E2E8F0

Used for:

Cards

Inputs

Tables

Dividers

---

## Text Primary

#0F172A

Main content.

---

## Text Secondary

#64748B

Descriptions

Metadata

Subtitles

---

## Disabled

#CBD5E1

Disabled buttons

Inactive icons

Placeholder text

---

# 6. Dark Theme

Background

#0F172A

Surface

#1E293B

Card

#334155

Primary Text

#F8FAFC

Secondary Text

#CBD5E1

Border

#475569

---

# 7. Task Priority Colors

Low

Blue

#3B82F6

Medium

Amber

#F59E0B

High

Red

#EF4444

Completed

Green

#22C55E

---

# 8. Task Status

Pending

Gray

#94A3B8

In Progress

Blue

#3B82F6

Completed

Green

#22C55E

Overdue

Red

#EF4444

Archived

Slate

#64748B

---

# 9. Productivity Dashboard Colors

Focus Time

Cyan

Completed Tasks

Green

Pending Tasks

Amber

Overdue Tasks

Red

Productivity Score

Purple

---

# 10. Chart Palette

Chart 1

#4F46E5

Chart 2

#06B6D4

Chart 3

#22C55E

Chart 4

#F59E0B

Chart 5

#EF4444

Chart 6

#7C3AED

---

# 11. Button Colors

Primary Button

Background

#4F46E5

Text

White

Hover

#4338CA

---

Secondary Button

Background

White

Border

#4F46E5

Text

#4F46E5

Hover

#EEF2FF

---

Danger Button

Background

#EF4444

Text

White

Hover

#DC2626

---

Success Button

Background

#22C55E

Hover

#16A34A

---

# 12. Form Colors

Input Border

#CBD5E1

Focused Border

#4F46E5

Error Border

#EF4444

Disabled Background

#F1F5F9

Placeholder

#94A3B8

---

# 13. Accessibility

All text should satisfy WCAG AA contrast requirements.

Minimum text contrast ratio:

4.5 : 1

Interactive elements should always have:

Hover state

Focus state

Disabled state

Active state

---

# 14. Color Usage Rules

Primary Color

Maximum 10–15% of the screen.

Accent Color

Use only to draw attention.

Success Color

Only for completed or successful actions.

Warning

Never use for destructive actions.

Error

Only for errors or destructive operations.

Avoid using more than three strong colors within the same component.

---

# 15. Future Support

The color system should support:

- Light Theme
- Dark Theme
- High Contrast Mode
- Theme Customization

---

# 16. Design Tokens

Primary

--color-primary

Secondary

--color-secondary

Accent

--color-accent

Background

--color-background

Surface

--color-surface

Text

--color-text

Border

--color-border

Success

--color-success

Warning

--color-warning

Error

--color-error

Info

--color-info

These tokens should be used consistently in CSS, Tailwind CSS, React components, and Figma variables.

---

# 17. Summary

The FocusFlow color system is designed to create a calm, professional, and productive experience. Every color has a defined purpose to improve usability, maintain consistency, and support accessibility as the application grows.