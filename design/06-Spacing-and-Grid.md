# FocusFlow – Spacing & Grid System

**Project:** FocusFlow  
**Document Version:** 1.0  
**Status:** Draft

---

# 1. Purpose

The spacing and grid system ensures every screen in FocusFlow maintains consistent alignment, spacing, and proportions.

A unified spacing system improves:

- Readability
- Visual balance
- Scalability
- Responsive behavior
- Developer consistency

All layouts should follow this document.

---

# 2. Design Philosophy

FocusFlow follows an **8-point design system**.

Almost every spacing value should be a multiple of 8.

Examples

8

16

24

32

40

48

56

64

This creates rhythm and consistency across the interface.

---

# 3. Base Spacing Scale

| Token | Pixels | Usage |
|--------|-------:|------|
| xs | 4 px | Tiny gaps |
| sm | 8 px | Icons, badges |
| md | 16 px | Between related elements |
| lg | 24 px | Between sections |
| xl | 32 px | Large spacing |
| 2xl | 40 px | Screen padding |
| 3xl | 48 px | Major layouts |
| 4xl | 64 px | Large page sections |

---

# 4. Page Padding

Desktop

40 px

Tablet

32 px

Mobile

20 px

Every page should use consistent outer padding.

---

# 5. Card Spacing

Internal Padding

24 px

Gap Between Cards

24 px

Card Header Bottom Margin

16 px

Content Gap

16 px

Footer Margin

24 px

---

# 6. Navigation Layout

Sidebar Width

280 px

Collapsed Sidebar

88 px

Top Navigation Height

72 px

Bottom Mobile Navigation

72 px

Navigation Item Height

48 px

Navigation Item Gap

8 px

---

# 7. Grid System

Desktop

12 Columns

Tablet

8 Columns

Mobile

4 Columns

Grid Gutter

24 px

Grid Margin

32 px

Maximum Content Width

1440 px

---

# 8. Responsive Breakpoints

| Device | Width |
|----------|-------:|
| Mobile | 0–767 px |
| Tablet | 768–1023 px |
| Laptop | 1024–1439 px |
| Desktop | 1440 px+ |

---

# 9. Dashboard Layout

Desktop

```
--------------------------------------------------------
 Sidebar |                Main Content
         |---------------------------------------------
         | Top Navigation
         |
         | Statistics Cards
         |
         | Charts
         |
         | Recent Tasks
--------------------------------------------------------
```

---

Mobile

```
---------------------
Top Bar

Statistics

Recent Tasks

Floating Add Button

Bottom Navigation
---------------------
```

---

# 10. Task Card Layout

Padding

24 px

Gap

16 px

Border Radius

16 px

Minimum Height

140 px

Maximum Width

100%

---

Structure

```
Priority Badge

Task Title

Description

Category

Due Date

Actions
```

---

# 11. Form Layout

Gap Between Inputs

20 px

Section Gap

32 px

Button Gap

16 px

Input Height

48 px

Textarea Minimum Height

120 px

---

# 12. Modal Layout

Maximum Width

600 px

Padding

32 px

Border Radius

24 px

Header Bottom Margin

24 px

Footer Top Margin

24 px

---

# 13. Table Layout

Row Height

56 px

Column Padding

20 px

Header Height

56 px

Cell Gap

16 px

---

# 14. Chart Layout

Chart Padding

24 px

Legend Gap

16 px

Chart Height

320 px

Card Padding

24 px

---

# 15. Empty State Layout

Illustration

120 px

Gap

24 px

Button Margin

24 px

Centered both vertically and horizontally.

---

# 16. Floating Action Button

Size

56 px

Bottom Margin

24 px

Right Margin

24 px

Shadow

Medium

---

# 17. Icon Spacing

Small Icons

16 px

Regular Icons

20 px

Large Icons

24 px

Gap Between Icon and Text

8 px

---

# 18. Alignment Rules

Always align elements to the grid.

Avoid arbitrary spacing values.

Maintain equal spacing within similar components.

Use consistent left alignment for content.

Center alignment should be reserved for hero sections and empty states.

---

# 19. Layout Principles

Use whitespace intentionally.

Do not overcrowd screens.

Group related information.

Separate unrelated sections.

Visual hierarchy should guide user attention naturally.

---

# 20. Responsive Rules

Desktop

Sidebar visible.

Tablet

Sidebar collapses.

Mobile

Bottom navigation replaces sidebar.

Cards stack vertically.

Charts become full width.

Tables transform into cards where appropriate.

---

# 21. Design Tokens

--space-xs : 4px

--space-sm : 8px

--space-md : 16px

--space-lg : 24px

--space-xl : 32px

--space-2xl : 40px

--space-3xl : 48px

--space-4xl : 64px

---

# 22. Summary

The FocusFlow spacing and grid system establishes a consistent layout foundation that ensures every screen feels balanced, organized, and scalable across desktop, tablet, and mobile devices.