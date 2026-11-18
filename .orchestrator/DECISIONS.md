# Decisions Log

## v1.0 - 2026-09-05

- Use Next.js App Router with TypeScript because the workspace is empty and the site benefits from route-level metadata and image handling.
- Use local structured content in `lib/content.ts`; no CMS or database.
- Use a restrained editorial system: warm mineral white, ink, muted clay, and moss accents; no decorative gradients.
- Keep `Work` as a dedicated index and make `Contact` an anchor to the global footer.
- Use a single reusable project template with optional sections so missing placeholder content does not create empty fake narratives.
- Treat personal contribution as first-class project metadata and never imply unprovided facts.
- Foundation and all page routes are owned by one integration owner in this workspace because isolated worktrees are not available.

## v1.1 - 2026-09-05

- The homepage first viewport must combine identity with the strongest project; the former biography-first full-screen hero is removed.
- Project 01 is the featured hero and receives approximately 80% of the desktop visual field; Projects 02-04 remain in the following selected-work section.
- On mobile, identity stays concise and Project 01 begins directly beneath it, with no biography before the work.
