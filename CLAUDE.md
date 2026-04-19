# Portfolio Page — CLAUDE.md

## Project Overview

A personal portfolio page for a frontend developer. Single-page site with smooth scrolling sections.

## Tech Stack

- **Framework:** Astro
- **Styling:** Tailwind CSS
- **Language:** TypeScript (minimal, only where helpful)
- **Package manager:** Bun
- **Formatter:** Prettier (with `prettier-plugin-astro`), print width 140

## Design Guidelines

- Minimalistic and clean aesthetic
- **Dark mode by default**, light mode toggle
- Accent color: menthol/mint (approx. `#3EB489` or similar — confirm with user)
- Minimal top navbar (not bold/heavy styled)
- **Smooth scrolling animations** are a key focus — sections and elements should animate in as the user scrolls
- No unnecessary decorative clutter — animations should feel purposeful and elegant

## Page Structure (single page)

1. **Navbar** — minimal, top of page, links to sections
2. **About** — short personal intro
3. **Work Experience** — jobs with project descriptions
4. **Skills** — list of technologies and tools
5. **Contact** — way to reach the developer

## Commands

```bash
# Install dependencies
bun install

# Start dev server
bun dev

# Build for production
bun run build

# Preview production build
bun run preview

# Format
bunx prettier --write src/
```

## Conventions

- All components live in `src/components/`
- Sections are individual Astro components composed in `src/pages/index.astro`
- Tailwind dark mode strategy: `class` (toggled via JS on `<html>`)
- Keep components small and focused — one section per file
- TypeScript: prefer `type` over `interface`; use ES6 arrow function syntax
