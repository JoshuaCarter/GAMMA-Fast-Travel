# Dorn's Fast Travel

A maintained fork of **[The Long Road Ahead](https://www.moddb.com/mods/stalker-anomaly/addons/the-long-road-ahead)** (TLRA v2.2.0) by **Damage_Zedd**, redesigned for same-zone travel with sneak mechanics and GAMMA integration.

**Replace** the original TLRA mod in Mod Organizer 2. Fair Fast Travel is **not required** — this mod provides its own PDA travel menus and journey system. If FFT is still enabled, its map handlers are unregistered and its trips are blocked automatically.

## Credits

- **The Long Road Ahead** — Damage_Zedd (base journey simulation, ambush system)
- **Skill System** — Haruka (Scouting skill integration)

## Features

- **PDA destinations** — bases (house icon), campfires (with map spots), fast-travel markers, and zone transition points
- **Same-zone travel** — animated journey within the current map; cross-zone destinations require a guide or zone exits
- **Two travel modes** — `Travel here (Xh Xm, X% sneak)` and `Sneak here (Xh Xm, X% sneak)`
- **Travel time** — driven by PDA map speed: default fastest pace is 50 (1 hr/km game time at normal weight). Sneak is ⅓ speed (3 hr/km). MCM **Fastest PDA Map Speed** sets that ceiling (up to 100); sneak and encumbrance slow from there.
- **Cancel travel** — free because game time never moves during the PDA bar. Hunger/thirst/sleep only apply when the clock jumps at arrival (or partial jump on ambush); cancel skips that and returns you to where you started
- **No ruble cost** for animated travel; guided instant travel costs rubles (default **2000 RU per km**, MCM slider up to 5000)
- **Scouting skill** (Haruka) — max level 20; +3% sneak per level; 5 XP per km of sneak travel, 10 XP per ambush dodged
- **Ambush detection** — scan radius from 50 m day base, minus time and weather (stacked). On ambush, pull back by **scan radius** (**×2** sneaking, **max 60 m**). Normal-travel ambush sets stamina to **50%**. Hostiles alerted **1 s** after spawn; invulnerable until then. Clear arrival: **5 m** before destination.
- **Ambush dodge** — base chance plus Scouting skill; Sneak mode doubles it. No night/rain bonus to dodge.
- **Survival costs** — hunger/thirst/sleep from the game-time jump only (journey length × map speed; sneak = 3× longer)
- **Encumbrance** — matches GAMMA inventory weight colours: normal (full map speed), near-max yellow (−25%), overweight red (speed ÷ carry ratio). Sneak is ⅓ map speed on top of that, so heavy + sneak is very slow and costly.
- **No arrival fade-in**

## Installation

1. Disable **The Long Road Ahead** and **TLRA Fair Fast Travel Patch** in MO2 (optional: disable **Fair Fast Travel** — Dorn's replaces it if left enabled)
2. Enable **Dorn's Fast Travel** and **Dorns_Common** in MO2
3. Configure in MCM → **Dorn's Fast Travel**
4. Read **PDA → Guide → Addons → Dorn's Fast Travel** for how the system works

Campfires on the PDA map require a mod that adds campfire map spots (e.g. **Display Campfires on Map**).

## Requirements

- S.T.A.L.K.E.R. Anomaly / GAMMA
- MCM
- **Dorns_Common**
- Skill System — Haruka (for Scouting skill)

## Repository

https://github.com/JoshuaCarter/GAMMA-Fast-Travel
