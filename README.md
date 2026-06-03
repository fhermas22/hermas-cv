# HERMAS — CV (Semantic HTML Portfolio)

A clean, responsive single-page CV/portfolio built with **semantic HTML** and lightweight structure (no framework required).

## Table of Contents
- [Overview](#overview)
- [Live/Preview](#livepreview)
- [Key Features](#key-features)
- [Project Structure](#project-structure)
- [How to Run Locally](#how-to-run-locally)
- [Semantic HTML Mini‑Documentation](#semantic-html-mini-documentation)
- [Semantic Best Practices Used](#semantic-best-practices-used)
- [Credits](#credits)

## Overview
This project is a **single HTML page** (`index.html`) that presents:
- Personal introduction (photo, name, title, contact)
- Projects (each described with `article`)
- Professional experiences (each described with `article` + `time`)
- Technical skills (using definition lists)
- Social/professional links (in an `aside`)
- Footer quote and copyright

The markup focuses on **clear sectioning**, **meaningful elements**, and **accessible structure**.

## Live/Preview
Open: `index.html` in a browser.

> If you deploy this repository, make sure the paths to `assets/` and `public/` remain unchanged.

## Key Features
- **Semantic layout** using:
  - `header`, `main`, `section`, `article`, `aside`, `footer`
- **Meaningful grouping** for content types (projects, experiences, skills)
- **Contact semantics** with `address`
- **Time semantics** with `time datetime="..."`
- **Description lists** for label/value patterns (`dl`, `dt`, `dd`)
- **Accessible media** (`img` with `alt`)
- External links include `target="_blank"` and `rel="noopener noreferrer"` where applicable

## Project Structure
```text
.
├── index.html
├── README.md
├── assets/
│   └── images/
│       ├── hermas/
│       │   └── profile-pic.webp
│       └── projects/
│           └── project images...
└── public/
    └── favicon.ico
```

## How to Run Locally
Because this is a static site, you can run it by opening the HTML file:
1. Go to the project folder
2. Open `index.html` with your browser

Optional (recommended for local preview):
- Use VSCode “Live Server” to avoid caching issues while iterating.

## Semantic HTML Mini‑Documentation
Below is a quick documentation of the semantic HTML tags used in `index.html` and why they matter.

### `header`
Used for the top-of-page identity area.
- Contains:
  - profile image (`img`)
  - main title (`h1`)
  - subtitle (`p`)
  - contact information inside `address`

### `address`
Used for contact details (email, phone, location).
- Helps browsers and assistive technologies understand the content is contact-oriented.

### `main`
Wraps the primary page content.
- Contains the main sections of the CV: About, Projects, Experiences, Skills.

### `section`
Groups related topics, each with a heading.
- In this project:
  - `section#about`
  - `section#projects`
  - `section#experiences`
  - `section#skills`

### `h1` / `h2` / `h3`
Heading hierarchy:
- `h1`: page/person main name
- `h2`: major blocks (About, Projects, etc.)
- `h3`: individual items (e.g., project name, experience role)

### `article`
Represents self-contained, reusable pieces of content.
- Used inside:
  - Projects list (`article` per project)
  - Experiences list (`article` per job/role)

### `ul` / `li`
Used for lists of homogeneous items:
- Projects
- Experiences
- Skills groups
- Social links

### `dl` / `dt` / `dd`
Used for label/value information.
- Example patterns:
  - Project “Stack Technique”
  - Experience “Type de contrat”, “Structure”, “Période”
  - Skills categories (“Mobile”, “Frontend”, etc.)

### `time`
Used for machine-readable dates.
- Example:
  - `<time datetime="2025">2025</time> - Présent`

### `aside`
Used for complementary content.
- Here, the “Réseaux & Liens Professionnels” block.

### `footer`
Contains page closure information.
- Includes a quote (`blockquote`) and copyright.

### `blockquote`
Indicates a quotation.
- Uses `cite` to reference the source URL (as present in the markup).

### `img` with `alt`
Accessible images.
- Each project photo has an `alt` description.

## Semantic Best Practices Used
These are the semantic best practices reflected in the existing markup:

1. **Clear semantic sectioning**
   - Major regions use `header`, `main`, `aside`, `footer`.

2. **Section headings are present**
   - Each `section` includes a relevant `h2`, improving document outline.

3. **Self-contained content uses `article`**
   - Projects and experiences are independent content units.

4. **Correct content models**
   - Contact information is inside `address`.
   - Label/value details use `dl` + `dt` + `dd`.
   - Dates are represented with `time`.

5. **Accessible media**
   - Images include `alt` attributes.

6. **External link safety**
   - External links that open new tabs use `rel="noopener noreferrer"`.

7. **Readable list structure**
   - Projects/experiences/social links are organized with `ul > li`.

## Credits
- Built by **fhermas22** — [github.com/fhermas22](https://github.com/fhermas22)
- Website Portfolio **Hermas Francisco** — [hermas.vercel.app](https://hermas.vercel.app)

