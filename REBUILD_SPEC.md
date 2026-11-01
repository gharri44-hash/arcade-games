# Joker Arcade — Reference-accurate rebuild brief

Status: Existing 2D pages are temporary prototypes. Do NOT present them as the finished games.

## Design goal
Recreate the **mechanics and 3D visual language** visible in the user-supplied reference recordings, using original or appropriately licensed assets. Netlify remains the static host and GitHub remains the source of truth. Existing placeholder gameplay should be replaced rather than cosmetically restyled.

## Vanguard Protocol
Reference: elevated grey bridge, close blue 3D soldier formation, left-hand +1 reinforcement lane, dense zombie river straight ahead, giant red/orange zombie boss with numeric health bar, metallic weapon-upgrade props on right, bright yellow multi-stream firing effects.

Minimum acceptance criteria:
1. Actual spatial 3D scene with perspective camera, depth, light, shadows, detailed materials, character mesh instances and animated running.
2. Visible squad count matches actual soldiers (LOD/instanced meshes when many).
3. Multiple lanes and side upgrade/reinforcement interactions, not generic random pickups dropped from sky.
4. Shootable/collectible weapon crates; immediate visible weapon model and HUD change, with genuinely distinct mechanics: minigun high fire rate/tracer stream; shotgun multi-pellet cone; progressive stats and upgrades.
5. Dense forward-travel zombie hordes, collisions, knockback, breach/base damage, final horde, oversized boss with health bar.
6. Responsive drag/touch and mouse control, usable portrait mobile presentation and desktop.
7. Gameplay verification for every pickup, collision and win/loss condition.

## Hold the Line
Reference: a massive orange angular downward-moving shape occupying most of the portrait view, fiery skyline, small densely arranged luminous cyan/blue defender squad at the bottom, intense vertical cyan projectile streams, side-mounted weapon icons/costs and +1 upgrade opportunities.

Minimum acceptance criteria:
1. Giant layered orange advancing formation with convincing depth, illuminated edges, particles, impact damage and pieces breaking away.
2. Blue clustered soldiers/defender guns with modern 3D models and clear scale contrast.
3. Actual weapon progression, purchasable/equippable upgrades, cost indicators, changed effects/stats.
4. Strong fire glow, hit sparks, bloom-like post effects, convincing warm environment and loss effects.
5. Balancing and UI that leave gameplay visible on phone.

## Engineering quality bar
- No placeholder triangles or rectangles as final enemy/weapon/character models.
- Use a 3D rendering engine with licensed original/third-party assets.
- Asset sizes and draw calls optimized for browser/mobile; graceful fallbacks.
- Controls, gameplay, effects and audio verified in-browser before calling finished.
- Prioritize mechanical fidelity before polish, then visual fidelity and performance.
