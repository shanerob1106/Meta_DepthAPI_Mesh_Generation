#Unity Mixed-Reality Room Mapper

## Overview
This Unity project is a mixed-reality application designed for the Meta Quest 3 VR headset. 
The project utilizes Unity 2022.3.43f1 and leverages the Meta Building Blocks, Meta Depth API, 
and Mixed-Reality SDK to create an immersive experience that maps the user's environment in real time.

## Features
1. Room Mapping with Depth Textures
  + **Depth Texture Integration:** The project accesses depth textures from the Meta Quest 3 camera, allowing it to analyze the linear depth of the scene. This data is used to identify points in front of the user.
  + **3D Cube Mapping:** Thousands of cubes are spawned in the scene to represent the room's geometry in real time, creating a visual map of the user's surroundings.
  + ** Mesh Generation:** With the click of a button, the application generates a mesh that represents the room based on the captured depth data. This mesh provides a detailed model of the user's environment.

2. Performance Optimization
  + **Point Filtering:** A feature that scans the room and removes all points that aren't within a predefined space (a cube within the scene) to enhance performance.
  + **Optimized Mesh Generation:** Work is ongoing to improve the mesh generation process by only including points that remain within the specified cube after filtering.
3. Work in Progress
  + **Advanced Mesh Generation:** An in-progress feature focuses on generating a more optimized mesh by using only the points that are inside the designated cube. This aims to further improve performance and provide a more accurate room model.

## Usage
  + **Mesh Generation**
    ++ **Mesh Room Mapping:** Press the 'A' button to spawn a mesh of the room
    ++ **(WIP) Mesh Inside Box:** Press the 'B' button to spawn a mesh inside the box
  + **Cube Generation**
    ++ **Cube Room Mapping:** Press the 'X' Button to spawn cubes to map the room
    ++ **Cubes Inside Box:** Press the 'Y'  button to spawn cubes inside of the box
