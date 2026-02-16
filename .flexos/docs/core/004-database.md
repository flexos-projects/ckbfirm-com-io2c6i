---
id: "004-database"
title: "Database & Data Model"
type: doc
subtype: core
status: complete
sequence: 4
tags: [schema, content-collections, astro]
---

# Database & Data Model

> Data schemas using Astro Content Collections to structure legal expertise and team data.

## Content Collections

### 1. Blog/Insights Collection (`src/content/blog`)
Used for industry updates and SEO articles.
- **title:** string (e.g., "5 Key Strategies for Successful Commercial Debt Recovery")
- **description:** string (Meta description)
- **pubDate:** date
- **author:** string (Reference to Attorney name)
- **tags:** array<string> (e.g., "Debt Recovery", "Illinois Law")
- **image:** string (Cover image path)
- **featured:** boolean

### 2. Team Collection (`src/content/team`)
Stores attorney profile data.
- **name:** string (e.g., "Michael Baim")
- **role:** string (e.g., "Managing Partner")
- **image:** string
- **bio:** markdown
- **email:** string
- **linkedin:** string (optional)
- **admissions:** array<string> (Bar admissions)

### 3. Services Collection (`src/content/services`)
- **title:** string
- **slug:** string (e.g., "commercial-litigation")
- **icon:** string
- **shortDescription:** string
- **fullDescription:** markdown

## Data Sources & Integrations

- **Source:** Local Markdown/MDX files within the repository.
- **Forms:** Contact form submissions handled via Netlify Forms or Formspree (POST request to endpoint).
- **Google Maps:** Embedded via iframe using address data defined in global site config.