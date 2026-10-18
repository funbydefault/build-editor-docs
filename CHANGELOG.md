# Build Editor 1.0

Initial public release.

- In-game walls, rooms, floors, doors, windows, straight stairs, beams and rectangular gable roofs with live previews and validated edits.
- Furniture placement, support surfaces, move/copy, free placement, rotation, scoped erase and surface/room painting.
- Floor levels, wall views, configurable native top-down camera, orbit fallback and a walking visitor.
- Mouse/keyboard and configurable gamepad controls, including interface pointing and an on-screen text keyboard.
- Editor setup, catalog authoring, reusable profiles, interface themes and UMG replacements.
- Named local save library, Undo/Redo, optional automatic recovery and developer diagnostics.
- One playable showcase map with switchable Home and Sci-fi scenes, 38 home furnishing models and 12 station equipment models with three LODs.

## Documentation update : 15 October 2026

- Added a screenshot-led Quick Start from plugin setup to the first room in your own level.
- Updated the editor, catalog, profile, validation and appearance instructions for the sidebar layout.


## Setup update : 17 October 2026

- Shortened the Basic-level Quick Start by removing the extra ground and save steps.
- Added an existing-GameMode setup action that creates a child with the supplied controller, camera and HUD.
- Added a Camera page for active view settings and movement speeds.
- Organized generated actors by floor and piece type in the editor Outliner.

## Scene and alignment update : 17 October 2026

- Added a complete Sci-fi conversion in the same map, with its own catalog, materials, decorations, interface and camera profile. The scene button preserves each scene's edits during Play.
- Exposed native frame, glass and hardware styling, including flush openings and roof surface materials.
- Aligned gables, roof edges, ceilings and wall ends with the configured wall thickness.
- Unified opening dimensions across windows, frames, glass, wall cutouts and selection outlines. Custom opening meshes fit the configured width, height and sill.

## Maintenance update : 18 October 2026

- Removed unreachable duplicate opening geometry code. Existing save readers and serialized asset compatibility remain available.
- Removed an unused background material and fixed direct header includes required by clean game builds.
- Aligned custom wall meshes to wall edges and configured thickness. Catalog IDs no longer change mesh sizing.
- Clarified the built-in Procedural Mesh Component dependency and its experimental API status in UE 5.4.

## Shared building and audio update : 18 October 2026

- Added server-approved shared construction for listen-server games, including late joining, reconnect, independent player cameras and personal Undo/Redo.
- Added Blueprint permission checks, edit limits and access to the player responsible for an accepted server edit.
- Shared Home/Sci-fi switches preserve each scene's edits and update every player's profile and presentation.
- Added optional scene music and ambience with local volume and mute controls.

## Scope

Standalone and shared editing in listen-server games. Architecture uses grid-aligned walls, straight stairs and rectangular gable roofs. Your game supplies hosting, joining and persistent storage. Touch, split-screen and cloud storage are outside this version.

## Existing saved designs

The current schematic format is 6. Readers accept formats 1-6. Older formats receive default closed opening states and inherit the appearances available in their original format. Earlier plugin builds cannot read format 6. Back up saves before changing stable catalog IDs, dimensions or grid settings. Unrecognized or incompatible designs are rejected before changing the scene.
