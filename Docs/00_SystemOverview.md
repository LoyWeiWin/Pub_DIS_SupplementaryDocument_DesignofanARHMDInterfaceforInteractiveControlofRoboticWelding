# System Overview

## Project Purpose

This project explores the integration of Augmented Reality (AR) and computational workflows to support novice users in programming and establishing robotic welding paths. It aims to lower the entry barrier for users lacking prior experience with robotic systems or welding automation, by providing intuitive, visual, and interactive guidance through AR head-mounted displays (HMDs).

By combining AR’s spatial visualization capabilities with a backend parametric computational framework, the system enables users to define, simulate, and refine welding paths directly within the physical context of the workpiece.
  
This approach seeks to:
- Streamline the welding setup process,
- Reduce programming errors,
- Enhance user understanding and confidence in robotic operations.

---

## System Architecture

The system is structured around two interconnected environments:

**Virtual Environment**:  
A parametric model-driven environment designed in Grasshopper for Rhino 3D, containing robot paths, welding simulation trajectories, and error visualization overlays.

**Physical Environment**:  
The real-world setup consisting of a Universal Robot UR10 CB-Series manipulator, a custom metal workpiece, and spatial anchoring through visual markers.

---

## Software Components

The system uses the following software stack:

| Software               | Purpose | Notes |
|-------------------------|---------|-------|
| Rhino 7 | 3D environment modeling and visual marker layout | Required |
| Grasshopper for Rhino | Parametric design control and robot trajectory planning | Required |
| [Robot Plugin for Grasshopper](https://github.com/visose/Robots) | Required |
| [Fologram](https://fologram.com/download) | Required |
| [Generation Plugin](https://www.food4rhino.com/en/app/generation?lang=en) | Required |

---

## Hardware Requirements

| Component                 | Specification |
|----------------------------|----------------|
| AR Head-Mounted Display    | Microsoft HoloLens 2 |
| Collaborative Robot (Cobot) | Universal Robot UR10 CB-Series |
| Tracking Markers           | Custom printed markers for Fologram tracking |
| End Effector               | Customized end effectors using Millibar or Soldamatic components |
| Computer Workstation       | Intel i7 (8th Gen or better), 16GB RAM, GTX 1070+ GPU, Windows 10/11 |

Additional physical components include customized metal workpieces for realistic welding path demonstrations.

---

## Key Features

- **Parametric Design Control**:  
  Users can dynamically adjust robot waypoints and visualize welding trajectories in real time using Grasshopper.
  
- **AR Visualization for Novice Guidance**:  
  Real-time AR overlays provide an intuitive visualization of robot movement, welding paths, and potential safety violations.
  
- **Seamless Robotic Integration**:  
  Direct linkage between the Grasshopper environment and UR10 robot via the Robot plugin enables quick transmission of robot programs.
  
- **Spatial Anchoring via Visual Markers**:  
  Accurate spatial synchronization is achieved using Fologram’s marker-based tracking system.

---

## Contact

For questions, technical support, or collaboration inquiries, please contact:

**Wei Win Loy**  
**Email**: loyweiwin@gmail.com

---

## Acknowledgements

This project was independently developed by Wei Win Loy as part of an ongoing initiative to advance intuitive human-robot interaction in manufacturing applications.

Special thanks to the open-source developers of Fologram, the Robot Plugin, and the Rhino/Grasshopper community.

---
