# QA Report

Status: implemented; partially verified due unavailable Node.js tooling.

## v1.1 featured-project revision

- At 1440px, the Project 01 feature image occupies the dominant hero field beside restrained identity text.
- At 375px, identity appears first and Project 01 begins directly below it within the opening viewport.
- Project 01 is a direct tap target and resolves to `projects/project-01.html`.
- The revised homepage has no horizontal overflow at 375px or 1440px.

## Verified

- 9 required HTML routes exist.
- 79 local links resolve, including all project navigation and the CV placeholder PDF.
- Browser page title, semantic landmarks, headings, navigation links, project links, CV link, and contact links are present on Home.
- At 375px browser viewport: no horizontal overflow after repair (`scrollWidth` equals content width).
- Mobile menu opens with `aria-expanded="true"` and closes with Escape to `aria-expanded="false"`.
- Placeholder content remains explicit and no project facts were invented.

## Partially verified

- Keyboard semantics and reduced-motion CSS are implemented, but a full automated accessibility scan was not available.
- Desktop/tablet CSS targets are implemented, but browser screenshots at every required width were not run.
- The CV PDF is a deliberately blank placeholder and must be replaced with the real CV.

## Planned verification

- `npm run lint`
- `npm run typecheck`
- `npm run build`
- Route and internal-link smoke tests.
- Browser checks at 320, 375, 768, 1024, and 1440px.
- Keyboard navigation, mobile-menu Escape/focus behavior, reduced motion, and focus visibility.
- Accessibility scan for serious/critical violations.
- Console/runtime error inspection.

## Not verified / blocked

- `npx create-next-app` could not run because `npx`, `node`, and `npm` are unavailable on PATH.
- `npm run lint`, typecheck, production build, Lighthouse, and automated E2E/accessibility suites cannot run until Node.js is installed.
- The local Python preview server exited immediately, so browser verification used the local HTML file directly.

## Known limitations

- Final project images and facts are not available.
- CV PDF, email address, LinkedIn URL, and favicon are placeholders until supplied.

## Project 02 content and asset verification - 2026-10-14

- Parsed project facts were added from the supplied eight-page PDF and the user's accompanying delivery notes.
- Confirmed facts now represented: Taichung, Taiwan; commercial hospitality and wellness; 130 sqm; £37,500 budget; completed October 2023; concept design, contractor procurement and site supervision; dual-use cafe and salon; statutory approvals; high-voltage supply upgrade; MEP overhaul; acoustic control; value-engineering strategy.
- The user-provided delivery scope is represented explicitly: coordination with the carpenter, deliveries and owner.
- `hero-image.jpg` and `render-view-01.jpg` were found to be byte-for-byte duplicates by SHA-256 and `render-view-01.jpg` was removed from the displayed page.
- Final Project 02 page: 6 displayed image references, 6 unique sources, 6 existing files, 0 duplicate hashes.
- Browser check at 375px and 1440px: 6/6 images loaded after forcing eager loading for the test, 6 unique sources, and no horizontal overflow.
- Browser content check: title, project facts, delivery coordination and all process sections present at both widths.
