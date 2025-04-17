# System Overview: Design of an AR-HMD Interface for Interactive Control of Robotic Tack and Seam Welding

## 1. Project Purpose

This project explores the integration of Augmented Reality (AR) and computational workflows to support novice users in programming and establishing robotic welding paths. It aims to lower the entry barrier for users lacking prior experience with robotic systems or welding automation, by providing intuitive, visual, and interactive guidance through AR head-mounted displays (HMDs).

By combining AR’s spatial visualization capabilities with a backend parametric computational framework, the system enables users to define, simulate, and refine welding paths directly within the physical context of the workpiece.
  
This approach seeks to:
- Streamline the welding setup process,
- Reduce programming errors,
- Enhance user understanding and confidence in robotic operations.

---

## 2. System Architecture

The system is structured around two interconnected environments:

**Virtual Environment**:  
A parametric model-driven environment designed in Grasshopper for Rhino 3D, containing robot paths, welding simulation trajectories, and error visualization overlays.

**Physical Environment**:  
The real-world setup consisting of a Universal Robot UR10 CB-Series manipulator, a custom metal workpiece, and spatial anchoring through visual markers.

---

## 3. Software Components

The system uses the following software stack:

| Software               | Purpose | Notes |
|-------------------------|---------|-------|
| Rhino 7 | 3D environment modeling and visual marker layout | Required |
| Grasshopper for Rhino | Parametric design control and robot trajectory planning | Required |
| [Robot Plugin for Grasshopper](https://github.com/visose/Robots) | Communication between Grasshopper and UR robots | Required |
| [Fologram](https://fologram.com/download) | 
| [Generation Plugin](https://www.food4rhino.com/en/app/generation?lang=en) |

---

## 4. Hardware Requirements

| Component                 | Specification |
|----------------------------|----------------|
| AR Head-Mounted Display    | Microsoft HoloLens 2 |
| Collaborative Robot (Cobot) | Universal Robot UR10 CB-Series |
| Tracking Markers           | Custom printed markers for Fologram tracking |
| End Effector               | Customized end effectors using Millibar or Soldamatic components |
| Computer Workstation       | Intel i7 (8th Gen or better), 16GB RAM, GTX 1070+ GPU, Windows 10/11 |

Additional physical components include customized metal workpieces for realistic welding path demonstrations.

---

## 5. Key Features

- **Parametric Design Control**:  
  Users can dynamically adjust robot waypoints and visualize welding trajectories in real time using Grasshopper.
  
- **AR Visualization for Novice Guidance**:  
  Real-time AR overlays provide an intuitive visualization of robot movement, welding paths, and potential safety violations.
  
- **Seamless Robotic Integration**:  
  Direct linkage between the Grasshopper environment and UR10 robot via the Robot plugin enables quick transmission of robot programs.
  
- **Spatial Anchoring via Visual Markers**:  
  Accurate spatial synchronization is achieved using Fologram’s marker-based tracking system.

---

## 6. Repository Structure

| Folder/File                   | Description |
|--------------------------------|-------------|
| `GrasshopperFiles/`            | Grasshopper (.gh) scripts for parametric modeling and robot path definition |
| `RhinoFiles/`                  | Rhino (.3dm) files defining the spatial layout and visual marker configuration |
| `Assets/`                      | High-resolution images, video demonstrations, and supplementary visuals |
| `Docs/`                        | Additional documentation for installation, setup, and troubleshooting |
| `Submission/`                  | Full-resolution version of the poster, photographs, and illustrations used for ISMAR 2025 submission |

For a quick overview of repository contents, refer to the [README.md](./README.md).

---

## 7. Installation and Setup Instructions

### 7.1 Software Installation
- Install Rhino 7 and ensure Grasshopper is available.
- Install Robot Plugin for Grasshopper.
- Install Fologram for Rhino.
- (Optional) Install Generation plugin for enhanced parametric workflows.

### 7.2 Hardware Setup
- Mount tracking markers around the physical workspace.
- Calibrate AR-HMD to recognize the markers.
- Position the UR10 robot with the customized end effector aligned to the physical metal workpiece.

### 7.3 Running the System
1. Open the Rhino workcell file (`RhinoFiles/robot_workcell.3dm`).
2. Open the Grasshopper parametric model (`GrasshopperFiles/robot_welding_trajectory.gh`).
3. Activate Fologram live streaming to the HoloLens.
4. Visualize the virtual robot and welding paths through the HoloLens.
5. Adjust parameters in Grasshopper to modify waypoints, trajectories, and welding sequence.
6. Send finalized programs to the UR10 robot via the Robot plugin.

---

## 8. Demonstration Videos

Available under the `Assets/` folder:

| Video File | Description |
|------------|-------------|
| `system_overview.mp4` | Overall system workflow from modeling to AR visualization |
| `marker_alignment_demo.mp4` | Visual marker tracking and spatial anchoring process |
| `prototype_interaction_demo.mp4` | Interaction with AR overlays to modify robot paths |

---

## Safety Notice

> ⚠️ **Warning**:  
> Operation of collaborative robots and AR-HMDs requires appropriate training.  
> Ensure supervision by a qualified advisor or robotics professional.  
> The repository contributor is not liable for any damage, injury, or misuse.

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
