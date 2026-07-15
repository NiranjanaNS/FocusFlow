# FocusFlow – Typography System

**Project:** FocusFlow  
**Document Version:** 1.0  
**Status:** Draft

---

# 1. Purpose

Typography defines how text is displayed throughout FocusFlow.

A consistent typography system improves readability, creates visual hierarchy, and provides a cohesive user experience across desktop and mobile devices.

---

# 2. Design Goals

The typography system should be:

- Clean
- Modern
- Professional
- Readable
- Accessible
- Scalable
- Consistent

---

# 3. Primary Typeface

## Inter

Why Inter?

- Designed specifically for digital interfaces
- Excellent readability at small sizes
- Clean and modern appearance
- Wide range of font weights
- Free and open source
- Popular in modern SaaS applications

Google Fonts

https://fonts.google.com/specimen/Inter

---

# 4. Fallback Fonts

font-family:

Inter,
system-ui,
Segoe UI,
Roboto,
Helvetica,
Arial,
sans-serif

---

# 5. Font Weights

| Weight | Value | Usage |
|---------|------:|-------|
| Light | 300 | Rare decorative text |
| Regular | 400 | Body text |
| Medium | 500 | Labels |
| SemiBold | 600 | Buttons & Cards |
| Bold | 700 | Headings |
| Extra Bold | 800 | Hero Titles |

---

# 6. Typography Scale

| Element | Size | Weight | Line Height |
|----------|------|---------|------------|
| Display | 48 px | 800 | 56 px |
| H1 | 36 px | 700 | 44 px |
| H2 | 30 px | 700 | 38 px |
| H3 | 24 px | 600 | 32 px |
| H4 | 20 px | 600 | 28 px |
| H5 | 18 px | 600 | 26 px |
| Body Large | 18 px | 400 | 28 px |
| Body | 16 px | 400 | 24 px |
| Small | 14 px | 400 | 20 px |
| Caption | 12 px | 400 | 16 px |

---

# 7. Letter Spacing

| Element | Letter Spacing |
|----------|----------------|
| Display | -1 px |
| Headings | -0.5 px |
| Body | 0 px |
| Small Text | 0.2 px |
| Buttons | 0.3 px |

---

# 8. Text Colors

Primary Text

#0F172A

Secondary Text

#64748B

Disabled Text

#CBD5E1

Inverse Text

#FFFFFF

Error Text

#EF4444

Success Text

#22C55E

---

# 9. Text Alignment

Default:

Left aligned

Center alignment only for:

- Empty states
- Hero sections
- Authentication screens

Avoid justified text.

---

# 10. Text Styles

## Display

Used for:

- Landing page
- Hero section

---

## Headings

Used for:

- Screen titles
- Cards
- Dashboard sections
- Analytics

---

## Body

Used for:

- Descriptions
- Settings
- Task details
- Notes

---

## Labels

Used for:

- Form labels
- Statistics
- Inputs

---

## Caption

Used for:

- Dates
- Metadata
- Helper text
- Footnotes

---

# 11. Button Typography

Size

16 px

Weight

600

Letter spacing

0.3 px

Text Transform

Sentence Case

Example

Create Task

Not

CREATE TASK

---

# 12. Input Typography

Font Size

16 px

Weight

400

Placeholder

Secondary Text

---

# 13. Dashboard Typography

Page Title

36 px

Card Title

20 px

Statistics

30 px

Card Description

14 px

Navigation

16 px

---

# 14. Responsive Typography

## Desktop

Display

48 px

H1

36 px

Body

16 px

---

## Tablet

Display

42 px

H1

32 px

Body

16 px

---

## Mobile

Display

36 px

H1

28 px

Body

16 px

Caption

12 px

---

# 15. Accessibility

- Maintain WCAG AA contrast ratio
- Never use font sizes below 12 px
- Use line heights between 1.4 and 1.6 for paragraphs
- Avoid long paragraphs
- Limit line length to approximately 70 characters where practical

---

# 16. Typography Tokens

--font-family

Inter

--font-display

48 px

--font-h1

36 px

--font-h2

30 px

--font-h3

24 px

--font-body

16 px

--font-small

14 px

--font-caption

12 px

---

# 17. Usage Guidelines

Use bold text only for emphasis.

Do not use more than three font weights on a single screen.

Maintain consistent spacing between headings and content.

Avoid using ALL CAPS except for small status badges when necessary.

---

# 18. Summary

The FocusFlow typography system provides a scalable and accessible text hierarchy that supports readability across desktop, tablet, and mobile interfaces while maintaining a modern and professional appearance.