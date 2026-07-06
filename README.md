# Dorn's Fast Travel

PDA map travel with a real path, real risk, and a Sneaking skill that gets better the more you use it - for **S.T.A.L.K.E.R. G.A.M.M.A.**

## Why this mod exists

Want to fast travel for free? Now you can - it just isn't free of risk.

GAMMA's own Fair Fast Travel is technically free - but only from a friendly base, which is rarely where you are when you actually want to travel. Everywhere else, the only option on the menu is Hire Guide, which costs rubles. Free or paid, both versions do the same thing: you click a menu, time skips forward on the clock, and you're just there. No path, no patrols, no chance of anything finding you along the way. That's the gap this mod exists to close.

Walking and sneaking here are free in rubles too, and you can start from wherever you're standing, not just a friendly base - but the clock still moves while you do it. The PDA bar is doing the walking for you, not stopping time while it does. And you're actually going somewhere: the PDA shows the journey you're taking along a real path across the navmesh - ground your character might walk, biased toward roads the way a real stalker might go - it just plays out faster, in real time, than if you'd covered it yourself. Carrying more gear slows that pace down, and choosing to sneak instead of jog slows it down further still, the same way either would on foot.

Because it's a real path and not an abstracted straight line, you can be ambushed on it, same as if you'd walked it yourself. Sneak mode gives you a real chance to slip past instead of fighting, and a Sneaking skill that gets a little better every time you use it - faster, and a bit safer - though it never makes you untouchable.

You can only fast travel within your current map. Crossing to another one means reaching an actual zone transition yourself (Travel or Sneak will get you there) and taking it for real - so crossing the Zone still feels like crossing the Zone, not a click from Cordon to Pripyat. Whatever's waiting on the other side is still waiting.

Hiring a guide skips all of that - the walk, the path, and the risk entirely - for a price, the same role GAMMA's own guide travel already fills. That price is set to beat the default guide fare, not undercut it, because a truly safe, zero-effort trip across the map should never be the cheap option. It's there for when you're willing to pay big for certainty; most of the time it's too expensive to be the answer.

There's no MCM slider for ambush chance, guide price, or travel speed. Options to make it easier would just tempt you to use them - so there aren't any. This is what fast travel in GAMMA should feel like by default.

The whole point: skip the tedium of travel, not the consequences of it.

In-game guide: **PDA > Guide > Addons > Dorn's Fast Travel**

Credit to damage_zedd and **The Long Road Ahead** mod, which inspired this mod.

## What this mod does

- Right-click destinations on the PDA map: bases, campfires, zone exits, and your own stashes.
- Replaces GAMMA's default fast travel options.
- **Travel here** - fast pace, current map only, no ambush dodge.
- **Sneak here** - slower, but gives you a real chance to dodge ambushes.
- **Hire guide** - pay rubles to jump straight to any base or owned stash on any map, no ambushes, no survival drain.
- An animated dot path plots your route along the real navmesh (road-biased) while the journey bar runs.
- Hunger, thirst, and sleep drain for the game time you skip on Travel/Sneak trips (guide trips skip this drain).

## Emissions

You can't start Travel, Sneak, or Hire guide if an emission is already active, or one is due immediately.

If one is due partway through a longer trip, you're carried to wherever you'd have reached by then, the clock jumps forward to just before it hits, and it plays out normally from there - only partial hunger/thirst/sleep drain for the shortened trip. If it catches you before that point instead, the journey cancels outright and you're left exactly where you started, with no time lost.

## Ambushes

Travel and Sneak can't even begin if hostiles are already within detection range. Once you're moving, the route is checked periodically for patrols or mutants close enough to notice you - reading the same real path shown on the map, not a straight line - so lingering near a threat for a while means more than one chance to be spotted, not a single roll of the dice.

Sneak mode gives you a chance to slip past instead of fighting; Travel doesn't - if something's close enough to notice you while sprinting, it will. Getting ambushed drops you short of your destination and puts the hostiles on alert. The same rules apply to threats waiting at your destination too, not just along the way.

## Sneaking skill

You gain Sneaking XP from ambush outcomes during a sneak journey: dodging a threat, or getting caught by one. It's a slow grind that makes sneaking faster and a little safer over time, but even at high levels it never removes ambush risk entirely.

## Settings

**MCM > Dorn's Fast Travel:** message duration only. The travel rules themselves aren't exposed as sliders - see "Why this mod exists" above.

## By the numbers

**Travel speed** (PDA bar speed = game time; heavier loads slow the bar and lengthen the trip):

- Travel: ~30 minutes per km at normal weight. +10 m ambush detection range vs Sneak (sprinting is louder).
- Sneak: ~3 hours per km at Sneaking Lv0. -5 min/km per Sneaking level, floor ~80 min/km.
- Encumbrance: yellow (within 10 kg of max carry) = -20% bar speed; red (over max carry) = -50% bar speed.
- Too encumbered to walk blocks Travel and Sneak; Hire guide still works.

**Ambush detection range** (day base 60 m for Sneak, stacking modifiers below):

- Twilight (6-7 AM, 7-8 PM): -10 m
- Night (8 PM-6 AM): -20 m
- Rain: -10 m. Storm: -15 m. Fog: -20 m (weather stacks with time of day)
- Sneak range after modifiers: 20-60 m. Travel: same modifiers, then +10 m (sprinting) = 30-70 m.
- Within range, a patrol notices you if they're within 10 m of your height, or have a clear line of sight to you.
- Checks repeat roughly every 12 seconds of real time while you're traveling.

**Ambush outcomes:**

- Dodge chance: Travel 0%. Sneak 25% base + 3% per Sneaking level, capped at 85%.
- Drop distance when ambushed: starts at your detection range, then Travel -10 m (reckless) or Sneak +10 m (cautious), plus +1 m per Sneaking level. Clamped to 20-80 m.
- Hire guide trips cannot be ambushed.
- Sneak mode XP: +20 for dodging, +10 for getting ambushed.

**Sneaking skill**, per level:

- +3% ambush dodge chance (Sneak mode only)
- +2% PDA travel speed (Sneak mode only)
- +1 m ambush drop distance

**Guide fees:**

- 3000 RU per km, flat, regardless of distance or danger.
- 1 hour of game time per km still passes on the clock.
- Blocked during active emissions, same as Travel and Sneak.
- For comparison, GAMMA's own guide travel charges about 1500 RU per km by default - this mod's guide is priced above that on purpose.

## Installation

1. Install via MO2.
2. Disable **The Long Road Ahead** if you use it - this mod replaces that travel style.
