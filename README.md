# Travel Hub — Multimodal Journey Planner (Demo)

**Status:** Working **single-file browser demo** (a compact preview of the broader Travel Hub V1.0 project). All schedules, operators, fares, and times are **simulated**, not real travel data.

## Run immediately

Open [index.html](./index.html) locally in Chrome/Edge, or host the repository as a static website. No installation, backend, keys, or database required.

## What this repository currently demonstrates

- Mobile-responsive journey search between sample locations in Vietnam.
- Three transport modes: **public bus**, **ride-hailing estimates**, and **private intercity coach**.
- A small directed transport network with scheduled departures and waiting times.
- Constructing journeys of up to five segments, excluding missed scheduled connections.
- Comparing and ranking journeys by cost, duration and preferred mode.
- Simulating extra bus delay (+25 minutes), triggering recalculation.
- Viewing step-by-step route details with transfer timing.

## Important scope note

This repository currently contains a **lightweight standalone demo**, rather than the complete multi-file Travel Hub V1.0 source package. Its data and route search are suitable for exploring the concept, **not for real-world navigation or booking**. It does not contain a live geographic map, payment, real authentication, operator integrations, or trained ML personalization.

## How to try it

1. Open the page.
2. Select **Biên Hòa** → **District 1** to compare urban bus/ride combinations.
3. Select **Biên Hòa** → **Đà Lạt Hotel** to see scheduled private coach + final-mile options.
4. Change the departure time; test **Simulate +25 minute bus delay**.
5. Change the preferred mode to see how preference affects ranking.

## Product vision

Travel Hub is intended to be a **mobile-first multimodal journey planner** that generates feasible routes from A to B, including combinations of ride-hailing, public buses, and private intercity coaches. Later development may include a route visualization on real map tiles, a more rigorous time-aware routing engine, an optional user profile/history, accessible navigation support, and operator information.

## For Codex

Start by auditing `index.html`, preserving working behavior. Before making major changes, create a normal source structure (`src/data.js`, `src/engine.js`, `src/ui.js`, `styles.css`) and add route-planning tests. Do not claim live or verified transport information. Use commits for each milestone.

## Publishing

The GitHub repository holds code; it is not automatically a hosted app. For a static preview, use GitHub Pages (Settings → Pages → Deploy from a branch → main / root) if your repository settings allow it, or import the repo into Vercel as a static project. No build step is needed for this standalone version.

## License

Student prototype, proof of concept only.
