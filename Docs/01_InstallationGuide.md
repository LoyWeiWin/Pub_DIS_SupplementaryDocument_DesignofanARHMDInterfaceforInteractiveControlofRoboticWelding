# Installation Guide

This document provides setup instructions for the AR-HMD Interface for Interactive Control of Robotic Tack and Seam Welding.

---

## Table of Contents
- [Getting Started](#getting-started)
- [Software Requirements](#software-requirements)
- [Connecting to the Robot](#connecting-to-the-robot)

---

## Getting Started

Before beginning, ensure you have administrative access to your system and are able to install plugins and configure your network settings.

---

## Software Requirements

1. **Install Rhino 7**  
   Download a trial or full version from the [Rhino website](https://www.rhino3d.com/download/).

2. **Install the Robots Plugin for Grasshopper**  
   - Open Rhino and run the `_PackageManager` command.
   - Search for `Robots` and install the plugin.
   - Restart Rhino and open Grasshopper.
   - A new **Robots** tab should appear.
   - Click the `Libraries` button on a `Load robot system` component to install a robot library.
   - Robot models from the library will populate a value list connected to the `Load robot system`.

> **Recommended:** For a helpful walkthrough, see [this YouTube playlist](https://www.youtube.com/watch?v=vAe47zN-d48&list=PLqtxhH1qb3Mw5A_YbvHDfrq4DNNfLtcW-) by [@robin-gdwl](https://github.com/robin-gdwl).

3. **Install the Generation Plugin**  
   - Download the plugin from [Food4Rhino](https://www.food4rhino.com/en/app/generation).
   - Right-click the downloaded `.zip` file → **Properties** → check **Unblock** if available.
   - Unzip the file.
   - Drag the plugin contents onto the Grasshopper canvas to complete installation.

---

## Connecting to the Robot

> ⚠️ Begin by powering on and starting the Universal Robot (UR10 CB-Series).

1. **Connect the Ethernet Cable**  
   Plug one end into your computer and the other into the robot's control box.

2. **Configure Static IP Address**  
   Set a [static IP address](https://pureinfotech.com/set-static-ip-address-windows-10/) for your computer on the same subnet as the robot.

   - You can [find the robot's IP address here](https://robodk.com/doc/en/Robots-Universal-Robots.html#UR-IP).

3. **Verify Connectivity with Ping Test**  
   - Open Command Prompt (Windows) or Terminal (macOS/Linux).
   - Type: `ping [robot_ip_address]`
   - A successful reply means the robot is reachable.

   > ❗ **Firewall Warning (Windows Users):**  
   > If ping fails, your firewall may be blocking ICMP requests.  
   > Refer to [this guide](https://windowsreport.com/windows-10-unable-to-ping-other-computers/) for help.

4. **Ready to Send Programs**  
   Once you receive ping replies, the connection is active. You are now ready to transmit robot programs using the Robot plugin in Grasshopper.

---

## Next Steps

Once the system is installed and connected, refer to the [`02_UsageInstructions.md`](./UsageInstructions.md) for details on running tack and seam welding operations using the AR interface.

