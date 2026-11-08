# WEB APPLICATION CLASSIFICATION & SYSTEM SPECIFICATION
# PROJECT: 3D iPOD MUSIC PLAYER — DYNAMIC ALBUM EXPERIENCE

## 1. APPLICATION IDENTITY

| Classification | Description |
|---|---|
| Application type | Web application |
| Product category | Digital music player |
| Subcategory | 3D interactive music interface |
| Primary experience | Music playback and album visualization |
| Visual identity | Classic iPod-inspired design |
| Rendering style | Realistic 3D, glass, metal, physical controls |
| Theme system | Dynamic album-art-based theming |
| Interaction model | Touch, mouse, keyboard |
| Platform | Responsive web, mobile-first |
| Development environment | GitHub + web development tools |
| Primary developer | Claude AI |

### Application definition

A browser-based, three-dimensional music player that recreates the recognizable physical experience of using an iPod.

It allows users to select music, browse their library, play songs, and interact with a realistically rendered virtual music device.

Unlike conventional music players, the application treats album artwork as the foundation of its visual identity.

Each selected song can transform the device's screen, colors, backgrounds, interface accents, and surrounding visual atmosphere.

---

## 2. CORE CONCEPT AND FUNCTIONALITY

The application revolves around one primary object: a virtual iPod.

The iPod should not be a flat image or a static illustration. It must be an actual interactive 3D object rendered inside the website.

Its physical appearance should include:

- A recognizable iPod-shaped body.
- Rounded metallic or plastic edges.
- A reflective front surface.
- A dedicated display screen.
- A circular click wheel.
- A center selection button.
- Functional navigation controls.
- Realistic shadows and lighting.
- Subtle reflections and depth.

The device should be presented as an object that exists within a virtual environment rather than simply being an image placed on a webpage.

IMPORTANT: The 3D device is the primary interface. The website itself should support and complement the device, not overpower it.

---

## 3. DYNAMIC ALBUM-ART THEME CLASSIFICATION

This is the application's most important distinguishing feature.

The iPod should automatically adapt its visual theme to the currently playing song's album artwork.

For example:

| Album artwork characteristics | Resulting iPod theme |
|---|---|
| Blue-dominant artwork | Blue interface accents and atmosphere |
| Red-dominant artwork | Red interface accents |
| Black-and-white artwork | Monochrome interface |
| Pink artwork | Pink interface accents |
| Green artwork | Green interface accents |
| Dark artwork | Darker screen and ambient lighting |
| Bright artwork | Brighter interface and lighting |

### 3.1 Theme extraction system

The application should analyze the selected album cover and extract:

1. Dominant color.
2. Secondary color.
3. Accent color.
4. Background color.
5. Overall brightness.
6. Color saturation.

These colors should be translated into a consistent visual theme.

The application should use image color extraction rather than manually assigning colors to individual albums.

### 3.2 Elements affected by the theme

The extracted colors should influence:

- iPod screen background.
- Progress bar.
- Selected menu items.
- Click wheel illumination, if enabled.
- Song title accents.
- Ambient lighting around the device.
- Background gradients.
- Subtle reflections.
- Loading and transition animations.

IMPORTANT: The album artwork itself must remain recognizable and unaltered. The theme extraction system should complement the cover, not replace it.

### 3.3 Theme transitions

When switching songs, the theme should transition smoothly.

For example:

- Previous song: predominantly blue.
- Next song: predominantly pink.
- The interface gradually transitions from blue to pink.
- The album artwork changes with a subtle fade.
- The progress indicator and surrounding atmosphere adapt.

Avoid abrupt color changes or excessive animations.

---

## 4. THREE-DIMENSIONAL DEVICE CLASSIFICATION

The 3D device should be constructed using a proper 3D rendering system.

### 4.1 Physical components

| Component | Required characteristics |
|---|---|
| Main body | Rounded rectangular iPod enclosure |
| Front panel | Glossy, reflective surface |
| Display | Recessed or integrated screen |
| Click wheel | Circular physical control |
| Center button | Separate clickable selection control |
| Outer edges | Rounded and dimensional |
| Rear panel | Metallic finish |
| Lighting | Realistic directional lighting |
| Shadows | Soft contact and environmental shadows |

### 4.2 3D interaction

The device should support:

- Dragging to rotate the iPod.
- Horizontal and vertical viewing angles.
- Gentle automatic idle rotation.
- Zooming in and out.
- Touch gestures on mobile.
- Returning to the default viewing angle.
- Smooth movement and realistic inertia.

The default presentation should show the front of the iPod at a slight three-quarter angle, allowing the user to appreciate its thickness and physical structure.

### 4.3 Click wheel functionality

The click wheel must be a working interactive component.

| Region | Function |
|---|---|
| Top | Previous track / rewind |
| Bottom | Next track / fast-forward |
| Left | Navigate backward |
| Right | Navigate forward |
| Center | Select / confirm |
| Circular movement | Scroll through menus |

The controls must be usable through touch and mouse interaction.

On mobile, the wheel should have appropriately sized touch regions so its functions are not difficult to activate.

---

## 5. APPLICATION NAVIGATION AND INTERFACE

The application should maintain the simplicity of classic iPod software.

Its interface should be organized into the following screens.

### A. NOW PLAYING

- Album artwork.
- Song title.
- Artist name.
- Album name.
- Playback progress.
- Current time and duration.
- Play/pause and skip controls.

### B. MUSIC LIBRARY

- All songs.
- Artists.
- Albums.
- Genres.
- Playlists.
- Recently added.
- Recently played.

### C. PLAYLISTS

- Create playlists.
- Add and remove songs.
- Rename playlists.
- Reorder songs.
- Shuffle playlist.

### D. SETTINGS

- Sound and volume.
- Equalizer.
- Repeat and shuffle.
- Device appearance.
- 3D viewing controls.
- Theme behavior.

### 5.1 Navigation behavior

The application should support two navigation methods:

PHYSICAL NAVIGATION:
Using the virtual click wheel.

DIRECT NAVIGATION:
Tapping or clicking interface elements on the iPod display.

Both methods must produce the same results.

---

## 6. MUSIC PLAYBACK CLASSIFICATION

The music player must be a functional audio application, not just a visual prototype.

### 6.1 Playback features

- Play.
- Pause.
- Resume.
- Previous track.
- Next track.
- Seek through a song.
- Volume adjustment.
- Shuffle.
- Repeat one.
- Repeat all.
- Queue management.
- Playback progress.
- Automatic next-track playback.

### 6.2 Audio behavior

The audio should continue playing when the user interacts with other parts of the website.

Playback must not restart unnecessarily when:

- Changing the 3D camera angle.
- Opening the music library.
- Changing the theme.
- Opening settings.
- Switching between application screens.

The audio engine should be independent of the 3D rendering system.

### 6.3 Music metadata

Every song should support the following information:

| Property | Description |
|---|---|
| Title | Song name |
| Artist | Performing artist |
| Album | Album title |
| Artwork | Album cover |
| Duration | Song length |
| Audio source | Actual playable audio file or authorized stream |
| Genre | Musical category |
| Track number | Position within the album |

Missing metadata should be handled gracefully.

---

## 7. MUSIC SOURCE AND WEEZER INTEGRATION CLASSIFICATION

This section requires particular attention.

The website should be designed to connect to the music application called WEEZER that I intend to use.

However, there is an important technical distinction between importing music and integrating with another application's internal systems.

### 7.1 Music source module

The music source system should support these potential methods:

| Source method | Function |
|---|---|
| Local audio import | Import audio files from the device |
| Metadata import | Read song titles, artists and album information |
| Artwork import | Obtain or upload album covers |
| Authorized streaming integration | Connect to a supported external music service |
| Manual song entry | Allow users to add missing metadata |

### 7.2 Weezer connection

The integration should be investigated before implementation.

Claude should:

1. Identify the exact Weezer application.
2. Determine whether it exposes an API or authorized integration method.
3. Determine whether it supports sharing audio files or playlists.
4. Determine whether song metadata and album artwork can be exported.
5. Determine whether playback can be controlled externally.
6. Implement only supported integration methods.

If no supported API exists, the website must not pretend that it is directly connected.

Instead, provide a local audio import system, with metadata and album artwork importing wherever supported.

### 7.3 Important compatibility requirement

The website should never depend entirely on Weezer to function.

Even without an external music connection, users should be able to:

- Import their own audio files.
- Play music locally.
- Create playlists.
- Change album artwork.
- Generate dynamic themes.
- Use the 3D iPod.
- Save their library.

This makes the application independently functional.

---

## 8. APPLICATION ARCHITECTURE CLASSIFICATION

The project should be separated into independent systems rather than developed as one enormous component.

### Main application systems

1. 3D Device Engine
   - Model.
   - Camera.
   - Lighting.
   - Materials.

2. Audio Engine
   - Playback.
   - Volume.
   - Queue.
   - Track transitions.

3. Theme Engine
   - Artwork color extraction.
   - Dynamic theme generation.
   - Color transitions.

4. Music Library
   - Songs.
   - Albums.
   - Artists.
   - Playlists.

5. Navigation
   - Menus.
   - Click wheel.
   - Selection states.

6. Integration
   - Weezer adapter.
   - Local music import.
   - External music services where supported.

7. Storage
   - Preferences.
   - Music metadata.
   - Playlists.
   - Persistent settings.

8. Interface
   - Responsive layout.
   - Screen transitions.
   - Animations.

### 8.1 Recommended technology classification

| Technology | Responsibility |
|---|---|
| HTML5 | Application structure |
| CSS3 | Interface styling |
| JavaScript / TypeScript | Application logic |
| React | Component architecture |
| Three.js | 3D rendering |
| React Three Fiber | 3D integration with React |
| Drei | 3D utilities and controls |
| Web Audio API | Audio processing |
| HTML Audio | Music playback |
| IndexedDB | Local music metadata and library |
| Local Storage | Small preferences |
| GitHub | Source-code repository |
| Vercel | Website hosting and deployment |

These are recommended technologies, not requirements to use every library simultaneously.

### 8.2 Three-dimensional rendering

Use Three.js or React Three Fiber to construct the device.

The 3D model should be composed of individual geometries and materials rather than using a single flat image.

The materials should support:

- Metallic surfaces.
- Glossy plastic.
- Transparent screen layers.
- Reflective highlights.
- Rounded edges.
- Realistic lighting.

### 8.3 Audio architecture

The audio engine must operate independently of the rendering engine.

A 3D rendering error must never stop the music.

Likewise, changing the selected song should not require reconstructing the entire 3D device.

### 8.4 Storage architecture

The application should distinguish between:

- Audio files.
- Song metadata.
- Album artwork.
- User playlists.
- Playback preferences.
- Device appearance settings.

Use IndexedDB for persistent local library data and avoid placing large audio files in Local Storage.

---

## 9. DYNAMIC INTERFACE BEHAVIOR

The application should respond intelligently to user actions.

| User action | Expected application response |
|---|---|
| Select a song | Load its metadata and artwork |
| Start playback | Begin audio and update progress |
| Change song | Update artwork and theme |
| Rotate iPod | Move the 3D camera or device |
| Scroll click wheel | Navigate menu selection |
| Open album | Display its track listing |
| Select playlist | Load playlist contents |
| Change volume | Adjust actual audio volume |
| Refresh website | Restore saved preferences and library metadata |
| Import new song | Add it to the music library |

### 9.1 Visual effects

Animations should be polished but restrained.

Recommended effects:

- Smooth screen transitions.
- Album artwork crossfades.
- Subtle 3D rotation.
- Click wheel interaction feedback.
- Progress bar animations.
- Dynamic ambient lighting.
- Button press animations.
- Screen loading transitions.

Avoid excessive glowing effects, unnecessary particles, and overwhelming gradients.

The application should feel like a premium physical music device.

---

## 10. USER INTERFACE DESIGN CLASSIFICATION

The visual direction should combine classic Apple iPod design with modern 3D product visualization.

### 10.1 Visual hierarchy

1. The 3D iPod must be the dominant visual element.
2. The music display must be readable.
3. The click wheel must be easily accessible.
4. Secondary controls must remain unobtrusive.
5. Additional settings should not clutter the main experience.

### 10.2 Responsive layout

DESKTOP:

- Larger 3D device.
- Room for library and playback information.
- Mouse-based rotation.
- Optional side navigation.

MOBILE:

- Centered 3D iPod.
- Touch-friendly click wheel.
- Compact navigation.
- Responsive screen sizing.
- No horizontal overflow.
- Performance-conscious 3D rendering.

The mobile version must not be a squeezed desktop layout. It should be intentionally designed for touchscreens.

---

## 11. GITHUB DEVELOPMENT AND DEPLOYMENT CLASSIFICATION

GitHub should serve as the application's source-code management environment.

The project should have a clean, organized repository.

### Recommended repository structure

```text
3d-ipod-player/
│
├── public/
│   ├── models/
│   ├── textures/
│   ├── icons/
│   └── fonts/
│
├── src/
│   ├── components/
│   │   ├── IPod/
│   │   ├── ClickWheel/
│   │   ├── Display/
│   │   ├── Controls/
│   │   └── Navigation/
│   │
│   ├── three/
│   │   ├── IPodModel/
│   │   ├── Materials/
│   │   ├── Lighting/
│   │   └── Camera/
│   │
│   ├── music/
│   │   ├── AudioEngine/
│   │   ├── MusicLibrary/
│   │   ├── Playlists/
│   │   └── Metadata/
│   │
│   ├── themes/
│   │   ├── ColorExtraction/
│   │   ├── ThemeGenerator/
│   │   └── Transitions/
│   │
│   ├── integrations/
│   │   ├── Weezer/
│   │   └── LocalImport/
│   │
│   ├── storage/
│   ├── hooks/
│   ├── styles/
│   ├── App.tsx
│   └── main.tsx
│
├── index.html
├── package.json
├── tsconfig.json
├── vite.config.ts
└── README.md
```

This is an initial organizational classification. Claude may adjust the structure when necessary, provided that the application remains modular.

### 11.1 GitHub workflow

1. Repository creation:
   Create a dedicated GitHub repository for the application.

2. Project initialization:
   Configure React, TypeScript, Vite and the required dependencies.

3. Core development:
   Develop the 3D device, audio engine, navigation and theme system.

4. Testing:
   Test functionality, responsiveness, audio playback and 3D performance.

5. GitHub synchronization:
   Commit and push completed changes to the repository.

6. Deployment:
   Connect the GitHub repository to Vercel and deploy the website.

---

## 12. PERFORMANCE AND COMPATIBILITY CLASSIFICATION

The application should prioritize actual usability over visual complexity.

### Required performance considerations

- Lazy-load 3D resources.
- Compress textures.
- Optimize 3D geometry.
- Avoid unnecessarily high polygon counts.
- Avoid rendering the 3D scene when it is not visible.
- Prevent unnecessary React re-renders.
- Preserve audio playback during interface updates.
- Handle missing audio files.
- Handle interrupted playback.
- Provide loading and error states.

### Device compatibility

| Environment | Requirement |
|---|---|
| iPhone Safari | Touch controls and responsive layout |
| Android Chrome | Touch controls and responsive layout |
| Desktop Chrome | Full functionality |
| Desktop Safari | Full functionality |
| Firefox | Core functionality |

A particularly important requirement is compatibility with older mobile hardware.

The application should provide a lower-quality 3D rendering option if the device struggles with the default graphics settings.

---

## 13. FUNCTIONAL REQUIREMENTS AND QUALITY ASSURANCE

The application must be tested against actual functionality, not merely whether the website looks complete.

| ID | Requirement | Priority |
|---|---|---|
| FR-01 | Render an actual 3D iPod | Critical |
| FR-02 | Functional virtual click wheel | Critical |
| FR-03 | Play real audio files | Critical |
| FR-04 | Display album artwork | Critical |
| FR-05 | Automatically generate album-based themes | Critical |
| FR-06 | Change songs without restarting the application | Critical |
| FR-07 | Create and manage playlists | High |
| FR-08 | Import local music | Critical |
| FR-09 | Save music library metadata | High |
| FR-10 | Support touch and mouse controls | Critical |
| FR-11 | Implement responsive mobile layout | Critical |
| FR-12 | Integrate with supported external music sources | High |
| FR-13 | Smooth 3D animations | High |
| FR-14 | Restore preferences after refreshing | High |

### Completion criteria

The project should not be considered complete until all of the following are demonstrated:

- [ ] The iPod is genuinely three-dimensional.
- [ ] Its click wheel actually works.
- [ ] Music can be imported and played.
- [ ] Album artwork appears correctly.
- [ ] Themes automatically adapt to album artwork.
- [ ] Music continues playing during navigation.
- [ ] Playlists can be created and edited.
- [ ] The application works on mobile.
- [ ] Saved information survives refreshing.
- [ ] No major buttons are decorative or nonfunctional.
- [ ] No critical console errors remain.
- [ ] The GitHub repository contains the complete source code.
- [ ] The deployed website is accessible.

---

## 14. DEVELOPMENT PRIORITIES

Claude should develop the application in stages instead of attempting everything simultaneously.

### PHASE 1 — FOUNDATION AND 3D DEVICE

Build:

- Website structure.
- iPod body.
- Display.
- Click wheel.
- Camera.
- Lighting.

### PHASE 2 — MUSIC ENGINE

Implement:

- Local audio import.
- Playback.
- Metadata.
- Queues.
- Playlists.

### PHASE 3 — DYNAMIC ALBUM THEMES

Implement:

- Artwork analysis.
- Color extraction.
- Theme generation.
- Transitions.

### PHASE 4 — NAVIGATION AND INTERACTIONS

Connect:

- Click wheel.
- Menus.
- Display.
- Playback controls.

### PHASE 5 — EXTERNAL INTEGRATIONS

Investigate and implement Weezer connectivity where technically supported.

### PHASE 6 — OPTIMIZATION AND DEPLOYMENT

Complete:

- Mobile compatibility.
- Bug fixes.
- Performance optimization.
- GitHub synchronization.
- Vercel deployment.

---

## 15. FINAL PRODUCT DEFINITION

PROJECT NAME: 3D iPod

PRODUCT CATEGORY: Dynamic, album-driven digital music experience.

### Product vision

A virtual music device that combines the nostalgia and physical interaction of the original iPod with modern web technology, three-dimensional rendering, personalized album aesthetics and functional music playback.

### Defining characteristic

Every song gives the iPod a different visual identity.

The album artwork determines the atmosphere of the device, making the listening experience visually connected to the music itself.

### Final expectations

- A real 3D iPod, not a static illustration.
- Fully functional music playback.
- Dynamic album-art-based themes.
- Interactive physical-style controls.
- A functional music library.
- Local audio import.
- Supported external music integrations.
- Persistent storage.
- Mobile and desktop compatibility.
- Complete GitHub source code.
- Working deployed website.

The result should be a polished, functional, visually immersive music application.

---

# 16. IMPORTANT DEVELOPMENT REQUIREMENTS FOR CLAUDE

1. Do not create a static mockup and present it as a completed application.
2. Do not use a flat iPod image as a substitute for the actual 3D device.
3. Do not create decorative controls that do not work.
4. Do not simulate audio playback without playing actual audio.
5. Do not hardcode album themes when they can be extracted dynamically.
6. Do not pretend to have connected to Weezer without a verified integration.
7. Do not put the entire application into one component.
8. Keep the audio engine independent of the 3D rendering system.
9. Make the website responsive, especially for mobile Safari.
10. Test every implemented feature.
11. Fix errors instead of hiding them.
12. Maintain the complete project through GitHub.
13. Use Vercel for deployment if appropriate.
14. Provide clear documentation for installation, configuration and deployment.
15. Do not claim that an implementation is finished until it has actually been tested.

END OF APPLICATION CLASSIFICATION.