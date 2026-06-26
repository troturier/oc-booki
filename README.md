# Booki

A responsive landing page built with **HTML5** and **CSS3** only, based on the UI mockups validated by the Product team. This is a first version intended to validate the interface — no JavaScript, no backend logic.

## Table of Contents

- [Project Overview](#project-overview)
- [Tech Stack & Constraints](#tech-stack--constraints)
- [Design Specs](#design-specs)
    - [Colors](#colors)
    - [Typography](#typography)
    - [Icons](#icons)
- [Responsive Strategy](#responsive-strategy)
    - [Breakpoints](#breakpoints)
    - [Min / Max Width](#min--max-width)
- [Functional Specifications](#functional-specifications)
    - [Search Field](#search-field)
    - [Header Navigation Links](#header-navigation-links)
    - [Accommodation & Activity Cards](#accommodation--activity-cards)
    - [Search Filters](#search-filters)
- [Code Guidelines](#code-guidelines)
- [Browser Compatibility](#browser-compatibility)

## Github Repository

The project's repository is available on [Github](https://github.com/troturier/oc-booki).

## Project Overview

Booki is a travel booking interface allowing users to search for accommodations and activities by city. This iteration focuses exclusively on layout, styling, and responsiveness — the search and filtering features are **non-functional placeholders**, meant only to validate the visual design.

Three mockups were provided by the UI designer: **desktop**, **tablet**, and **mobile**.

## Tech Stack & Constraints

- **HTML5** + **CSS3** only
- **No CSS framework** (Bootstrap, Tailwind CSS, etc.)
- **No CSS preprocessor** (Sass, Less, etc.)
- **No JavaScript** or any other language
- Layout built with **Flexbox**
- Approach: **desktop-first** (desktop layout implemented first, then tablet, then mobile, via Media Queries)

## Design Specs

### Colors

| Usage | Color | Hex |
|---|---|---|
| Primary blue | 🔵 | `#0065FC` |
| Light blue | 🔵 | `#DEEBFF` |
| Background gray | ⚪ | `#F2F2F2` |

### Typography

- Font: **[Raleway](https://fonts.google.com/specimen/Raleway)**, imported via Google Fonts.

### Icons

- Icon library: **[Font Awesome](https://fontawesome.com/)**

## Responsive Strategy

### Breakpoints

| Range | Target |
|---|---|
| `> 1024px` | Desktop |
| `>= 768px` and `<= 1024px` | Tablet |
| `< 768px` | Mobile |

### Min / Max Width

- **Max content width:** `1440px` — beyond this, white margins appear on the sides.
- **Min supported width:** `320px` — behavior below this width is not guaranteed.

## Functional Specifications

### Search Field

- Text input field, editable by the user.
- Wrapped in a `<form>` element.
- **Not functional** in this version — UI validation only.

### Header Navigation Links

- The "Accommodations" and "Activities" texts in the header are links.
- They scroll/link respectively to the **"Accommodations in Marseille"** and **"Activities in Marseille"** sections.

### Accommodation & Activity Cards

- Each card must be **entirely clickable**, not just the title.
- Links are placeholders for now (`href="#"`).

### Search Filters

- Accommodations can be filtered by theme (e.g. budget, atmosphere).
- Filters must **change color on hover**.
- **Not functional** in this version — UI validation only.

## Code Guidelines

- Code must be valid against the **W3C HTML** and **W3C CSS** validators.
- HTML must **not contain inline CSS** (no `style` attributes).
- No HTML duplication between desktop, tablet, and mobile views — *except* for the search form's "Search" label and magnifying glass icon, which may be handled separately for responsive purposes.
- Target elements with **CSS classes**, not element selectors.
- Avoid duplicating CSS classes: if multiple elements share the same styling, reuse a single class rather than repeating it across several.
- Use **semantic HTML tags**, at minimum: `header`, `nav`, `h1`–`h3`, `main`, `section`, `article`, `footer`.

## Browser Compatibility

The page must be tested and compatible with the latest versions of:
- Google Chrome
- Mozilla Firefox