# GAMMA Prone Fix

Makes low-crouch ("prone") in **S.T.A.L.K.E.R. G.A.M.M.A.** actually useful — within the limits of what modding allows. It's a hacky workaround, not a proper prone system., but it's no worse than what we have now IMO.

## Demo

<video src="https://github.com/JoshuaCarter/GAMMA-Prone-Fix/raw/main/GAMMA%20Prone%20Fix.mp4" controls width="100%"></video>

## The problem

Vanilla prone is fake. It's really just a low crouch: your view drops, but your body stays much higher. You can:

- Think you're behind cover when you're not — enemies shoot you in the face.
- Stick up or out of tight gaps (like a skinny pipe) while feeling fully hidden in first person

## What this mod does

- Lowers your posture to something closer to real prone
- Fixes the headlamp while prone so the light follows your view, not your floating head
- Hides legs and arms on the prone body to reduce clipping through walls and ugly shadows

## What to expect

- **First person** — feels more like actual prone
- **Third person** — looks ridiculous
- Getting in and out of prone is janky but this only affects shadows (and it's less janky than current shadows anyway)
- Best effort given modding constraints — also my first mod - don't expect too much

## Installation

1. Install via MCM like normal

**WARNING!** This mod overrides the `stalker_smart_cover_animation.omf` animations file so it wont play nice with other mods that do the same (If you know a better way, im listening)
