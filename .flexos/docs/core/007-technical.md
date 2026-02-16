---
id: "007-technical"
title: "Technical Architecture"
type: doc
subtype: core
status: complete
sequence: 7
tags: [stack, deployment, seo]
---

# Technical Architecture

> Engineering standards and stack definition for high-performance delivery.

## Technology Stack

- **Framework:** Astro 5 (Static Site Generation).
- **Language:** TypeScript (Strict mode enabled).
- **Styling:** Tailwind CSS v4.
- **Icons:** Lucide React or Phosphor Icons.
- **Deployment:** Vercel (Git-based workflow).

## SEO Strategy

### Meta Tags & Structure
- **Title Template:** `%s | The CKB Firm`
- **Canonical URLs:** Auto-generated based on site URL.
- **Sitemap:** `sitemap-index.xml` generated at build time.
- **Robots.txt:** Allow all, disallow `/admin`.

### Schema Markup
Implementation of structured data for local search dominance:
```json
{
  "@context": "https://schema.org",
  "@type": "LegalService",
  "name": "The CKB Firm",
  "address": {
    "@type": "PostalAddress",
    "addressLocality": "Chicago",
    "addressRegion": "IL"
  },
  "priceRange": "$$"
}
```

## Performance Targets

- **Core Web Vitals:** All "Good" (LCP < 2.5s, CLS < 0.1).
- **Lighthouse Score:** 95+ across Performance, Accessibility, Best Practices, and SEO.
- **Images:** Automatic conversion to WebP via Astro `<Image />` component.

## Accessibility (a11y)

- **Standard:** WCAG 2.1 AA Compliance.
- **Requirements:**
    - Semantic HTML5 elements (`<main>`, `<nav>`, `<article>`).
    - Contrast ratio > 4.5:1 for text (verified for `#1B365D` on `#FBFBFB`).
    - Focus indicators visible on all interactive elements.
    - Alt text required for all content images.