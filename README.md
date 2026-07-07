# Dorn's Fast Travel

PDA map travel with a real path, real risk, and a Sneaking skill that gets better the more you use it - for **S.T.A.L.K.E.R. G.A.M.M.A.**

## Why this mod exists

GAMMA's own Fair Fast Travel is technically free - but only from a friendly base, which is rarely where you are when you actually want to travel. Everywhere else the only option is Hire Guide, for rubles. Free or paid, both do the same thing: click a menu, time skips, you're just there. No path, no patrols, no chance of anything finding you along the way. That's the gap this mod closes.

Travel and Sneak are free and start from wherever you're standing - but the clock still moves while you do it, and you're actually going somewhere: the PDA plots a real path across the navmesh, the ground your character might walk, biased toward roads the way a real stalker might go. It just plays out faster, in real time, than covering it yourself would. Carrying more gear slows the pace; choosing to sneak instead of jog slows it further, the same way either would on foot.

Because it's a real path, you can be ambushed on it, same as if you'd walked it yourself. Sneak mode gives you a real chance to slip past instead of fighting, and a Sneaking skill that gets a little better every time you use it - faster, and a bit safer - though it never makes you untouchable.

You can only fast travel within your current map. Crossing to another means reaching an actual zone transition yourself (Travel or Sneak gets you there) and taking it for real, so crossing the Zone still feels like crossing the Zone. Hiring a guide skips the walk, the path, and the risk entirely, for a price pitched above GAMMA's own guide fare on purpose - a truly safe, zero-effort trip across the map should never be the cheap option.

No MCM sliders for ambush chance, guide price, or travel speed. Options to make it easier would just tempt you to use them, so there aren't any. This is what fast travel in GAMMA should feel like by default.

In-game guide: **PDA > Guide > Addons > Dorn's Fast Travel**

Credit to damage_zedd and **The Long Road Ahead** mod, which inspired this mod.

## How to travel

Right-click a destination on the PDA map - bases, campfires, zone exits, or your own stashes (including anomalous stashes) - and pick:

- **Travel here** - current map only. Free. Fast. No ambush dodge - if something's close enough to notice a sprinting stalker, it will.
- **Sneak here** - current map only. Free. Much slower. Gives you a real chance to dodge ambushes.
- **Hire guide** - jumps you to any base or owned stash on any map. Costs rubles per km, no ambush risk, no survival drain - but game time still passes.

You have to keep the PDA open for the whole trip: putting it away, or taking any damage, cancels the journey on the spot, wherever you're standing.

## What the PDA shows you

The map draws your actual route and animates a dot along it as you travel - grey ahead of you, green behind you as you make progress. If you dodge a threat along the way the dot near that spot turns blue; if one catches you, it turns red and a short PDA alert plays half a second before you're pulled into the fight, so you have a moment to see it coming.

Hunger, thirst, and sleep drain for the game time a Travel/Sneak trip takes (guide trips skip this drain).

## Emissions

You can't start Travel, Sneak, or Hire guide if an emission is already active, or one is due immediately.

If one is due partway through a longer trip, you're carried to wherever you'd have reached by then, the clock jumps forward to just before it hits, and it plays out normally from there - only partial hunger/thirst/sleep drain for the shortened trip. If it catches you before that point instead, the journey cancels outright and you're left exactly where you started, with no time lost.

## Ambushes

Travel and Sneak can't even begin if hostiles are already within detection range. Once you're moving, the route is checked periodically for patrols or mutants close enough to notice you - reading the same real path shown on the map, not a straight line - so lingering near a threat for a while means more than one chance to be spotted, not a single roll of the dice.

Getting ambushed drops you short of your destination, puts the hostiles on alert, and leaves you winded: 50% stamina normally, 100% if you were sneaking. The same detection and ambush rules apply to threats waiting at your destination too, not just along the way.

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
- Arrival stamina: ambushed = 50% (100% if sneaking); arriving over max carry weight = 10% regardless - whichever is lower wins.
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
