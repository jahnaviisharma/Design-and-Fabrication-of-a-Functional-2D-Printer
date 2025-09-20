# Design-and-Fabrication-of-a-Functional-2D-Printer
# 🖨️ 2D Printer — Design Lab Course Project
**Course Instructors:** Dr. Prabhat Agnihotri, Dr. Manish Agrawal, Dr. Satwinder Jit Singh  
 *Jan 25 – May 25*  

---

##  Overview
This project was developed as part of the **Design Lab Course**. The objective was to design and build a **fully functional 2D printer from scratch**, covering every stage from **mechanical design** and **electronics integration** to **firmware programming** and **motion control**.

The system is capable of interpreting **G-code instructions** to coordinate XY-axis motion, enabling precise drawing, plotting, or additive manufacturing tasks.

---

- **Mechanical Design**
  - Designed the XY-axis frame and carriage system using aluminum extrusions and 3D-printed joints.  
  - Selected appropriate belt, pulley, and bearing systems for smooth motion.  
  - Developed a lightweight tool mount (pen/marker holder) for 2D plotting tasks.  

- **Electronics & Circuit Integration**
  - Wired and configured **NEMA 17 stepper motors** with **A4988 drivers** and **Arduino Uno**.  
  - Chose power supply specifications to ensure reliable motor performance.  
  - Debugged wiring and stepper driver current settings for stable motion.  

- **Firmware Development**
  - Wrote Arduino firmware (`printer_firmware.ino`) using **AccelStepper library**.  
  - Implemented parsing of **G0/G1 commands** to control XY movement.  
  - Calibrated **steps-per-mm** values for accurate motion.  
  - Added basic **homing (G28)** routine for zeroing the system.  

- **Host Software**
  - Developed a Python script (`send_gcode.py`) to transmit `.gcode` files via serial.  
  - Implemented simple flow control to ensure Arduino processed commands correctly.  

- **Testing & Validation**
  - Ran multiple **test paths** (square, circle, text outlines) to validate coordinated XY motion.  
  - Fine-tuned feedrates and accelerations to reduce vibrations and improve accuracy.  
  - Documented build process, results, and challenges for future reference.  

---

##  Features of the System
- Custom-designed XY-axis motion system  
- Stepper motor control with microstepping support  
- G-code parser for linear motion (G0/G1)  
- Host-side G-code sender tool for PC-Arduino communication  
- Modular hardware design — easily extendable to CNC or 3D printing applications  

---

##  Hardware Setup
- **Motors:** 2 × NEMA 17 stepper motors  
- **Drivers:** A4988 / DRV8825 (microstepping enabled)  
- **Controller:** Arduino Uno  
- **Power Supply:** 12 V / 3 A DC  
- **Motion System:** GT2 belts & pulleys + linear bearings  
- **Frame:** Aluminum extrusion + custom 3D-printed parts  
- **Toolhead:** Pen mount for 2D plotting (expandable to extruder for 3D printing)  


