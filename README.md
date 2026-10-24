# Build Editor

Build Editor adds in-game building and furnishing to Unreal Engine projects. Players can draw rooms, walls and floors, place doors and windows, connect levels with straight stairs, add roofs, and decorate with furniture.

## Try the free demo

[Download the Windows demo](https://funbydefault.itch.io/build-editor-demo). Build and furnish a home or a sci-fi station without installing Unreal Engine. The download is the playable example; the paid plugin and Unreal editor tools are separate.

## Quick Start

Follow the [Documentation](https://funbydefault.github.io/build-editor-docs/#quick-start): enable the plugin, connect the supplied controls in **Tools > Build Editor > Setup**, then press **Play** and draw a room. Each step shows the actual editor control and expected result.

[![Build Editor Setup page with the main setup controls marked](quickstart-editor.png)](https://funbydefault.github.io/build-editor-docs/#quick-start)

Supports Unreal Engine 5.4–5.8 on Windows 64-bit. Guide screenshots use UE 5.4. The supplied setup works in a Blueprint-only game. A source-only installation needs Unreal's supported C++ build tools. Built-in dependencies are enabled automatically, including editor animation support for the supplied visitor.

- [Set up your own level](https://funbydefault.github.io/build-editor-docs/#quick-start)
- [Add building to an existing GameMode](https://funbydefault.github.io/build-editor-docs/#keep-your-existing-gamemode)
- [Add shared multiplayer building](https://funbydefault.github.io/build-editor-docs/#shared-multiplayer-building)
- [Change the camera](https://funbydefault.github.io/build-editor-docs/#change-the-camera)
- [Change the interface and placement controls](https://funbydefault.github.io/build-editor-docs/#customize-the-interface-and-build-interactions)
- [Create your own item catalog](https://funbydefault.github.io/build-editor-docs/#make-a-catalog)
- [Resize windows and doors](https://funbydefault.github.io/build-editor-docs/#resize-windows-and-doors)
- [Mouse, keyboard and gamepad controls](https://funbydefault.github.io/build-editor-docs/#default-controls)
- [Save builds and recover work](https://funbydefault.github.io/build-editor-docs/#schematic-saves)
- [Version notes](CHANGELOG.md)

The included map offers Home and Sci-fi scenes through one scene button. Each scene uses its own catalog, materials, interface theme, camera settings and audio. Use the same profile and scene assets to offer your own building styles.

## Scope

Standalone and shared building in listen-server games with grid-aligned walls, straight stairs and rectangular gable roofs. Shared sessions use server-approved edits, personal Undo/Redo and independent player cameras. Your game supplies hosting and joining. Touch, split-screen and cloud storage are outside version 1.0.

## Support

Contact [funbydefault.dev@gmail.com](mailto:funbydefault.dev@gmail.com). Include your plugin and Unreal Engine versions, the steps to reproduce the issue, and the diagnostic message if available.
