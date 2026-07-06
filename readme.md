# Hollow Pines Harvest (Bunny Killer)

A single-file VHS analog-horror hunting game built on Three.js. Survive five days in the
forest around your cabin: hunt bunnies by day, staple them to the wall by night, and try
not to think too hard about why the forest missed you.

## How to play

Open `Hollow_Pines_Harvest_PERFECT_VISUAL_REMASTER_GUNS_OPTIMIZED.html` in a browser.
The game is one self-contained file; it only needs an internet connection to fetch
Three.js r128 from the CDN.

### Controls

| Input | Action |
| --- | --- |
| Mouse | Look / aim |
| Left click | Fire |
| Right click | Aim down sights |
| W A S D | Move (Shift to sprint) |
| Space | Jump |
| C | Crouch (Shift + C while moving to slide) |
| E | Interact / collect |
| R | Reload |
| 1–5 | Weapons (one unlocks per day) |
| J | Journal |
| Esc | Pause |

### Weapons

Hunting Rifle (bolt) · Semi-Auto Rifle · MP40 · Galil · Bloodhound (revolver) —
each unlocks on its matching day. Coins from kills buy per-gun and global upgrades
at the workbenches.

## VHS Analog Horror Remaster

The latest pass replaces the old CSS-overlay CRT fake with a real WebGL
post-processing shader and remasters the guns, reloads, and bunnies:

- **Shader pass** — tape wobble, rolling tracking bands, chroma bleed with a proper
  VHS chroma low-pass, scanlines, animated grain, dropout specks, head-switching
  noise, and a vignette. The grade grows more wrong as the days pass; day 5 pulls
  red with heavy chroma separation, and glitch spikes ride threat and the god
  sequence. Toggle the CRT setting to soften it.
- **Guns** — procedural worn-metal and wood-grain detail textures on every
  viewmodel, plus machined parts (scope glass, muzzle brakes, ejection ports, mag
  ribs, cylinder flutes, ejector rod, triggers and guards) and additive
  muzzle-flash sprites.
- **Reloads** — fully keyframed with easing: magazine guns drop the old mag in an
  arc, swing the new one in, and seat it with a slap before racking the charging
  handle; the bolt rifle feeds visible rounds one by one; the revolver swings out,
  dumps brass muzzle-up, and takes a speedloader.
- **Bunnies** — fur detail maps with per-bunny tint, whiskers, eye glints, hop
  squash-and-stretch, ear flop, and an analog-horror stare twitch from day 3 on.

## Audio & the God Encounter

- **Sound remaster** — every gunshot is layered synthesis (a sharp crack, a body
  report, a pressure thump, and a decaying tail) tuned per weapon, plus metallic
  reload clicks, soft dirt footsteps, and a creaking cabin door.
- **Horror score** — a procedural score that has no music in normal play, then
  wakes on Day 5: a low detuned drone and a dissonant cluster swell through the
  God countdown while a heartbeat speeds up as the timer runs out. His arrival
  lands a low toll; the boss fight drives a steady pulse with dissonant stabs on
  his attacks.
- **God arrival** — when God comes, the camera is dragged onto him and a choice
  rises: **Fight** or **Succumb**. Succumb plays a cutscene where he lunges,
  grabs, and rips your head off, then the run ends.
- **Boss arena** — Fight drops you into a blood-lit arena where the Bunny God has
  four telegraphed attacks — **Ground Slam** (marked circles at your feet),
  **Shockwave** (get away from him), **Eye Beam** (strafe out of the lane), and
  **Leap Slam** (leave the marked landing). Read the wind-up, dodge the glowing
  ground, then empty his health bar to win.
