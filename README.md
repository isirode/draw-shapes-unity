# Draw 2D Physics Shapes in Unity3D

This is a fork of https://github.com/Hyperparticle/draw-shapes-unity.

This tutorial project provides an example of how to draw shapes with the cursor in Unity similar to [IncrediBots](http://incredibots.com/if/game.php) or [Phun (now Algodoo)](http://www.algodoo.com/).

The core logic of this project uses vertices specified from the cursor's coordinates to dynamically generate and configure a mesh, outline, and 2D collider.

- [Go to the Tutorial](https://medium.com/@hyperparticle/draw-2d-physics-shapes-in-unity3d-2e0ec634381c) to read about how it works in greater detail.
- [Play it in your browser](https://simmer.io/@hyperparticle/draw-2d-physics-shapes)
- [Unity Asset Store Bundle](https://www.assetstore.unity3d.com/#!/content/105996)

[![Draw Shapes Preview](docs/draw-shapes-unity-preview-short.gif "Blog Post")](https://hyperparticle.com/2d-physics-shapes)

## Project Overview

Requires Unity3D (tested with 2017.x, but should also work with 5.x)

```
./Isirode/draw-shapes-unity
├── Scenes
|   └── Main.unity              - The project's main scene
├── Prefab
|   ├── Circle.prefab           - Circle physics shape
|   ├── Platform.prefab         - Stationary rectangular physics platform
|   ├── Rectangle.prefab        - Rectangle physics shape
|   ├── RotatingPlatform.prefab - Rotating rectangular physics platform
|   └── Triangle.prefab         - Triangle physics shape
└── Scripts
    ├── DrawCircle.cs           - Creates circle meshes and colliders
    ├── DrawController.cs       - Captures mouse input and creates shapes
    ├── DrawRectangle.cs        - Creates rectangle meshes and colliders
    ├── DrawShape.cs            - Base class for all shapes
    ├── DrawTriangle.cs         - Creates triangle meshes and colliders
    ├── ExplosionController.cs  - Generates explosion forces at the cursor
    ├── TestPolygon.cs          - Demonstrates how to draw polygon meshes
    ├── Triangulator.cs         - Generates triangles from polygon vertices
    └── Util.cs                 - Provides handy operations on vectors
```

## Running the Project

To run the project, open `Scenes/Main.unity` and click on the play button.

In the main scene there will be three buttons: square, circle, and triangle. Click on one of the buttons and then click 2-3 points in the game view to draw and release a physics shape. The shape will react to gravity and interact with other objects in the scene.

## Importing the project

You can add this package as a git url : "https://github.com/isirode/draw-shapes-unity.git?path=/Assets/Isirode/draw-shapes-unity#0.0.3".
The project will be added to your "Packages" folder, the scenes will be read-only, if you want to open them, just copy them in your Assets folder and they will be usable.

You can also download the .unitypackage of the version you want, here for instance https://github.com/isirode/draw-shapes-unity/releases/tag/0.0.3 and add it manually to your project.
This should import the project in your Assets folder.
