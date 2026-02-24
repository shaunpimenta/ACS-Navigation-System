# Autonomous Navigation System  
### SAE International AeroDesign Competition 2022

This repository documents the autonomous navigation system I developed as part of the **SAE International AeroDesign Competition 2022**.

The system enabled autonomous target detection and navigation for our unmanned aircraft, including high-altitude visual detection of a designated landing zone and real-time decision-making during flight.

This project represents a full-cycle engineering effort — from aircraft construction to perception algorithms and flight integration.

---

# 🏆 Competition Context

SAE AeroDesign challenges university teams to design, build, and fly a mission-capable aircraft under strict performance constraints.

For the 2022 competition, we designed and built a fixed-wing UAV and integrated a custom autonomous navigation subsystem capable of:

- Detecting a colored landing zone from over **200 feet**
- Computing directional corrections
- Assisting in mission alignment and landing

This repository serves as a **technical portfolio of my contributions** to that system.

---

# ✈️ Designing the Aircraft

## Designing the Wings

![IMG-20220209-WA0031](https://github.com/user-attachments/assets/19b52bf1-c2d1-406c-b38e-c87ef1da0d6e)
![IMG-20220209-WA0034](https://github.com/user-attachments/assets/a69d4d6f-c9b0-4280-bb36-62b71fc00416)

- Airfoil selection and structural design  
- Weight optimization for payload constraints  
- Stability considerations for autonomous flight  
- Iterative prototyping and testing  

The aircraft platform had to be stable and predictable to ensure reliable autonomous behavior.

---

# 🧠 Developing the Navigation System

## Making the Navigation System

![PXL_20220125_095421048](https://github.com/user-attachments/assets/8c4d5e20-585f-4299-aa00-167d13163e67)

I designed and implemented the onboard navigation logic using Python and OpenCV. The system architecture included:

- Real-time camera input processing  
- Color-based target detection  
- Heading computation  
- Error correction and directional output  
- GUI-based monitoring and debugging tools  

The system was built modularly to allow rapid iteration before competition.

---

# 🎯 Color Detection & High-Altitude Target Recognition

One of the primary mission goals was identifying a **yellow landing zone** from altitude.

## Landing Zone (Ground View)

![WhatsApp Image 2026-01-15 at 00 19 22 (1)](https://github.com/user-attachments/assets/aacaaeb5-a89f-4c2b-80ac-2b0b47280d0b)

## Successful Detection from 200+ ft

![WhatsApp Image 2026-01-15 at 00 19 22](https://github.com/user-attachments/assets/8025af07-3ceb-4611-b2f6-36f34f5627d9)

### Technical Approach

- HSV color space filtering for robustness under outdoor lighting  
- Threshold tuning to reduce false positives  
- Contour detection and centroid estimation  
- Directional vector computation relative to aircraft heading  

Detecting a colored region from 200+ feet required careful calibration due to:

- Sunlight variability  
- Motion blur  
- Limited onboard processing power  
- Changing ground textures  

---

# 🔧 Integration Phase

## It’s All Coming Together

![IMG-20220201-WA0006](https://github.com/user-attachments/assets/195a657f-a5f4-49d1-9092-89ad96af81ca)

This phase involved:

- Hardware-software integration  
- Sensor validation  
- Field testing  
- Iterative parameter tuning  

Testing cycles were critical to ensuring reliability before competition day.

---

# 🖥 Control Panel GUI

## The Control Panel Interface

![IMG-20220222-WA0000](https://github.com/user-attachments/assets/112ba1c3-2511-4ada-8b6f-4bb40984d2cf)

I developed a GUI to:

- Visualize live detection results  
- Display heading and positional feedback  
- Tune detection thresholds  
- Monitor system health during tests  

This significantly accelerated debugging and calibration.

---

# 🏗 Final Aircraft Build

## The Final Build

![IMG-20220226-WA0003](https://github.com/user-attachments/assets/84985495-6705-4041-92e2-95ca1b7244b7)

## Autonomous Aircraft with Integrated Navigation System

![IMG-20220226-WA0009](https://github.com/user-attachments/assets/b7cad50b-5489-453a-adf6-b573ea137d5e)

The final system combined:

- Custom-built airframe  
- Autonomous navigation software  
- Vision-based landing zone detection  
- Flight control integration  

---

# 🧩 System Architecture Overview
