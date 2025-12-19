# Augmented Reality Interface for Direct Robotic Welding Path Programming  - Supplementary Documents

This repository provides supplemental materials for the long paper titled "Augmented Reality Interface for Direct Robotic Welding Path Programming," presented at the DIS, 2026.

## Overview

Programming robotic welding tasks remains challenging for non-experts due to the complexity of conventional teach-pendant and CAD-based methods. This paper explores how Augmented Reality (AR) can support direct, spatially contextualised path definition for robotic welding. Unlike prior AR-assisted HRI studies that emphasise seam welding through Programming-through-Demonstration (PtD), this work investigates the potential of AR integrated with computational design tools in the underexplored domain of tack welding, where discrete spatial judgement and segmentation are required. We developed an AR interface that enables users to specify both seam and tack welding paths through gesture-based spatial input, while receiving in-situ, real-time reachability feedback derived from the robot’s inverse kinematics model. Following a Research-through-Design (RtD) approach, the system was iteratively refined through internal technical validation and structured reflective analysis, rather than empirical user evaluation, focusing on feedback clarity, task interaction, and the perception of robotic constraints. Our study contributes (1) an AR-assisted path planning workflow that integrates tack and seam welding within a unified spatial interface, (2) design knowledge derived from reflective system development on how computational feedback can mediate embodied human-robot negotiation, and (3) a conceptual framing that showcases AR as a reflective medium that transforms robotic programming into a situated, reflective activity.¬

<p>
  <img src="https://github.com/LoyWeiWin/Pub_ISMAR_SupplementalDocument_DesignofanARHMDInterfaceforInteractiveControlofRoboticTackandSeamWeld/blob/ef99aa30721b453bffd0c857b2cd5e39fd112f61/Assets/Images/GitHub-Fig-01.jpg?raw=true" alt="Figure 01: AR-supported Robotic Welding Setup" width="600"><br>
  <em>Figure 01: AR-supported robotic welding setup illustrating the use of a head-mounted display (HMD) to guide novice users in defining and verifying welding paths in real-time. (A) Workstation (B) Microsoft HoloLens 2 (C) Visual Marker for spatial anchoring (D) Virtual Overlay of the Cobot and End Effector (E) Control Box (F) Metal Workpiece </em>
</p>

## Software Requirements
- Rhino 7 or later
- [Robot plugin](https://github.com/visose/Robots)
- [Fologram](https://fologram.com/download)
- [Generation](https://www.food4rhino.com/en/app/generation?lang=en)

## Hardware Requirements
- Universal Robot, UR10 CB-Series
- Microsoft HoloLens (AR-HMD)
- Customised metal workpieces
- Customised end effector ([Millibar](https://millibar.com/manual-tool-changer/), [Soldamatic](https://seaberyat.com/en/soldamatic/), customised connection)

## Key Features
**Parametric Design Control**: Use Grasshopper to dynamically adjust robot waypoints, visualise robot trajectories, transmit robot commands, and visualise potential robotic errors.

**Compatibility with Universal Robot**: Seamless integration with UR collaborative robots for robotic welding (both tack and seam welding).

## Repository Structure
- `GrasshopperFiles/`: Grasshopper scripts.
- `RhinoFiles/`: Robot workcell and marker setups.
- `Assets/`: Images, thumbnails, and video demonstrations.
- `Docs/`: Documentation for installation and troubleshooting.
- `Submission/`: Full-resolution photographs, illustrations, and full poster submission.

## Contributing

This repository is intended to share supplemental materials related to the poster.  
Currently, external contributions are not accepted.

For any queries, please contact loyweiwin@gmail.com.


> [!WARNING]  
> If you are unfamiliar with using cobots such as the UR10 and AR-HMD systems, ensure supervision by a qualified advisor or professional. The contributor or owner of this repository is not responsible for any physical damage, injury, or harm caused to individuals or the environment due to improper usage of cobots or related tools.

## License

This repository is licensed under the Custom Academic License v1.0 (2025).

See the [LICENSE](./LICENSE) file for full terms.

## Acknowledgements
This project was independently developed as part of my personal initiative and commitment to advancing this field. This research was conducted at Advanced Robotic for Manufacturing Hub (ARMHub). 

## References
[1] J. Gwyllim, N. Cam, and N. van der Bruggen, "Fologram for Grasshopper," Fologram, 2025. [Online]. Available: https://fologram.com/

[2] Y.-S. Kim, C.-H. Lee, and Y.-K. Kim, "Effect of heat input on microstructure and mechanical properties of austenitic stainless steel welds," Materials Science and Engineering: A, vol. 396, pp. 1–9, 2005. doi: 10.1016/j.msea.2004.11.063

[3] G. Liu, W. Sun, and P. Li, "Motion capture and AR-based programming by demonstration for industrial robots using handheld teaching device," Scientific Reports, vol. 14, no. 1, p. 23259, 2024. doi: 10.1038/s41598-024-73747-4

[4] F. Mueller, C. Deuerlein, and M. Koch, "Intuitive welding robot programming via motion capture and augmented reality," IFAC-PapersOnLine, vol. 52, no. 10, pp. 294–299, 2019. doi: 10.1016/j.ifacol.2019.10.045

[5] D. Ni, A. W. W. Yew, S. K. Ong, and A. Y. C. Nee, "Haptic and visual augmented reality interface for programming welding robots," Advances in Manufacturing, vol. 5, no. 3, pp. 191–198, 2017. doi: 10.1007/s40436-017-0184-7

[6] S. K. Ong, A. Y. C. Nee, A. W. W. Yew, and N. K. Thanigaivel, "AR-assisted robot welding programming," Advances in Manufacturing, vol. 8, no. 1, pp. 40–48, 2020. doi: 10.1007/s40436-019-00283-0

[7] D. Rutten, "Grasshopper – Algorithmic Modeling for Rhino," Grasshopper3D. [Online]. Available: https://www.grasshopper3d.com/
