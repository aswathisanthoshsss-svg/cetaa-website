# CETAA Website — Frontend

Static HTML/CSS/JS site for the College of Engineering Trivandrum Alumni Association (CETAA), covering the homepage and the Diamond Jubilee Hall renovation campaign page.

## Structure

```
CETAA-WEBSITE/
├── index.html          → Homepage (Navbar, Hero, About, Mission & Vision,
│                          Legacy Timeline, President's & Secretary's Message,
│                          Executive Committee, Distinguished Alumni,
│                          CETAA Day & Community, CET Chronicle, Gallery,
│                          Call to Action, Footer)
├── renovation.html      → Diamond Jubilee Hall page (Navbar, Hero Banner,
│                          Project Overview, Why Renovation?, Objectives,
│                          Current Hall, Renovation Scope, Project Highlights,
│                          Before/After Concept Visuals, Support the Project,
│                          Contact, Footer)
├── css/
│   ├── style.css        → Design tokens, layout, and component styles
│   └── responsive.css   → Breakpoints (1024px / 880px / 720px / 540px)
├── js/
│   └── script.js        → Mobile nav, scroll reveals, animated counters,
│                          gallery filter tabs, before/after drag slider
└── assets/               → Images organized by section (see below)
```

## Design system

- **Palette:** deep pine green (`#0B3D2E`) navigation/footer, primary green (`#1F7A4D`) for actions, soft mint (`#E8F3EC`) section backgrounds, warm paper (`#F7F5EF`) base, and a brass accent (`#C9A66B`) used throughout for the "heritage" details (dividers, plaques, timeline dots).
- **Type:** Fraunces (serif display) for headings, Inter for body copy, Space Mono for eyebrow labels and the "ledger divider" section breaks — a nod to the printed CET Chronicle.
- **Signature elements:**
  - The **Legacy Timeline** (home page) — a vertical brass/green thread connecting real institutional milestones.
  - The **Before/After compare slider** (renovation page) — drag to compare the hall's current state against the renovation concept.

## Replacing placeholder assets

All images in `/assets` are auto-generated color placeholders labeled with their filename, sized correctly for their slot. Drop in real photography using the same filenames and folder paths and everything will update with no code changes. The same goes for `assets/chronicle/CET-Chronicle.pdf`, which is a one-page placeholder.

## Notes

- Both pages share `css/style.css`, `css/responsive.css`, and `js/script.js` — edit once, both pages update.
- All copy (leadership names, timeline dates, budget figures, etc.) is sample content written for this template. Replace with CETAA's real details before publishing.
