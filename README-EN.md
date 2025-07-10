> [!NOTE]
> Đây là bản README tiếng Anh. Vui lòng đọc bản tiếng Việt tại [đây](README.md).

<div align="center" class="grid cards" style="display: flex; align-items: center; justify-content: center; text-decoration: none;" markdown>
    <img src="assets/App/AstrocelerateLogo-Branded.png" alt="Logo" width="75%">
    <p>Copyright © 2024-2025 <a href="https://www.linkedin.com/in/minhduong-thechosenone/">Dương Duy Nhật Minh</a>, D.B.A. <b>Oriviet Aerospace</b>. All Rights Reserved.</p>
    </br>
</div>


This is the public-facing repository of Astrocelerate, Vietnam's first ever orbital mechanics and spaceflight simulation engine, built to deliver sovereign aerospace capability through high-fidelity physics, Vulkan rendering, and modular C++ extensibility.
For more detailed information about the project's goals, features, and design philosophy, please refer to this README.

> [!NOTE]
> The full source code for Astrocelerate is currently maintained in a private repository to protect intellectual property for academic purposes.
> However, you can still view Astrocelerate's progress in the [Screenshots](#screenshots) section.

---

# Table of Contents
* [About Astrocelerate](#about-astrocelerate)
    * [Goal](#goal)
    * [Vision](#vision)
        * [Short-term vision (MVP)](#short-term-vision-mvp)
    * [Design philosophy](#design-philosophy)
* [Features](#features)
    * [Currently implemented](#currently-implemented)
    * [Near-future plans](#near-future-plans)
* [Installation](#installation)
    * [Prerequisites](#prerequisites)
    * [Bootstrapping](#bootstrapping)
* [History](#history)
    * [Screenshots](#screenshots)

---

# About Astrocelerate
Astrocelerate is Vietnam’s first high-performance orbital mechanics and spaceflight simulation engine, designed from the ground up to serve as a sovereign alternative to foreign aerospace software.

## Goal
Developed in C++ with a Vulkan-based graphics pipeline and custom ECS architecture, Astrocelerate is engineered for real-time, physically accurate visualizations of satellite kinematics, launch trajectories, and maneuver simulations. But beyond technical performance, Astrocelerate stands for something far greater:

>The assertion that world-class aerospace tools can emerge from within Vietnam, built not by legacy contractors, but by a new generation of engineers who refuse to wait for permission.

Its mission is to empower academic institutions, disaster-response planners, space technologists, and national defense researchers with a transparent, extensible, and self-owned simulation platform. But more than that, it represents technological sovereignty in a domain long dominated by external systems.

Powered by Oriviet Aerospace. Grounded in Vietnam. Engineered for the stars.

## Vision
### Short-term vision (MVP)
The short term vision of Astrocelerate is to create a Minimum-Viable Product (MVP) that satisfies core features. Specifically, the MVP must be able to achieve these minima:
- Accurate real-time and interactive visualizations demonstrating simple scenarios (e.g., Earth-satellite orbit, basic maneuver simulation, the "launch, enter orbit, stage separation, re-entry, recovery" sequence)
- A clean, polished user interface
- An Entity-Component-System (ECS)-based design

## Design philosophy
Astrocelerate's design philosophy takes inspiration from that of the Unity game engine and the GMAT spaceflight simulation engine.
These principles are subject to change over time, as Astrocelerate (and I) become more mature.

|              Core design principles              | Description                                                                                                                                                                                                                                                                                                                                                                                                                    |
| :----------------------------------------------: | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
|         **Open-source**          | Astrocelerate aims to be transparent and thrives on community feedback, modification, and extension. Therefore, to maximize contribution and growth, it is decided that the engine should be open-source.                                                                                                                                                              |
| **ECS-based, Modular & Extensible Architecture** | Astrocelerate is structured to allow flexibility and modularity, allowing users to set up and develop their own environments, objects, gravity, etc. with built-in, third-party, and custom "modules". This is part of Astrocelerate's integration of Entity-Component-System principles.<br><br>Astrocelerate is built to allow third-party plug-ins and extensions, enabling researchers to integrate new models or solvers. |
|      **Non-proprietary scripting language**      | Astrocelerate allows users to program their own modules and override built-in counterparts with C++.                                                                                                                                                                                                                                                                                                                           |
|          **Support for real missions**           | Astrocelerate can be used for operational mission planning (e.g., lunar and interplanetary transfers, spacecraft launch-and-recovery procedures).                                                                                                                                                                                                                                                                              |


# Features
## Currently implemented
- Real-time orbital propagation
- Accurate 2-body simulation
- Configurable physics time step
- Reference frame system with fixed simulation scaling (maintains physical accuracy across polarized scales)
- Custom ECS-based architecture with sparse-set storage (allows for performant simulation and efficient data flow between the GUI and backend)
- Live telemetry data, console, etc.; Tweakable simulation settings
- Offscreen rendering (allows for custom viewports, post-processing, etc.)

## Near-future plans
- Swappable numerical integrators (Symplectic Euler, RK4)
- Data-caching in ECS for even more performance
- Compute shaders and the offloading of parallelizable processes to the GPU
- Dynamic scaling for seamless transitions (e.g., from terrain to planet)
- N-body simulation capabilities
- A more diverse range of numerical integration methods (Verlet, Simpson's Rule, Gaussian quadrature)
- Solvers, coordinate systems, epochs
- C++ scripting to allow for user-created simulations
- Serialization of GUI and simulation data, with basic exporting capabilities
- A more advanced model loader, with better, correctly mapped textures and visual fidelity


# Installation
> [!WARNING]
> Astrocelerate has only been tested on Windows, although the application aims to be cross-platform-compatible.

## Prerequisites
- Vulkan SDK (Vulkan 1.2+)
- Vcpkg dependency manager
- CMake 3.20+
- Python 3.9+
- C++20

## Bootstrapping
Configuring and running Astrocelerate is currently unavailable: The prerequisite bootstrapping scripts are currently limited to the private repository. 


# History
Astrocelerate made its first commit on November 28th, 2024. As of July 10th, 2025, it has been in development for 7 months:
- Legacy engine (OpenGL): 2 months
- Current engine (Vulkan): 5 months

## Screenshots
The following screenshots document the development of Astrocelerate.

### July 10th, 2025
![2025-07-10](https://github.com/user-attachments/assets/f86a19d1-0204-4aa8-9122-41ffcf0d268c)

### July 3rd, 2025
![2025-07-03](https://github.com/user-attachments/assets/60805ea1-2385-41f6-97dd-79cd571188f0)

### June 21st - 22nd, 2025
![2025-06-22](https://github.com/user-attachments/assets/2c5361d0-848e-479e-b3eb-a0c578d079ee)
![2025-06-21](https://github.com/user-attachments/assets/7c4e388d-0296-4222-aa37-aa3e346985ca)

### June 8th, 2025
![2025-06-08](https://github.com/user-attachments/assets/8b4ba3e0-a3b3-4434-83dc-818e1e4f1828)

### June 3rd, 2025
![2025-06-03](https://github.com/user-attachments/assets/7757061d-c7f4-4e8a-9faf-d0fd595bcec1)
![2025-06-03](https://github.com/user-attachments/assets/b9d7e9eb-0035-405f-bc4d-deff89e718b8)

### May 20th - 21st, 2025
![2025-05-21](https://github.com/user-attachments/assets/190a28e6-0b11-4355-bdf6-54978e707660)
![2025-05-20](https://github.com/user-attachments/assets/23634f9f-067f-4235-a932-015feccdfa0b)

### May 16th, 2025
![2025-05-16](https://github.com/user-attachments/assets/f5c2d98c-7b1b-4b93-a833-b132181dd948)

### May 14th, 2025
![2025-05-14](https://github.com/user-attachments/assets/22cfff2a-6a79-4b6f-a889-0931ed3235ec)

### May 4th, 2025
![2025-05-04](https://github.com/user-attachments/assets/ef1fa152-f5c0-4e16-a6a5-40a53180fe14)

### April 1st, 2025
![2025-04-01](https://github.com/user-attachments/assets/f7368b9e-8606-4182-a882-192753768ba5)

### March 17th, 2025
![2025-03-17](https://github.com/user-attachments/assets/19f4eb20-e56b-4275-b877-eb5a6e027f51)

### December 9th, 2024 (Legacy Astrocelerate)
![2024-12-09](https://github.com/user-attachments/assets/419ba7f0-8b80-4663-bb30-a6815ffc8af4)
