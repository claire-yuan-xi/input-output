# Input/Output — progress

## Current position

- Phase: P0 Setup and first scene
- Task: Write index.html with the import map
- Total hours: 0 / 84 (minimum 75)
- Started: 2026-11-09

## Phases (budget in hours)

### P0 · Setup and first scene — 6 h
- [x] Create GitHub repo, install Live Server, turn on GitHub Pages
- [ ] Write index.html with the import map (three, three/addons, cannon-es, gsap, lil-gui; pinned)
- [ ] main.js: Scene, PerspectiveCamera, WebGLRenderer, animation loop, pixel ratio clamped to 2
- [ ] First matcap: draw a shaded sphere on a canvas, use it on a RoundedBoxGeometry cube that spins
- Done when: the matcap cube spins on the live GitHub Pages link.

### P1 · The toy desktop arena — 10 h
- [ ] src/data/palette.js: my own colors; a matcap maker that turns any color into a CanvasTexture
- [ ] Soft gradient background from a 2x2 canvas texture
- [ ] Desktop floor and three app windows built from rounded geometries, grouped as models
- [ ] Window title bars and icons drawn with CanvasTexture
- [ ] Blob shadows under objects (radial-gradient plane)
- [ ] Angled perspective camera, resize handling, lil-gui behind #debug
- Done when: the arena looks like a chunky toy desktop from above and resizes cleanly.

### P2 · Input and combo engine — 10 h
- [ ] input.js: keydown/keyup, preventDefault, Ctrl vs Cmd detection
- [ ] shortcuts.js: the 16 shortcuts as data
- [ ] combos.js: turn key presses into shortcut events
- [ ] On-screen debug panel that names each detected shortcut
- [ ] Test all 16 in Chrome, Firefox, and Safari or Edge
- Done when: all 16 register in 3 browsers and none opens a browser dialog.

### P3 · Physics, player and data-pulses — 10 h
- [ ] physics.js: cannon-es World, gravity, floor body, sleeping on
- [ ] Mesh-to-body sync each frame (position + quaternion)
- [ ] Cursor ship as a physics body, moved with forces; blob shadow fades with height
- [ ] Eased follow camera (lerp toward the player)
- [ ] Pulse projectiles with object pooling; Ctrl+C locks a test target, Ctrl+V fires at it
- Done when: the ship slides with physics, the camera follows smoothly, and lock + fire work.

### P4 · Enemies, waves and the system wipe — 10 h
- [ ] enemy.js: toy-like enemies that drop in with a bounce, with a Sprite label showing their shortcut
- [ ] spawner.js + levels.js waves
- [ ] collisions.js: hits knock enemies over with physics impulses; dispose() on removal
- [ ] wipe.js: the wall that chases you; health and game over
- Done when: you can play three waves, lose, and restart.

### P5 · All 16 abilities — 10 h
- [ ] Wave 1-2 abilities (copy, paste, save, undo, redo, cut)
- [ ] Wave 3-4 abilities (select all, find, tab, word jump, line jump, delete word)
- [ ] Wave 5-6 abilities (bookmark, print, link, comment)
- [ ] Cooldowns shown on the HUD
- Done when: each shortcut does its effect and shows a cooldown.

### P6 · The learning layer — 10 h
- [ ] Boot-sequence tutorial per new shortcut
- [ ] codex.js: the shortcut manual
- [ ] stats.js: reaction time per shortcut (performance.now)
- [ ] Spawner favors your slowest shortcuts
- [ ] Results screen; best scores in localStorage (try/catch)
- Done when: a friend who didn't know Ctrl+K uses it without looking by the end of one run.

### P7 · Motion, glitch and sound — 8 h
- [ ] Intro: objects rise out of the floor one by one (GSAP timeline)
- [ ] Springy details (antennas or flags that wobble back to center)
- [ ] GSAP camera moves between areas; GlitchPass burst and screen shake on damage
- [ ] Hit particles with Points; sfx.js Web Audio blips and hits
- Done when: the intro feels like Bruno's drop-in, hits feel bad and combos feel great.

### P8 · Menus and HUD polish — 4 h
- [ ] Title, pause and settings screens (Ctrl/Cmd override, volume) in my own style
- [ ] HUD polish and a monospace or pixel font
- Done when: a new player can start, pause and quit without help.

### P9 · Playtest, performance and ship — 6 h
- [ ] Three playtests with notes; balance fixes
- [ ] renderer.info, frame rate on a school laptop; matrixAutoUpdate off for static objects
- [ ] README with a GIF, the shortcut list, the live link, and credit to Bruno Simon as visual inspiration
- Done when: 60 fps on a school laptop and the live link is in the README.

## Hours log

| Date | Phase | Hours | What I did | What I learned |
| --- | --- | --- | --- | --- |

## Parking lot (ideas for later phases)

-
