# Design of an AR-HMD Interface for Interactive Control of Robotic Tack and Seam Welding (Supplemental Document)

## Overview
This project explores the integration of Augmented Reality (AR) and computational workflows to support novice users in programming and establishing robot welding paths. The aim is to lower the entry barrier for users who lack prior experience with robotic systems or welding automation by providing intuitive, visual, and interactive guidance through AR interfaces. By combining AR’s spatial visualization capabilities with a backend computational framework, the system enables users to define, simulate, and refine welding paths directly within the physical context of the workpiece. This approach seeks to streamline the welding setup process, reduce errors, and enhance user understanding and confidence in robotic operations.

<p align="center">
  <img src="https://github.com/LoyWeiWin/Pub_ISMAR_SupplementalDocument_DesignofanARHMDInterfaceforInteractiveControlofRoboticTackandSeamWeld/blob/ef99aa30721b453bffd0c857b2cd5e39fd112f61/Assets/Images/GitHub-Fig-01.jpg?raw=true" alt="Figure 01: AR-supported Robotic Welding Setup" width="600"><br>
  <em>Figure 01: AR-supported robotic welding setup illustrating the use of a head-mounted display (HMD) to guide novice users in defining and verifying welding paths in real-time.(A) Workstation (B) Microsoft HoloLens 2 (C) Visual Marker for spatial anchroing (D) Virtual Overlay of the Cobot and End Effector (E) Control Box (F) Metal Workpiece </em>
</p>

## Software Requirement
- Rhino 7 or latest
- [Robot plugin](https://github.com/visose/Robots)
- [Fologram](https://fologram.com/download)
- [Generation](https://www.food4rhino.com/en/app/generation?lang=en)

## Key Features
- **Parametric Design Control**: Use Grasshopper to dynamically adjust sketching pattern (bychanging reference image).
- **Compatibility with Universal Robot**: Seamless integration with UR collaborative robots for industrial applications.

## Repository Structure
- `GrasshopperFiles/`: Grasshopper scripts.
- `RhinoFiles/`: Robot workcell, and end-effectors.
- `Assets/`: Images, thumbnails and videos
- `Docs/`: Documentation for installation, and troubleshooting.

## Contributing
Contributions to improve this workflow are welcome! Please follow the contributing guidelines in the [contributing guidelines](https://github.com/LoyWeiWin/TemplateRepo/wiki/06_Contributing-Guidelines) in wiki.

## Code of Conduct
This project follows the Contributor Covenant Code of Conduct. Please read our [Code of Conduct](https://github.com/LoyWeiWin/TemplateRepo/blob/main/CODE_OF_CONDUCT.md) before contributing.

> [!WARNING]  
> If you are unfamiliar with using [XYZ], please ensure you have supervision from a qualified advisor or professional.
> The contributor or owner of this repository is not responsible for any physical damage, injury, or harm caused to the immediate environment or individuals due to improper usage of cobots or related tools.

## Acknowledgements
This project was independently developed as part of my personal initiative and commitment to advancing this field.

## References
1. [APA 7th Edition]




