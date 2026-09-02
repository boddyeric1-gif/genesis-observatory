# Genesis Observatory

**A living digital civilization in a single self-contained HTML file.**

Genesis Observatory is a real-time simulation of an evolving society inside a sealed bio-dome. Citizens are born, form relationships, build structures, invent ideologies, mentor the young, age, die, leave legacies, and occasionally create lasting traditions and entirely new factions. Everything runs client-side with no server required.

## Features

- **Emergent society** — Citizens have roles (Artisan, Inventor, Philosopher, Researcher, Builder, Steward), motivations, ideologies, traits, memories, relationships, and goals.
- **Dynamic structures** — Aether Reactors, Energy Grids, Bio-Nurseries, Ideological Totems, faction outposts. Structures age, get restored, accumulate upgrades, and can carry ancestral legacy bonuses.
- **Ideology system** — Starting factions (Techno-Expansionist, Knowledge-Seeker, Social-Harmonizer, Resource-Seeker, Resource-Harmonizer, etc.) can synthesize into permanent Traditions and Ascended hybrid ideologies with their own colors, structures, and outposts.
- **Territory** — The dome is divided into a grid; factions claim physical ground and gain home-turf relationship advantages.
- **Mentor bonds** — Elders take on mentees of the same ideology, transferring knowledge and contribution.
- **Natural mortality + resource death** — Citizens have a real maxAge and can also die of energy exhaustion.
- **The Chronicle** — Automatic narrative history of the civilization, chaptered by era, grounded only in recorded events.
- **Player agency** — Limited but meaningful: once-per-era Sponsorship of a citizen.
- **Offline progress** — The simulation catches up when you return, with proper compound probability for mortality.
- **AI-optional enrichment** — Optional Gemini integration for richer Analyst reports, obituaries, and Chronicle narration (falls back cleanly if unavailable).
- **Fully standalone** — Tailwind, Font Awesome, and GSAP are embedded. No external CDN dependency required for core function.

## How to run

Just open `index.html` in any modern browser.

No build step, no server, no install.

## Saving & Sharing

- The game autosaves to `localStorage`.
- Use **Export JSON** to download a full snapshot (simulation state + the entire codebase).
- Use **Import JSON** to restore a previous civilization on any copy of the file.
- A sample civilization is included as `sample-save.json`.

## Current civilization (sample)

The included export contains a living society of the **Vegega** lineage (generations 6–10), with active Resource-Harmonizer, Resource-Seeker, Techno-Expansionist, and Social-Harmonizer citizens, dozens of structures (many restored or optimized across centuries of simulated time), mentor bonds, and ancestral memory.

## Tech notes

- Single HTML file (~2.1 MB) containing all logic, styles, and assets.
- Simulation loop driven by `requestAnimationFrame` with speed controls (1x / 2x / 4x).
- Isometric rendering with depth sorting, minimap, relationship web, mentor lines, and territory overlays.
- Extensive self-test suite and debug views (organisms, settlements, ancestral memory, hall of fame, formulas, history graph, culture, chronicle, changelog).

## License

This project is provided as-is for personal exploration and further development.

---

*Born from a long-running experiment in emergent digital life.*
