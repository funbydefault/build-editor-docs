# Build Editor 1.0

Initial public release.

- In-game walls, rooms, floors, doors, windows, straight stairs, beams and rectangular gable roofs with live previews and validated edits.
- Furniture placement, support surfaces, move/copy, free placement, rotation, scoped erase and surface/room painting.
- Floor levels, wall views, configurable native top-down camera, orbit fallback and a walking visitor.
- Mouse/keyboard and configurable gamepad controls, including interface pointing and an on-screen text keyboard.
- Editor setup, catalog authoring, reusable profiles, interface themes and UMG replacements.
- Named local save library, Undo/Redo, optional automatic recovery and developer diagnostics.
- One playable showcase map and 38 furnishing models with three LODs.

## Documentation update : 15 October 2026

- Added a screenshot-led Quick Start from plugin setup to the first room in your own level.
- Updated the editor, catalog, profile, validation and appearance instructions for the sidebar layout.


## Scope

Local single-player editing. Architecture uses grid-aligned walls, straight stairs and rectangular gable roofs. Touch, network authority and cloud storage are outside this version.

## Existing saved designs

The current schematic format is 6. Readers accept formats 1-6. Older formats receive default closed opening states and inherit the appearances available in their original format. Earlier plugin builds cannot read format 6. Back up saves before changing stable catalog IDs, dimensions or grid settings. Unrecognized or incompatible designs are rejected before changing the scene.
