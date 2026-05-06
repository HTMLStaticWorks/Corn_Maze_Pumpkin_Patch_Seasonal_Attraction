# Universal HTML Template Development Rules & Quality Standards

This document serves as the mandatory checklist and architectural guide for all HTML template projects. Following these rules ensures consistency, high performance, and premium quality suitable for platforms like ThemeForest and TemplateMonster.

## 1. Core Architecture
- **Semantic HTML**: Use proper HTML5 elements (`<header>`, `<nav>`, `<main>`, `<section>`, `<footer>`).
- **Responsive Design**: Mobile-first approach. Breakpoints:
  - Mobile: 280px 640px
  - Tablet: 640px - 1050px
  - Desktop: 1050px - 1280px
  - Large: > 1280px

  in mobile and tablet need offcanvas navbar which should be visible 
  when click on 3 dash icon in right top cornor.
  and when click on 3 dash icon it should close offcanvas navbar.
  in desktop navbar should be visible always.
- **Accessibility**: WCAG 2.1 AA compliance. Minimum touch target 44px.
- **File Structure**:
  - `/assets/css/`: `style.css`, `dark-mode.css`, `rtl.css`
  - `/assets/js/`: `main.js`
  - `/assets/images/`: Optimized WebP formats.
  - `index.html`: Main landing page in root.
  - `*.html`: All sub-pages in root (no /pages/ subdirectory).

## 2. Design & UI Excellence
- **Theming**: Implement Dark/Light mode toggle with system preference detection.
- **RTL Support**: Full compatibility for Arabic/Hebrew (mirrored layouts, icons, and text alignment).
- **Typography**: Max 2-3 Google Fonts. No browser defaults.
- **Spacing**: 8px base grid system for consistent margins/padding.
- **Aesthetics**: Use smooth gradients, micro-animations, and hover effects. Avoid generic colors.

## 3. SEO & Performance
- **Meta Tags**: Unique Title (max 60 chars) and Description (150-160 chars) per page.
- **Hierarchy**: Single `<h1>` per page, logical heading order (H2 -> H3).
- **Performance**: 
  - PageSpeed Score: 90+
  - LCP: < 2.5s
  - CLS: < 0.1
- **Structured Data**: JSON-LD for business/event info.

## 4. Common Mistake Prevention (QA Checklist)
- [ ] **Navbar**: Hamburger menu functional on all mobile devices; no overlapping elements.
- [ ] **Forms**: Client-side validation with user-friendly error messages.
- [ ] **CTAs**: Correct redirects (e.g., Contact buttons shouldn't go to Login).
- [ ] **Alignment**: "Remember Me" and "Forgot Password" checkboxes/links aligned correctly.
- [ ] **Dashboard**: Sidebar toggle visible on tablets; top-right controls present.
- [ ] **Imagery**: High-fidelity, niche-specific images. No repeated placeholders.

## 5. Required Pages (Standard Multi-purpose)
- **Home Page(s)**: Landing & Niche-specific.
- **About Us**: Mission, Team, Testimonials.
- **Services**: Grid/List and Detail pages.
- **Blog**: List and Full Post pages.
- **Contact**: Map, Form, Social links.
- **Utility**: 404, Login/Register, Coming Soon, Pricing.
- **Admin Dashboard**: Analytics, User/Order management.
