# Dorn's Fast Travel

A maintained fork of **[The Long Road Ahead](https://www.moddb.com/mods/stalker-anomaly/addons/the-long-road-ahead)** (TLRA v2.2.0) by **Damage_Zedd**, redesigned for same-zone travel with sneak mechanics and GAMMA integration.

**Replace** the original TLRA mod in Mod Organizer 2. **Disable Fair Fast Travel** in MO2 — this mod provides its own PDA travel menus and journey system. If FFT is still installed, its map handlers are unregistered and its trips are blocked.

## Credits

- **The Long Road Ahead** — Damage_Zedd (base journey simulation, ambush system)
- **Skill System** — Haruka (Scouting skill integration)

## Features

- **PDA destinations** — bases (house icon), campfires (with map spots), fast-travel markers, and zone transition points
- **Same-zone travel** — animated journey within the current map; cross-zone destinations require a guide or zone exits
- **Two travel modes** — `Travel here (Xh Xm, X% sneak)` and `Sneak here (Xh Xm, X% sneak)`
- **Travel time** — 10 minutes per km (normal), 30 minutes per km (sneak, 3× longer)
- **No ruble cost** for animated travel; guided instant travel costs rubles (default **2000 RU per km**, MCM slider up to 5000)
- **Scouting skill** (Haruka) — +5% sneak per level, −2% resource cost per level (max 90% reduction); XP from dodging ambushes and completing sneak journeys
- **Survival costs** — 10% per game hour on hunger/thirst/sleep (sneak costs more because it takes 3× longer)
- **Encumbrance** — over 100% carry weight adds travel time linearly (110% = +10%)
- **No arrival fade-in**

## Installation

1. Disable **The Long Road Ahead**, **TLRA Fair Fast Travel Patch**, and **Fair Fast Travel** in MO2
2. Enable **Dorn's Fast Travel** (after Dorns_Common and Haruka Skills)
3. Configure in MCM → **Dorn's Fast Travel**

Campfires on the PDA map require a mod that adds campfire map spots (e.g. **Display Campfires on Map**).

## Requirements

- S.T.A.L.K.E.R. Anomaly / GAMMA
- MCM
- **Dorns_Common**
- Skill System — Haruka (for Scouting skill)

## Repository

https://github.com/JoshuaCarter/GAMMA-Fast-Travel
