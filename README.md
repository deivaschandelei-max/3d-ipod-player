# 3d-ipod-player

A browser-based 3D iPod music player. The device is a real 3D object you can rotate and zoom, with a working click wheel, and its colours follow the album artwork of whatever song is playing.

> **Status: planning.** This repository currently holds the project specification only. There is no application code yet, and nothing here has been built, tested or deployed.

## What it will be

- A real-time 3D iPod (Three.js via React Three Fiber), not a flat image
- A working click wheel, usable by touch, mouse and keyboard
- Local music import: your own audio files, stored in your browser (IndexedDB)
- Playback with queue, shuffle, repeat and playlists
- Themes extracted from album artwork, so every song gives the device a different look
- Mobile-first, with a lower-quality 3D mode for older phones

The full specification is in [docs/SPEC.md](docs/SPEC.md).

## Planned stack

React, TypeScript, Vite, Three.js, React Three Fiber, Drei, Web Audio API and IndexedDB. Source code on GitHub, hosting on Vercel.

## Roadmap

1. Foundation and 3D device
2. Music engine (import, playback, playlists)
3. Dynamic album themes
4. Navigation and click wheel
5. External integrations (only where a supported API exists)
6. Optimisation and deployment

## Notes on music

The plan is for music files to be imported from the listener's own device and kept in their browser. This repository will not contain or host any music.
