# HERMAS — CV | Semantic HTML Portfolio

[![Language](https://img.shields.io/badge/Language-French_(fr)-blue?style=flat-square)](https://github.com/fhermas22/hermas-cv)
[![Version](https://img.shields.io/badge/Version-2.0.0-success?style=flat-square)](https://github.com/fhermas22/hermas-cv)
[![License](https://img.shields.io/badge/License-MIT-blue?style=flat-square)](LICENSE)

A clean, responsive single-page CV/portfolio built with **semantic HTML**, modern CSS, and lightweight structure—no framework required.

## Table of Contents

- [Overview](#overview)
- [Live Preview](#live-preview)
- [Key Features](#key-features)
- [Project Structure](#project-structure)
- [Getting Started](#getting-started)
- [Semantic HTML Reference](#-semantic-html-reference)
- [Best Practices Applied](#-best-practices-applied)
- [CSS Architecture & Best Practices](#-css-architecture--best-practices)
- [License & Author](#-license)

## Overview

This project is a **single HTML page** (`index.html`) featuring a professional CV/portfolio with semantic markup excellence:

- **Personal introduction** — photo, name, title, and contact information
- **Projects** — self-contained descriptions using semantic `article` elements
- **Professional experiences** — structured with time semantics and metadata
- **Technical skills** — organized with definition lists for clarity
- **Social/professional links** — neatly grouped in the sidebar
- **Footer section** — with professional quote and copyright

Built with a focus on **semantic clarity**, **accessibility**, and **modern web standards** (no framework dependencies).

## Live Preview

Simply open `index.html` in any modern web browser to view the portfolio.

**Deployment note:** When deploying, ensure relative paths to `assets/` and `public/` directories remain intact.

## Key Features

✨ **Semantic HTML Excellence**
- Proper use of `header`, `main`, `section`, `article`, `aside`, and `footer` elements
- Meaningful content grouping for different information types

🎯 **Accessibility First**
- Fully accessible media with descriptive `alt` attributes
- Semantic `address` for contact information
- Proper time semantics with machine-readable `datetime` attributes
- Definition lists (`dl`, `dt`, `dd`) for metadata and structured content
- Custom focus rings with `focus-visible` for keyboard navigation
- Opacity adjustments for improved visual hierarchy

🔗 **Web Standards Compliance**
- External links properly secured with `rel="noopener noreferrer"`
- Clean document outline with correct heading hierarchy
- Responsive design with modern CSS (Glassmorphism effect)

📱 **Modern Design**
- Lightweight, no-framework approach
- Custom CSS with theme variables
- Dot-grid background pattern with glassmorphism effect
- Professional color palette (slate blue + warm brown)

💅 **CSS Best Practices**
- **CSS Custom Properties (CSS Variables)** for centralized theme management
- **REM-based typography** for scalable, accessible font sizing
- **Global CSS Reset** with proper box-sizing and margin/padding normalization
- **Organized stylesheet** with clear sections and meaningful comments
- **Smooth transitions** (0.3s-0.4s) for polished interactions
- **Vendor prefixes** (`-webkit-`) for cross-browser compatibility
- **Backdrop filters** for modern glassmorphism effects
- **Semantic color management** with primary and secondary color variables
- **Advanced CSS selectors** (`:focus-visible`, `:last-of-type`, `:hover`)
- **Layered box-shadows** for depth and 3D effects
- **Gradient backgrounds** for sophisticated visual elements
- **Responsive container queries** approach with max-width constraints

## Project Structure

```text
.
├── index.html
├── README.md
├── LICENSE
├── assets/
│   └── images/
│       ├── hermas/
│       │   └── profile-pic.webp
│       └── projects/
│           └── project images...
├── public/
│   └── favicon.ico
└── styles/
    └── style.css
```

## Getting Started

### Quick Start

Since this is a static site, simply:
1. Navigate to the project directory
2. Open `index.html` in your web browser

### Recommended Development Setup

For local development with live reload:
- Use the **VSCode Live Server** extension to avoid caching issues and enable hot refresh during editing

### Browser Compatibility

Works on all modern browsers supporting:
- CSS custom properties (CSS variables)
- Backdrop filter / Glassmorphism
- ES6+ (if future enhancements are added)

## 📚 Semantic HTML Reference

This section documents the semantic HTML tags used throughout the project and explains their purpose and benefits.

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
- Contains the main sections of the CV: About, Skills, Experiences, Education, Projects, Languages.

### `section`
Groups related topics, each with a heading.
- In this project:
  - `section#about`
  - `section#skills`
  - `section#experiences`
  - `section#education`
  - `section#projects`
  - `section#languages`

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

### `figure` (and optional `figcaption`)
Used to semantically group media with related context.
- In this project, media can be wrapped in a `figure` element (optionally with `figcaption`) so the image stays logically connected to its description.


## ✅ Best Practices Applied

The markup follows industry-standard semantic HTML best practices:

1. **Clear semantic document structure**
   - Page regions properly defined with `header`, `main`, `aside`, and `footer`
   - Ensures proper interpretation by screen readers and search engines

2. **Proper heading hierarchy**
   - Each section includes appropriate `h2` headings
   - Creates an accessible and SEO-friendly document outline

3. **Self-contained content blocks**
   - Projects and experiences use `article` elements
   - Allows content to be independently syndicated or reused

4. **Semantic content models**
   - Contact details properly wrapped in `address`
   - Metadata and label-value patterns use `dl`, `dt`, `dd`
   - Temporal information marked with `time` and `datetime` attributes

5. **Accessibility-first media**
   - All images include descriptive `alt` text
   - Media grouped with `figure` and optional `figcaption` for semantic context

6. **Security best practices**
   - External links that open in new tabs include `rel="noopener noreferrer"`
   - Protects against security vulnerabilities

7. **Well-organized content lists**
   - Projects, experiences, and social links use semantic `ul` and `li` elements

## 🎨 CSS Architecture & Best Practices

The stylesheet demonstrates professional CSS organization and modern techniques:

### **1. CSS Custom Properties (Variables)**
```css
:root {
    --primary-color: #1E293B;
    --secondary-color: #854D0E;
    --bg-color: #F8FAFC;
    --font-title: 'Poppins', sans-serif;
    --font-body: 'Inter', sans-serif;
}
```
- Centralized color and typography management
- Easy theme switching and maintenance
- Semantic variable names for clarity

### **2. Global CSS Reset**
- Universal reset: `margin: 0`, `padding: 0`, `box-sizing: border-box`
- Ensures consistency across all browsers
- Foundation for predictable layouts

### **3. Responsive Typography Scale**
- **Base font size:** 0.938rem (15px) using REM units
- **H1:** 2rem (32px) | **H2:** 1.375rem (22px) | **H3:** 1.125rem (18px)
- Proper line-height values (1.2–1.6) for readability
- Maintains accessibility with scalable units

### **4. Modern Visual Effects**
- **Glassmorphism design:**
  - `backdrop-filter: blur(2px)` with vendor prefix
  - `border: 1px solid rgba(255, 255, 255, 0.6)` for frosted glass look
  - Layered box-shadows for soft-3D depth effect

- **Background patterns:**
  - Radial-gradient dot grid pattern
  - Linear-gradient horizontal separators

### **5. Advanced Selectors & Pseudo-classes**
- `:focus-visible` for keyboard accessibility (3px outline with custom shadow)
- `:last-of-type` for smart border/spacing removal
- `:hover` with smooth transitions for interactive feedback

### **6. Smooth Interactions**
- Transition framework: `all 0.3s-0.4s ease-in-out`
- Enhances UX without being distracting
- Applied to links, buttons, and interactive elements

### **7. Semantic Color Management**
- **Primary color:** Dark slate (#1E293B) for text/structure
- **Secondary color:** Warm brown (#854D0E) for accents/highlights
- **Background:** Light blue-gray (#F8FAFC) for contrast

### **8. Typography Best Practices**
- **Font families:** Poppins (titles) + Inter (body)
- **Letter-spacing:** Fine-tuned (`-0.5px`) for headers
- **Opacity variations:** Used for hierarchy (`opacity: 0.85-0.9`)
- **Line-height ratios:** Optimized per heading level

### **9. Box-Shadow Layering**
- Multiple shadow layers for depth:
  - Ambient shadows (subtle)
  - Colored tints (bronze glow effects)
  - Light reflections (top-left highlighting)

### **10. Vendor Prefixes**
- `-webkit-backdrop-filter` for Safari compatibility
- Ensures glassmorphism works across modern browsers

### **11. Organized File Structure**
Stylesheet divided into logical sections with clear comments:
- Global theme variables & reset
- Typography & links
- Structural spacing
- Component-specific styles (header, sections, footer)
- Accessibility enhancements

### **12. Performance Considerations**
- No external icon libraries (lightweight)
- Efficient use of gradients instead of image assets
- CSS-only animations (no JavaScript required)
- Minimal repaints with optimized selectors

## 📄 License

This project is licensed under the [MIT License](LICENSE) — feel free to use, modify, and distribute.

## 👤 Author

- **Developer:** [fhermas22](https://github.com/fhermas22) — Hermas Francisco
- **Portfolio:** [hermas.vercel.app](https://hermas.vercel.app)
- **GitHub:** [@fhermas22](https://github.com/fhermas22)

---

**Version:** 2.0.0 | Last updated: June 2026