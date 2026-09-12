# Hardcore Zombie Variants

This source tree adds a stronger alternate form for the vanilla zombie types.

## How it works

`Board::AddZombieInRow` rolls an elite/hardcore flag when a normal wave spawn is
created. The chance starts at 12% and rises by 3 percentage points every five
waves, capped at 30%.

The original `ZombieType` is preserved, so existing animations and special AI
continue to work. `Zombie::ApplyHardcoreVariant()` then gives the selected
zombie a type-specific health and movement boost. Equipment health (cone,
bucket, doors, etc.) is boosted too.

No EA/PopCap resources are included or modified by this change.
