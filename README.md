# GAMMA Prone Fix

## Just watch the video :)

Makes low-crouch ("prone") in **S.T.A.L.K.E.R. G.A.M.M.A.** actually useful — within the limits of what modding allows. It's a hacky workaround, not a proper prone system., but it's no worse than what we have now IMO.

## Demo

https://github.com/user-attachments/assets/d76e38ac-12f6-43be-a209-573fa6dc55bb

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
- You take 20% more damage by default when prone, but you can adjust that (100% - 200%) in an effort to compensate for the missing limbs...

## Installation

1. Download the latest release from here: https://github.com/JoshuaCarter/GAMMA-Prone-Fix/releases <img width="695" height="275" alt="Screenshot 2026-06-27 232624" src="https://github.com/user-attachments/assets/e91f0db7-fcc0-4195-a7f4-de0e3ee6b419" />
2. Install via MO2 like normal

## Warnings!

- This mod overrides the `stalker_smart_cover_animation.omf` animations file so it wont play nice with other mods that do the same (If you know a better way, im listening)
- This mod relies on calculations that use camera height, so you pose/posture will be broken in 3rd person etc.
