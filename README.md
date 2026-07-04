# Dorn's Fast Travel

A maintained fork of **[The Long Road Ahead](https://www.moddb.com/mods/stalker-anomaly/addons/the-long-road-ahead)** (TLRA v2.2.0) by **Damage_Zedd**, with QoL fixes and extra travel options for GAMMA.

**Replace** the original TLRA mod and its FFT compatibility patch with this mod in Mod Organizer 2. Keep **Fair Fast Travel** enabled.

## Credits

- **The Long Road Ahead** — Damage_Zedd (base design, journey simulation, ambush system)
- **Fair Fast Travel** — Catspaw (cost/duration integration)

## Changes from TLRA

- **No arrival fade-in** — removed `fade_in.ppe` on arrive, abort, and ambush
- **Time acceleration works** — MCM time factor now scales real-time journey speed on the PDA map
- **Weapon restore mode** — MCM: keep current weapon, force primary, or force secondary after travel
- **Message duration** — configurable on-screen message time (default 10s)
- **Rank sneak toggle** — disable rank bonus on ambush dodge rolls
- **Ambush spawn offset** — separate slider from normal arrival offset
- **Sneaky travel** — extra PDA option: higher cost/time, bonus sneak chance
- **Cross-zone PDA options** — *Final leg only* and *Travel to zone exit* without toggling MCM
- **Combat fix** — no stealth dodge while hostiles are already near you; no sneaking past active fights after transitions

## Installation

1. Disable **The Long Road Ahead** and **TLRA Fair Fast Travel Patch** in MO2
2. Enable **Dorn's Fast Travel** (load after Fair Fast Travel)
3. Configure in MCM → **Dorn's Fast Travel**

## Requirements

- S.T.A.L.K.E.R. Anomaly / GAMMA
- MCM
- Fair Fast Travel (Catspaw)

## Repository

https://github.com/JoshuaCarter/GAMMA-Fast-Travel

## Files

- `gamedata/scripts/zzzz_dorn_fast_travel.script` — main travel logic
- `gamedata/scripts/zzz_dorn_fast_travel_mcm.script` — MCM
- `gamedata/scripts/zzz_dorn_fast_travel_fft_patch.script` — FFT hook
- `gamedata/configs/text/eng/ui_mcm_dorn_fast_travel.xml` — strings
