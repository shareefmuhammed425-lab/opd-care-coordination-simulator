# OPD Queue Simulator: Current vs Proposed

An interactive, browser-based simulation comparing two ways of running a morning
outpatient department (OPD): **everyone walks in** (current) vs **appointments + PIN/tokens + triage** (proposed).
Both systems run on the same patients and the same staff.

**Live demo:** https://YOUR-USERNAME.github.io/opd-queue-simulator/

## What it shows
- Two animated floorplans side by side (registration → vitals → consultation → pharmacy)
- KPIs: time standing in queues, registration wait, total time in the OPD
- Click any patient dot to follow their journey
- Sliders for appointment share, patient volume, service times, staffing, PIN uptake
- Preset scenarios (heavy Monday, high digital adoption, complex cases)

## Run locally
No build step and no dependencies. Download the repo and open `index.html` in any modern browser.

## Project structure
```
index.html   # the whole simulator (HTML + CSS + JavaScript)
README.md
LICENSE
.nojekyll
```

## Customising
Open `index.html` and edit the `params` object near the top of the `<script>` block
(service times, staffing, appointment ratio, number of patients). The `LAYOUT` object controls the floorplan.

## License
MIT. See `LICENSE`.
