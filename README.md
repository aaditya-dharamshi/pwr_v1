# pwr_v1
Main powerboard (first version) PCB files.

This was the first major board designed for SeeGoals, a project under FIA Robotics at Linkoping University, Sweden. I designed the complete PCB (assisted by other teammates who have developed the foundation), and the design files are shared here with permission from LiU SeeGoals.

This was the prototype for the main power distribution and interface board for the robot, powered by a 23.8V LiPo battery. This board is designed with KiCAD 8, and this repository contains the KiCAD project files and related documents.

# Documentations
📄 [Schematic PDF](Docs%20and%20Images/pwr_v1_schematic.pdf)
📄 [Layout PDF ](Docs%20and%20Images/pwr_v1_CopperLayers.pdf)

# 3D renders
Top view
![Top Layer](Docs%20and%20Images/3dViews/pwr_v1_3dT1.png)
Bottom view
![Bottom Layer](Docs%20and%20Images/3dViews/pwr_v1_3dB1.png)


Main features:
- 3.3V, 5V and 12V buck converters
- IMU on board
- Interfaces for STM32 Nucleo, nRF board and kicker board.

Stackup: 
- 4-layer FR4 PCB with 1.6mm thickness
- Copper thickness: 2 oz outer layer and 1 oz inner layers.

Design considerations:
- High-current power distribution from the LiPo battery.
- Dedicated power and signal layers.
- 4-layered stackup for improved grounding and power integrity.
- Decoupling capacitors placed carefully near the components.
- SMD-type connectors used for STM32 Nucleo interface, reducing thru hole pins and enabling better power and ground plane integrity.

Validation	
- This board was fabricated, assembled and integrated into the robot.
- During validation, issues related to nRF connector pin mapping, connector selection and mechanical design perspectivewere identified, which were addressed in the second revision.
