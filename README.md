# Michael Flynn, PE

Civil / water resources / dam engineer in the Blue Ridge (you may know me as **Hydro Engineer**). I build the **HydroComplete ecosystem** — formula-transparent water-resources software that meets engineers on whatever platform they already work in: the browser, QGIS, Civil 3D, OpenRoads, or a Python console. Single-file HTML games at night.

## The HydroComplete ecosystem

One family of real hydrology & hydraulics engines, many front doors:

| Platform | Project | What |
|---|---|---|
| Desktop | [**stormsewer**](https://github.com/mf4633/stormsewer) | **StormSewer** — a free, GPL storm sewer design app for Windows, macOS and Linux. Rational method, Manning across four conduit shapes, standard-step HGL/EGL, HEC-22 inlets with bypass carryover, auto-sizing, submittal PDF reports. `brew install --cask mf4633/tap/stormsewer` · `winget install MichaelFlynn.StormSewer` · [direct download](https://github.com/mf4633/stormsewer/releases/latest) |
| Browser | [hydrocomplete.com](https://hydrocomplete.com/) | Full stormwater design suite — four calculation engines, live USDA/NOAA data, KaTeX-transparent formulas |
| QGIS | [hydrocn-qgis](https://github.com/mf4633/hydrocn-qgis) | Free GPL plugin: SCS Curve Number from SSURGO + NLCD + DEM slope + NOAA Atlas 14, fetched automatically, with an ESA WorldCover backup source |
| Civil 3D | [hydrocomplete-civil3d](https://github.com/mf4633/hydrocomplete-civil3d) | Stormwater hydraulics add-in — Rust/WASM calculation DAG inside AutoCAD Civil 3D |
| Open CAD Studio | [Storm Sewer plugin](https://github.com/mf4633/opencad-storm-sewer-plugin) · [HydroComplete plugin](https://github.com/mf4633/opencad-hydrocomplete-plugin) · [plugin host (PR #80)](https://github.com/HakanSeven12/OpenCADStudio/pull/80) | GPL plugins in the [Open CAD Studio](https://github.com/HakanSeven12/OpenCADStudio) marketplace, built for v2026.36. Draw a storm-drain network on the DWG and run Rational + Manning + HGL on it; free to draw and analyze, Pro keys ($29 / $149 a year) unlock reports and sizing — [details](https://hydrocomplete.com/open-source) |
| Engines & libraries | [stormsewer](https://crates.io/crates/stormsewer) · [hydro-tools](https://github.com/mf4633/hydro-tools) · [hydrocomplete-dag](https://github.com/mf4633/hydrocomplete-dag) | The storm sewer engine as an embeddable Rust crate — `cargo add stormsewer`, also compiled to WebAssembly for [in-browser calculators](https://mf4633.github.io/stormsewer/) · open hydrology primitives · WASM model builder |
| Research | [swmm-breach](https://github.com/mf4633/swmm-breach) · [ALR](https://github.com/mf4633/ALR) | Dam-breach hydrographs for SWMM · vortex-particle scour screening |

## Live products

| Project | What | Stack |
|---|---|---|
| **[hydrocomplete.com](https://hydrocomplete.com/)** | Browser-based stormwater engineering — four real calculation engines (Sedimentology, Water Quality, H&H, Conveyance), live USDA soil data, NOAA rainfall, formula transparency via KaTeX. Subscription SaaS. | Node/Express on Fly.io · Supabase · Stripe · Netlify static frontend |
| **[pe-calc.com](https://pe-calc.com/)** | 60+ free engineering calculators — hydraulics, dam safety, environmental, geotech, structural, transportation, mechanical, electrical, chemical. AdSense-supported. | Static HTML/JS · Netlify |
| **[siteprior.com](https://siteprior.com/)** | $29 property due-diligence reports — federal flood zones, soils, slope, wetlands. Single-page checkout. | Static frontend · same Fly backend as HydroComplete |
| **[boardgaminghub.com](https://boardgaminghub.com/)** | 30+ free in-browser games & sims — chess, go, mancala, plus originals (Bisque, Aresia, Doctrine) and physics sims (Apoapsis, Floodline, Tower). Each one a single HTML file. | Vanilla JS, Canvas, Three.js where it earns its keep |

## CAD desk tools

Drop-in scripts for the three major civil platforms. Every routine is one file, named for the command it adds.

- **[C3D-AutoCAD](https://github.com/mf4633/C3D-AutoCAD)** — 23 LISP commands for AutoCAD / Civil 3D (LABELACRES, BD, SLP, FLAT, CHZ, T2M, BC, PA, ...).
- **[Carlson-CAD](https://github.com/mf4633/Carlson-CAD)** — 22 LISP commands for Carlson Civil/Survey, survey-first (LABELAC, LOTBD, PNORENUM, PNOINV, TRAV, FBREP, STALBL, ...).
- **[OpenRoads_vba](https://github.com/mf4633/OpenRoads_vba)** — 24 VBA subs for Bentley OpenRoads Designer (LabelAcres, PointsIO PNEZD I/O, StationOffset, LevelTranslate, ZTools, ...), shipped as importable `.bas` source.

## Engineering research & tooling

- **[swmm-breach](https://github.com/mf4633/swmm-breach)** — pip-installable dam-breach hydrograph generator for EPA SWMM / PCSWMM. Froehlich (2008) implemented, Teton validation case included.
- **[ALR](https://github.com/mf4633/ALR)** — physics-based vortex particle simulation as a Manning's-equation alternative for open-channel scour screening. 109 tests, MIT-licensed.
- **[eclipse-predictor](https://github.com/mf4633/eclipse-predictor)** — 3D solar eclipse paths computed live from Meeus / ELP-2000, NASA catalog dates, single HTML file.

## Sims & games

- **[board-gaming](https://github.com/mf4633/board-gaming)** — every game on boardgaminghub.com, one HTML file each.
- **[Hellcats-Flight-Sim](https://github.com/mf4633/Hellcats-Flight-Sim)** — WWII Pygame flight sim, F6F Hellcat with carrier ops and AI opponents.
- **[flappy-modern](https://github.com/mf4633/flappy-modern)** — Flappy Bird clone with coins, shield, day/night, slow-mo close calls.

## What I care about

- Real formulas over abstractions. If a tool reports a number, it should show the equation it came from.
- Single-file HTML deliverables. No build step, no framework lock-in, no broken links in five years.
- Engineering software that respects engineers' time and their licenses.

## Reach me

- Web: [hydrocomplete.com](https://hydrocomplete.com/) · [pe-calc.com](https://pe-calc.com/) · [siteprior.com](https://siteprior.com/) · [boardgaminghub.com](https://boardgaminghub.com/)
- Location: Asheville, NC
