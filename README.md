# Planet Noise Map

A test project for learning procedural generation techniques, Godot 3D development, and space game programming concepts with realistic physics simulation.

## Project Purpose

This project was created as a learning exercise to explore:

- **Procedural generation** algorithms for solar systems
- **Godot 4.2** 3D capabilities and scene management
- **Space physics simulation** with real astronomical constants
- **Noise-based terrain generation** for planet surfaces

## Features

- **Procedural Solar System Generation**: Creates random star systems with 0-12 planets
- **Realistic Physics**: Uses actual astronomical constants (Sun radius: 700,000 km, Earth radius: 6,300 km)
- **Environmental Zones**: Planets are placed based on:
  - Goldilocks zone (habitable region)
  - Frost line calculations
  - Roche limit (minimum safe distance)
  - Hill sphere (gravitational influence)
- **Multiple Planet Types**: Star, Terrestrial, Gaseous, Lava, Ice, No Atmosphere, Sand
- **3D Camera System**: Free-look camera with WASD movement and mouse control
- **Orbital Mechanics**: Planets orbit stars with proper angular velocity

## Technical Overview

- **Engine**: Godot 4.2 with Forward Plus rendering
- **Noise Generation**: FastNoiseLite for procedural planet generation
- **External Addon**: naejimer_3d_planet_generator for planet mesh creation
- **Scaling**: Real astronomical units scaled to Godot coordinate system (scale factor: 0.0000007)

## Usage

1. Open the project in Godot 4.2
2. Run the main scene (`main.tscn`)
3. Click "spawn Star" button to generate a new star system
4. Use **WASD** keys to move the camera
5. Hold **right mouse button** and move mouse to look around
6. Use **mouse wheel** to adjust movement speed

## Learning Goals

This project helped me learn:

- Procedural generation algorithms and noise functions
- 3D game development in Godot
- Space physics simulation and astronomical calculations
- Scene management and node relationships
- Camera systems and user input handling

## Stretch Goals

- **Multiple Star Systems**: Planned implementation of several star systems based on noise representing gravitational hotspots
- **Galaxy Generation**: Procedural galaxy with interconnected star systems

_These stretch goals remain planned features if I return to the project._

## Controls

- **W/A/S/D**: Move camera forward/left/back/right
- **Q/E**: Move camera down/up
- **Right Mouse**: Look around (mouse capture)
- **Mouse Wheel**: Adjust movement speed
- **Shift**: Speed multiplier
- **Button**: Generate new star system

## Project Structure

- `Node3D.gd`: Main system controller with physics calculations
- `camera.gd`: Free-look camera implementation
- `main.tscn`: Main scene with UI and system setup
- `addons/`: 3D planet generator addon
- `bg_space_seamless.png`: Space background texture