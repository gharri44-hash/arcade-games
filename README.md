# Arcade Lab

Two original browser games using a locally bundled Three.js renderer:
- [Hold the Line](./hold-the-line/): orange advancing armor, a fire-lit battlefield, and weapon progression.
- [Vanguard Protocol](./vanguard-protocol/): daylight bridge, zombie crowds, oversized bosses, recruit lane and weapon lane.

## Visual rebuild

Shared `assets/combat.js` includes original modeled soldiers, animated instanced character meshes, equipment pouches, helmets, anatomical faces and limbs, shadows, and procedural asphalt detail. Vanguard uses neutral daylight, bridge supports, river, buildings and trees. Hold the Line uses orange lighting, layered extruded armor and a damaged skyline.

Rifle, shotgun and six-barrel minigun pickups display the actual weapon meshes. Shooting or collecting them equips the corresponding model across the squad and changes spread, fire rate and damage. Left-side gates recruit actual visible soldiers. Mouse, drag and arrow keys steer; P pauses. Coin totals persist in browser storage.

Characters are original procedural models and remain stylized. They are not scanned or motion-captured assets. Browser WebGL with hardware acceleration is required; a visible startup message explains context failure.

## Hosting

Serve the repository root as static files with no build step. Both game folders import the shared assets locally. Existing Git-based hosts can deploy on pushes to main; no hosting-provider change is required. Three.js 0.169.0 is bundled under its MIT license in `assets/vendor/`.

## Verification

JavaScript syntax checks and a Node simulation using actual Three.js geometry passed for both modes: valid geometry, weapon shoot/equip, recruitment, pause and restart. The cloud browser's WebGL context was unavailable, so visual GPU rendering and mobile performance need verification on a WebGL-enabled device. This is a visual rebuild milestone, not a claim of reference-identical realism.
