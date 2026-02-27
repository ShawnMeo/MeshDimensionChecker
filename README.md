# Mesh Dimension Checker

A lightweight, web-based utility designed for 3D Technical Artists, Modeler, and Game Developers. This tool helps you quickly verify, transform, and scale 3D models against real-world references right in your browser—no software installation required.

## Why Use This?
When collaborating across different 3D software (Blender, Maya, Unreal Engine), models often suffer from scale discrepancies due to mismatched unit settings (e.g., 1 unit = 1cm vs 1m). This tool offers a fast, frictionless way to:
- **Sanity check proportions** before handing off assets to a game engine or other departments.
- **Instantly visualize scale** comparisons next to common real-world objects (humans, doors, cars, etc.).
- **Fix unit discrepancies** rapidly by applying scale multipliers and exporting directly back to GLB.

## Features & Workflow

### 1. Unified 3D Viewport
Drag and drop your `GLB`, `GLTF`, `OBJ`, `STL`, or `FBX` models straight into the viewport. You can navigate the 3D scene effortlessly using standard orbit controls.

### 2. Built-in Real-World References
Quickly spawn reference models directly alongside your asset to guarantee accurate scale. Available references include:
- Human (1.75m tall)
- Standard Door (2.1 x 0.9m)
- Soda Can (12.2 x 6.6cm)
- Car (4.5 x 1.5 x 1.8m)
- ...and more.

### 3. Move, Rotate, and Scale Gizmos (W, E, R)
Select any object in the scene and modify it using standard industry gizmo hotkeys:
- `W` - Move/Translate
- `E` - Rotate
- `R` - Scale

Transformations dynamically update alongside dimension displays (X, Y, Z axes) so you can precisely lock in your required metrics. 

### 4. Frame to Selection (F)
To orbit and zoom perfectly onto an object, simply select it and press `F` to frame your camera.

### 5. Non-Destructive Undo (Ctrl+Z)
Make a mistake while dragging a transform handle? No problem. The tool features an undo stack that tracks translation, rotation, and scale. Press `Ctrl+Z` (or `Cmd+Z` on Mac) to seamlessly revert an action.

### 6. Zero-Friction GLB Export
Once your model's scale matches your engine or project's rigorous standards, click **Export GLB** to instantly download the corrected asset, ready for pipeline integration.

## Usage Guide
1. Launch `index.html` in your browser.
2. Drag & drop your mesh into the scene.
3. Select a reference object from the right panel.
4. Use the side panel sliders *or* the `R` scale gizmo to shrink or enlarge your mesh. (Watch the numerical dimensions update in real-time).
5. Switch display units between Meters (m), Centimeters (cm), or Inches (in).
6. Click **Export GLB** when finished.

## Built With
- Three.js
- HTML5 / Vanilla JS
- CSS custom layouts (no external framework overhead)
