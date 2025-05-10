
![ascii-text-art](https://github.com/Dambylik/42_cub3D/blob/main/cub3de.png)


# cub3D

## Table of Contents

- [Project Overview](#project-overview)
- [Summary](#summary)
- [Project Goals](#project-goals)
- [Project Requirements](#project-requirements)
- [Screenshots and Demos of our project](#screenshots-and-demos-of-our-project)
- [Team Development Steps](#team-development-steps)
  - [1. Project Setup](#1-project-setup)
  - [2. Parsing Configuration File](#2-parsing-configuration-file)
  - [3. Initialize Graphics](#3-initialize-graphics)
  - [4. Raycasting Engine](#4-raycasting-engine)
  - [5. Texture Mapping](#5-texture-mapping)
  - [6. Player Movement and Controls](#6-player-movement-and-controls)
  - [7. Rendering Game World](#7-rendering-game-world)
  - [8. Error Handling and Cleanup](#8-error-handling-and-cleanup)
  - [9. Optimization and Refactoring](#9-optimization-and-refactoring)
  - [10. Bonus Features (Optional)](#10-bonus-features-optional)
- [Project Structure](#project-structure)
- [I. Project Setup](#i-project-setup)
  - [Step 1: Setup](#step-1-setup)
  - [Step 2: Create Files](#step-2-create-files)
- [II. Parsing Configuration File](#ii-parsing-configuration-file)
  - [Map requirements](#map-requirements)
  - [Prsing and Storing the Configuration File](#prsing-and-storing-the-configuration-file)
- [III. Initialize Graphics](#iii-initialize-graphics)
- [Resources](#resources)
  - [Video resources](#video-resources)


## Project Overview

Welcome to our cub3d project! As a team, we'll be diving into the exciting world of raycasting and basic 3D graphics programming. Our main goal is to create a simple 3D maze game from scratch using raycasting techniques.

## Summary

This project is inspired by the world-famous [Wolfenstein 3D game](https://en.wikipedia.org/wiki/Wolfenstein_3D), which was the first FPS ever. It is a remarkable technique to explore, and a great opportunity to create a game with a good design and a nice user interface.

![cool-guys-1992-small](https://github.com/zelhajou/42-cub3D/assets/39954629/e53038ee-d9ed-43fa-8f58-44ee63a5ede3)

Developed by [id Software](https://en.wikipedia.org/wiki/Id_Software) and published by [Apogee Software](https://en.wikipedia.org/wiki/Apogee_Software), Wolfenstein 3D was released in 1992. It was a revolutionary game that popularized the FPS genre and helped establish the PC as a gaming platform.

[Playable Wolfenstein 3D](http://users.atw.hu/wolf3d/)

## Project Goals

1. **Raycasting Engine**: Develop a raycasting engine to render a 3D world from a first-person perspective.
2. **Parsing Configuration File**: Read and parse a configuration file (.cub) to define our game settings, including map layout, textures, and other parameters.
3. **Texture Mapping**: Apply textures to walls and potentially the floor and ceiling to enhance our game's visual appearance.
4. **Player Movement and Controls**: Implement controls to allow the player to move within the 3D world, including basic movement (e.g., forward, backward, strafing) and rotation.
5. **Basic Game Mechanics**: Create a playable game where the player can navigate through a maze-like environment, interact with objects, and complete objectives.
6. **Error Handling and Optimization**: Implement robust error handling to handle invalid input and prevent crashes. Optimize our code for performance to ensure smooth gameplay.

## Project Requirements

- **Language**: We'll be using C for this project.
- **Libraries**: We can use standard libraries like `math`. External libraries like `minilibx` are allowed for graphics rendering.
- **Map Configuration**: Our game should read a map configuration file (.cub) that defines game settings, including map layout, textures, colors, and more.
- **Graphics**: The game must render a 3D perspective view of the game world using raycasting techniques. Textures should be applied to walls to enhance the visual appearance.
- **Controls**: Implement controls to allow the player to move and navigate within the 3D world using keyboard input.

## Screenshots of our project

| | |
|:-------------------------:|:-------------------------:|
| <img width="1230" alt="Screen Shot 2024-05-09 at 12 22 47 PM" src="https://github.com/Dambylik/42_cub3D/blob/main/Screenshot%20From%202025-05-10%2019-27-48.png"> | <img width="1245" alt="Screen Shot 2024-05-09 at 12 24 31 PM" src="https://github.com/Dambylik/42_cub3D/blob/main/Screenshot%20From%202025-05-10%2019-27-25.png">
| <img width="1346" alt="Screen Shot 2024-05-09 at 12 47 45 PM" src="https://github.com/Dambylik/42_cub3D/blob/main/Screenshot%20From%202025-05-10%2019-24-07.png"> | <img width="1288" alt="Screen Shot 2024-05-09 at 12 40 14 PM" src="https://github.com/Dambylik/42_cub3D/blob/main/Screenshot%20From%202025-05-10%2019-23-39.png"> |


## Team Development Steps

As a team, we'll be tackling the cub3d project in a systematic manner to ensure a successful outcome. Here's our proposed development roadmap:

### 1. Project Setup

Set up the project repository, establish communication channels, and assign roles.

- [x] **Create Repository**: Set up a Git repository for the project.
- [x] **Establish Communication**: Choose communication tools (Discord) for team collaboration.
- [x] **Assign Roles**: Define roles and responsibilities for each team member.

### 2. Parsing Configuration File

Implement the code to read and parse the configuration file (.cub) to extract game settings.

- [x] **Read File**: Open and read the .cub configuration file.
- [x] **Validate Data**: Check for valid map settings, resolution, textures, etc.
- [x] **Parse Data**: Extract and store relevant information from the configuration file.

### 3. Initialize Graphics

Set up the graphics rendering engine using the `minilibx` library.

- [x] **Initialize Minilibx**: Set up the Minilibx library for graphics rendering.
- [x] **Create Window**: Create a window for rendering the game.
- [x] **Setup Buffer**: Set up a buffer for rendering pixels to the window.

### 4. Raycasting Engine

Develop the raycasting engine to render a 3D perspective view of the game world.

- [x] **Initialize Ray**: Start with the player's position and direction.
- [x] **Cast Rays**: Cast rays from the player's position to calculate distances to walls.
- [x] **Calculate Wall Strips**: Determine the height and texture of each wall strip to draw.

### 5. Texture Mapping

Apply textures to walls to enhance the visual appearance of the game.

- [x] **Load Textures**: Load wall and sprite textures from files.
- [x] **Implement Texture Mapping**: Apply textures to the rendered walls.

### 6. Player Movement and Controls

Implement controls to allow the player to move and navigate within the 3D world.

- [x] **Handle Input**: Implement controls for player movement (e.g., WASD for movement, arrow keys for rotation).
- [x] **Update Player Position**: Update the player's position based on input and collision detection.

### 7. Rendering Game World

Render the game world using the raycasting results and textures.

- [x] **Draw Walls**: Render the walls of the 3D world using the raycasting results.
- [x] **Draw Floor and Ceiling**: Render the floor and ceiling of the 3D world.
- [ ] **Draw Sprites**: Implement sprite rendering if necessary.

### 8. Error Handling and Cleanup

Implement error handling to prevent crashes and ensure a smooth user experience.

- [x] **Error Checks**: Implement error handling to catch and handle any runtime errors.
- [x] **Memory Cleanup**: Free allocated memory and resources.
- [x] **Close Window**: Properly close the graphics window when exiting the game.

### 9. Optimization and Refactoring

Optimize the code for performance and refactor as needed for better readability.

- [x] **Optimize Raycasting**: Improve raycasting performance if necessary.
- [x] **Refactor Code**: Clean up and organize the code for better readability and maintainability.


## Project Structure

The project will be structured as follows:

```
cub3d/
│
├── correct_maps
├── error_maps
├── includes
│   ├── cub3d.h
│   └── minilibx-linux
├── Makefile
├── src
│   ├── libft
│   ├── main.c
│   ├── parsing
│   ├── RayCasting
│   └── start_mlx
│  
└── textures

```

## Resources

### Researched Topics

- [Wolfenstein 3D](https://en.wikipedia.org/wiki/Wolfenstein_3D)
- [How do games render their scenes? | Bitwise](https://youtu.be/Oct4Oi-KfVQ)
- [How do Video Game Graphics Work?](https://youtu.be/C8YtdC8mxTU?list=PLzjH3XFHoi6jTjDid_O3BEa-VRIqzoZ_U)
- [How Rendering Graphics Works in Games!](https://youtu.be/cvcAjgMUPUA)

### [Mathematics]

- [The Math behind (most) 3D games - Perspective Projection](https://youtu.be/U0_ONQQ5ZNM)

**Trigonometry:** Essential for dealing with angles and rotations in 3D space. You'll frequently use trigonometric functions like sine, cosine, and tangent to calculate positions and angles.

Trigonometry is a branch of mathematics that deals with the relationships between the sides and angles of triangles. It is essential for understanding 3D graphics programming, as it helps you calculate positions, rotations, and other transformations in 3D space.

- [Trigonometry for Games (Making a Homing Rocket)](https://demoman.net/?a=trig-for-games)
- [Trigonometry - Easy to understand 3D animation](https://youtu.be/ovLbCvq7FNA)
- [Trigonometry in Game Development](https://www.youtube.com/watch?v=SEqFQl2ADi0)
- [Trigonometry | Gamedev Math](https://www.youtube.com/watch?v=FZ9HWff734c)
- [So how does your computer ACTUALLY compute sine? Basics of trig and more…](https://www.youtube.com/watch?v=kkMt4lrJzs8)
- [Trigonometry • Math for Game Devs [Part 3]](https://www.youtube.com/watch?v=1NLekEd770w)
- [Trigonometry - Khan Academy](https://www.khanacademy.org/math/trigonometry)
- [Trigonometry - Math is Fun](https://www.mathsisfun.com/algebra/trigonometry.html)
- [من أين جاءت النسب المثلثية وما أهميتها؟](https://youtu.be/LAn56tz1nX8?list=PLzjH3XFHoi6jTjDid_O3BEa-VRIqzoZ_U)

**linear algebra:** Linear algebra is a branch of mathematics that deals with vectors, matrices, and linear transformations. It is essential for understanding 3D graphics programming, as it helps you represent and manipulate objects in 3D space.

- [Linear Algebra - 3Blue1Brown](https://www.youtube.com/watch?v=kjBOesZCoqc)
- [Linear Algebra - Khan Academy](https://www.khanacademy.org/math/linear-algebra)
- [Linear Algebra - Math is Fun](https://www.mathsisfun.com/algebra/linear-equations.html)

**Vectors and Matrices:** Vectors and matrices are fundamental concepts in 3D graphics programming. You'll use them to represent positions, directions, transformations, and more.

Vector and Matrix is a very important concept in computer graphics. It is used to represent the position, direction, and transformation of objects in 3D space. It is also used to represent the color of the object, the texture of the object, and the light source in the scene.

- [Game Math Theory - VECTORS](https://youtu.be/wXI9_olSrqo)
- [Vectors and Matrices - 3Blue1Brown](https://www.youtube.com/watch?v=fNk_zzaMoSs)
- [Vectors and Matrices - Khan Academy](https://www.khanacademy.org/math/linear-algebra/vectors-and-spaces)
- [Vectors and Matrices - Math is Fun](https://www.mathsisfun.com/algebra/vectors.html)
- [Vectors and Matrices in Game Development](https://www.youtube.com/watch?v=7k03zkkvQv0)
- [Vectors and Matrices | Gamedev Math](https://www.youtube.com/watch?v=8M5d2MfK2Vg)
- [Linear Algebra - Matrix Transformations](https://www.youtube.com/watch?v=IrggOvOSZr4)

**Geometry:** Geometry is the branch of mathematics that deals with shapes, sizes, and properties of space. It is essential for understanding 3D graphics programming, as it helps you calculate positions, angles, and distances in 3D space.

- [Vectors & Dot Product • Math for Game Devs [Part 1]](https://www.youtube.com/watch?v=MOYiVLEnhrw)
- [Geometry - Khan Academy](https://www.khanacademy.org/math/geometry)
- [Geometry - Math is Fun](https://www.mathsisfun.com/geometry/index.html)

**Calculus:** Calculus is a branch of mathematics that deals with rates of change and accumulation. It is essential for understanding 3D graphics programming, as it helps you calculate velocities, accelerations, and other dynamic properties of objects in 3D space.

- [Calculus - Math is Fun](https://www.mathsisfun.com/calculus/index.html)
- [Calculus -- The foundation of modern science](https://www.youtube.com/watch?v=rjLJIVoQxz4)

### [Computer Graphics]

Computer graphics is a field of study that focuses on the creation, manipulation, and rendering of images using computers. It is essential for understanding how to create 2D and 3D graphics, animations, and visual effects.

- [History of computer graphics with Aymane Biri | BlaBlaConf 2021](https://www.youtube.com/watch?v=WlE5N_DSlq0&list=PLzjH3XFHoi6gh6md_WlQMcDZ8zZ1AoZov&index=2&t=571s&pp=gAQBiAQB)
- [Computer Graphics - Scratchapixel](https://www.scratchapixel.com/)
- [Computer Graphics from Scratch](https://www.gabrielgambetta.com/computer-graphics-from-scratch/)
- [Quick Understanding of Homogeneous Coordinates for Computer Graphics](https://www.youtube.com/watch?v=o-xwmTODTUI&list=PLzjH3XFHoi6jTjDid_O3BEa-VRIqzoZ_U&index=3&pp=gAQBiAQB)
- [What Is A Graphics Programmer?](https://www.youtube.com/watch?v=O-2viBhLTqI&list=PLzjH3XFHoi6jTjDid_O3BEa-VRIqzoZ_U&index=4&pp=gAQBiAQB)
- [How do Video Game Graphics Work?](https://www.youtube.com/watch?v=C8YtdC8mxTU&list=PLzjH3XFHoi6gh6md_WlQMcDZ8zZ1AoZov&index=1&t=580s&pp=gAQBiAQB)

### [Raycasting]

Raycasting is a rendering technique used to create a 3D perspective view of a scene from a 2D map. It is commonly used in video games to simulate 3D environments using 2D graphics.

- [Raycasting](https://en.wikipedia.org/wiki/Ray_casting)
- [Super Fast Ray Casting in Tiled Worlds using DDA](https://www.youtube.com/watch?v=NbSee-XM7WA)
- [RayCasting Tutorials by Lode Vandevenne](https://harm-smits.github.io/42docs/projects/cub3d) 
- [Matt Godbolt - Wolfenstein 3D's map renderer](https://www.youtube.com/watch?v=eOCQfxRQ2pY) ⭐
- [3DSage - Make Your Own Raycaster - Part 1](https://www.youtube.com/watch?v=gYRrGTC7GtA) 
- [3DSage - Make Your Own Raycaster - Part 2](https://www.youtube.com/watch?v=PC1RaETIx3Y) 
- [3DSage - Make Your Own Raycaster - Part 3](https://www.youtube.com/watch?v=w0Bm4IA-Ii8)
- [Pikuma - Raycasting](https://drive.google.com/drive/folders/1GzCshkJDq5x4EZHRnoir6g4YeQ-9lU_r)
- [Ray-Casting Tutorial by F. Permadi](https://permadi.com/1996/05/ray-casting-tutorial-table-of-contents)

### [MinilibX]

- [Introduction to the MinilibX](https://www.youtube.com/watch?v=bYS93r6U0zg)
- [x.org Documentation](https://www.x.org/wiki)
- [libX11 Documentation](https://www.x.org/releases/X11R7.6/doc/libX11/specs/libX11/libX11.html)

### [42 students articles]

- [Cub3D Tutorial [Using angles]. INTRODUCTION](https://medium.com/@afatir.ahmedfatir/cub3d-tutorial-af5dd31d2fcf)
 - [Jun Han Ng - Cub3D ](https://hackmd.io/@nszl/H1LXByIE2#introduction)
