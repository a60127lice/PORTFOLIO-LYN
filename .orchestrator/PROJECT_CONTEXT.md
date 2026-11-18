# Project Context

## Context Version

`v1.1` - 2026-09-05

## Purpose

Build a production-ready portfolio website for Chang Ya-Lin, an Interior Designer / Spatial Designer based in Glasgow, UK. The primary goal is to support applications to UK interior-design and spatial-design studios.

## Audience

UK design studios, architects, recruiters, hiring managers, and potential collaborators.

## Confirmed Visual Direction

- Contemporary editorial and architectural minimalism.
- Calm, spacious, image-led layouts with precise alignment.
- Neutral palette, strong typographic hierarchy, large project imagery.
- The interface is a quiet exhibition system around the work.
- Avoid generic templates, dashboard/card layouts, gradients, glassmorphism, heavy shadows, excessive colour, invented claims, and unnecessary animation.

## Required Pages and Sections

- Home: Hero, Selected Work, How I Work, Experience, About preview, Contact/footer.
- Work index.
- Four reusable project case-study routes using clearly labelled placeholders.
- About page.
- CV link/download placeholder.
- Contact through footer and navigation.
- Useful 404 page.

## Technical Constraints

- Empty workspace: Next.js was selected initially, but Node/npm/npx are unavailable in the environment. A dependency-free static implementation was used so the site is immediately previewable; migration to Next.js remains straightforward if Node is installed.
- Keep dependencies minimal.
- Separate content from layout logic.
- Responsive targets: 320, 375, 768, 1024, and 1440px.
- Use semantic HTML, responsive images, lazy loading below the fold, stable image dimensions, and reduced-motion support.
- Do not add CMS, database, authentication, or complex state management.

## Content Status

Final project content and assets will be supplied later. Do not invent project facts, employers, awards, clients, qualifications, outcomes, or responsibilities. Placeholder fields must remain clearly labelled and easy to replace.

## Accessibility Requirements

- Semantic landmarks and logical headings.
- Keyboard-accessible navigation and mobile menu with visible focus states.
- Skip link, useful image alt text, sufficient contrast, touch-friendly controls.
- No essential hover-only interactions.
- Respect `prefers-reduced-motion`.
- Drawings must have a readable enlarge/zoom path.

## Acceptance Criteria

- Recruiters understand identity, role, and location within 5-10 seconds.
- Strongest work is immediately reachable.
- Project role, contribution, process, technical ability, and experience are scannable.
- All required routes and links work.
- Desktop, tablet, and mobile compositions are intentional and free of overflow/clipping.
- Lint, typecheck, production build, route checks, browser smoke tests, accessibility checks, and responsive inspection are completed where tooling allows.
- Placeholder projects are replaceable from one obvious content location.

## Explicit Exclusions

- No fabricated portfolio narratives or professional facts.
- No CMS, database, auth, contact backend, or external service integration unless later requested.
- No autoplay audio/video, forced scrolling, scroll hijacking, heavy parallax, cursor gimmicks, or long preloaders.

## Current State

Homepage hero revised in `v1.1`: identity and Project 01 now share the first viewport, with the project visually dominant. Static route/link verification remains valid; browser checks at 375px and 1440px confirm the featured image placement and no horizontal overflow. Node-based lint, typecheck, and production build remain unavailable until Node.js is installed.
