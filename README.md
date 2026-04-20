# CS 330: Computational Graphics and Visualization - Final Project

**Author:** LukasCS (Lukas Brkovic Leighton)  
**Course:** CS-330 at Southern New Hampshire University  
**Date:** April 2026  

## Project Overview

This repository contains my final project for **CS-330 Computational Graphics and Visualization**. The 3D scene recreates a modern computer workstation/desk setup, including:

- A wooden desk with four tapered legs
- A monitor with metal frame, bezel, and lit screen
- Monitor stand (base + neck)
- Keyboard and mouse
- Floor and back wall with textures

The scene features **Phong lighting** (multiple colored lights with ambient, diffuse, and specular components), **texture mapping**, and **custom materials** for realistic shading on wood and metal surfaces.

**Key technical features:**
- Built in C++ with **OpenGL**, **GLFW**, **GLEW**, and **GLM**
- Dynamic camera navigation (WASD + QE movement, mouse look, scroll for speed, P/O for perspective/orthographic toggle)
- Multiple light sources for depth and realism
- Reusable meshes (box, cylinder, tapered cylinder, plane, sphere/half-sphere)

### Files Included
- `7-1_FinalProjectMilestones.zip` — Complete Visual Studio project with source code, shaders, textures, and executable
- Design Decisions document (if separate; otherwise referenced in this README)
- All source files, shaders, and textures are inside the ZIP

You can run the `7-1_FinalProjectMilestones.exe` (Release build) on a Windows machine with compatible graphics drivers.

---

## Reflection: Module Eight Journal

### How do I approach designing software?

I approach software design by first breaking the problem into smaller, manageable components. For this 3D scene, I started by analyzing the reference image (my desk setup) and decomposing complex objects into basic primitives (boxes, cylinders, planes, etc.). I then planned the scene hierarchy, materials, lighting, and user interaction before writing any code.

**New design skills gained:**
- Modular scene management (separating `SceneManager`, `ViewManager`, and `ShaderManager`)
- Using transformation matrices systematically for positioning, scaling, and rotating objects
- Designing material and lighting systems that work together with the Phong reflection model

**Design process followed:**
1. Reference image analysis → identify shapes and materials
2. Define reusable meshes and textures
3. Implement lighting and materials
4. Add camera controls and iteration/testing

This structured approach (decomposition + iteration) can be applied to any future graphics, game development, or simulation projects.

### How do I approach developing programs?

I treat development as an iterative process: build a minimal version, test frequently, then enhance with new features (textures → lighting → materials → polish).

**New development strategies used:**
- Working with external libraries (GLFW for window/input, GLEW for OpenGL extensions, GLM for math)
- Shader-based rendering pipeline (vertex + fragment shaders with uniforms for transformations, lighting, and materials)
- Texture loading with **stb_image** and proper mipmapping
- Managing multiple light sources and per-object materials in a single render loop

**How iteration factored in:**
Each milestone added a layer:
- Early milestones: basic shapes and camera
- Mid milestones: textures and transformations
- Final project: full Phong lighting, custom materials, multiple lights, and scene polish

My approach evolved significantly. I started with trial-and-error placement of objects. By the end, I was confidently using vector math, matrix transformations, and shader uniforms to achieve precise, reusable results. Debugging became faster once I learned to isolate one object/light at a time.

### How can computer science help me in reaching my goals?

Computational graphics and visualizations gave me hands-on experience with low-level rendering pipelines, linear algebra in practice (matrices, vectors, transformations), and real-time 3D programming. These skills directly strengthen my understanding of computer science fundamentals.

**Future educational pathway:**
These concepts will help in advanced courses involving game engines, computer vision, simulation, or any graphics-related electives. The experience with OpenGL provides a strong foundation for learning Vulkan, Unity, or Unreal Engine.

**Future professional pathway:**
In my career, these skills open doors to roles in game development, VR/AR, data visualization, 3D modeling for engineering/architecture, or even UI/UX with 3D elements. Understanding how light, materials, and camera systems work together helps me create more engaging and realistic digital experiences. Even outside pure graphics, the problem-solving, performance optimization, and modular design practices apply to general software engineering.

Overall, this project was challenging but extremely rewarding. It transformed abstract math and theory into a visually impressive, interactive 3D world I can be proud of.

---

## How to Run the Project

1. Download and extract `7-1_FinalProjectMilestones.zip`
2. Navigate to the `Release` folder
3. Run `7-1_FinalProjectMilestones.exe`
4. Controls:
   - **Mouse** → Look around (cursor is hidden)
   - **WASD** → Move forward/back/left/right
   - **QE** → Move up/down
   - **Scroll Wheel** → Adjust movement speed
   - **P** → Perspective projection
   - **O** → Orthographic projection
   - **ESC** → Exit

Enjoy exploring the desk scene!

If you have any questions or feedback, feel free to reach out.

**Thank you for reviewing my portfolio artifact!**
