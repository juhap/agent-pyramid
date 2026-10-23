# Raising the Great Pyramid

A browser 3D animation of a first-principles plan for building the Great Pyramid of Giza with
the tools of the time: sledges on wetted tracks, a wide straight ramp for the lower 60 m, a
narrow ramp wrapped around the stepped faces for the upper part, levers for the last metres,
and casing dressed from the top down while the ramps are removed.

## Running it

Open `index.html` in a browser with WebGL. It works straight from the filesystem (`file://`);
three.js and the fonts are loaded from CDNs, so it needs an internet connection.

## What is in it

- **The plan** — the button "Read the plan" opens the written building plan with the numbers
  behind it: volume distribution, sledge friction and team size, ramp dimensions, delivery
  rate, schedule and workforce.
- **The animation** — survey and orientation, levelling with water trenches, the quarry,
  hauling teams of stick figures (haulers on two ropes, a water pourer, a foreman), the straight
  ramp with two up lanes and a return lane, a granite-beam convoy for the King's Chamber, the
  spiral ramp on the stepped core, lever crews and the pyramidion at the top, and masons
  dressing the casing while the ramps come down.
- **Controls** — timeline with clickable phases, play/pause (Space), speeds 0.5×–8×, camera
  presets (Overview, Ramp, Quarry, Working level), "Follow team" and a "Cinematic" camera that
  plays a scripted shot list.

The model uses 100 courses instead of the real ~210, and people are drawn to true scale
(1.7 m), so use "Follow team" or "Working level" to see them.

## Recording

`index.html?record` hides the interface and exposes `recorder.start()`, which renders every
frame at a fixed 30 fps time step, encodes it with WebCodecs and uploads the MP4 to a small
local server (not included here). The video in `../videos/opus-5-5.mp4` was made this way and
re-encoded to fit the repository.
