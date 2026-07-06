# Dorn's Fast Travel

PDA map travel with a visible journey, ambushes along the way, optional sneaking, and a Sneaking skill - for **S.T.A.L.K.E.R. G.A.M.M.A.**

## What this mod does

- Right-click destinations on the PDA map: bases, campfires, zone exits, and your own stashes.
- Replaces GAMMA's default fast travel options.
- **Travel here** - fast pace on the current map only.
- **Sneak here** - much slower, but you can dodge ambushes.
- **Hire guide** - pay rubles for an instant jump to any base or owned stash on any map.
- Animated dot path while the journey bar runs.
- Hunger, thirst, and sleep drain for the game time you skip.

In-game guide: **PDA > Guide > Addons > Dorn's Fast Travel**

Credit to damage_zedd and **The Long Road Ahead**, which inspired this mod.

## Travel speed (PDA bar = game time)

The map journey bar speed sets how long the trip takes and how much hunger/thirst/sleep you lose. Heavier loads slow the bar and lengthen the trip.

| Mode | Trip time (normal weight) | Notes |
|------|---------------------------|-------|
| **Travel** | ~30 minutes per km | No ambush dodge. Louder: enemies spot you from farther away (+10 m vs sneak). |
| **Sneak** | ~3 hours per km at Sneaking Lv0 | Dodge ambushes (see below). -5 min/km per Sneaking level (floor ~80 min/km). |

Encumbrance (inventory weight colours): yellow within 10 kg of max carry = -20% bar speed; red over max carry = -50%. Too encumbered to walk blocks Travel and Sneak; Hire guide still works.

## Emissions

At journey start the mod reads GAMMA's emission schedule and compares it to your trip time:

- **Cannot start** Travel, Sneak, or Hire guide if an emission is already running, or one is due right now.
- **Emission during trip (planned):** if the next emission falls before you would arrive, the mod precomputes how far along your route you will be (seconds until emission divided by trip game-time). When the journey bar reaches that point, you are teleported there, game time fast-forwards to just before the emission (~8 seconds of lead), and the emission begins normally. Partial hunger/thirst/sleep only.
- **Emission starts early (unplanned):** if an emission begins while you are still on the bar before that point, the journey is **cancelled** - you stay at your starting spot and face it there. No time passes.

Hire guide is still blocked during active emissions.

## Ambushes

**Cannot start** if hostiles are within detection range - Travel or Sneak, no exceptions.

**Detection range** (day base 60 m; stacks with time and weather):

- **Sneak:** 20-60 m. Twilight (6-7 AM, 7-8 PM): -10 m. Night (8 PM-6 AM): -20 m. Weather stacks: rain -10 m, storm -15 m, fog -20 m.
- **Travel:** same reductions, then **+10 m** (sprinting). Range 30-70 m.

Patrols within range (or within 10 m height, or with a clear line of sight) can ambush you.

| Mode | Dodge chance | If spotted |
|------|--------------|------------|
| **Travel** | 0% | Dropped short, hostiles alerted, fight. |
| **Sneak** | 25% base + 3% per Sneaking level (cap 85%) | Dodge = slip past. Fail = dropped short, hostiles alerted. |

**Drop distance** when ambushed: starts at your detection range, then Travel -10 m (reckless) or Sneak +10 m (cautious), plus +1 m per Sneaking level. Clamped 20-80 m. Tighter visibility (night, fog) means a smaller drop distance.

Hostiles at your destination use the same rules. Sneak dodge can let you arrive cleanly; Travel always stops short if they spot you.

Hire guide trips cannot be ambushed.

## Sneaking skill

Gained by dodging threats and finishing sneak journeys. Per level (open Skills menu for live stats):

- +3% ambush dodge (Sneak mode only)
- +2% PDA travel speed
- +1 m ambush drop distance

## Guide fees

**3000 RU per km**, flat (any difficulty). Ignores weight and ambushes.

## Settings

**MCM > Dorn's Fast Travel:** message duration only.

## Installation

1. Install via MO2.
2. Disable **The Long Road Ahead** if you use it - this mod replaces that travel style.
