# A S Prajwal Bhat

<p align="center">
  <strong>Electronics & Communication Engineering · BIT Bengaluru · Class of 2027</strong>
</p>

<p align="center">
  <a href="https://as-prajwal-bhat.github.io/AS_Prajwal_Bhat/">Portfolio</a> ·
  <a href="https://as-prajwal-bhat.github.io/AS_Prajwal_Bhat/docs/A_S_Prajwal_Bhat_Resume.pdf">Resume</a> ·
  <a href="mailto:prajwalbhat113@gmail.com">Email</a>
</p>

<p align="center">
  <a href="https://github.com/AS-Prajwal-Bhat">
    <img src="https://cdn.simpleicons.org/github/C4CEB8" height="24" alt="GitHub"/>
  </a>&nbsp;&nbsp;
  <a href="https://www.linkedin.com/in/a-s-prajwal-bhat-aa3717296/">
    <img src="https://cdn.simpleicons.org/linkedin/C4CEB8" height="24" alt="LinkedIn"/>
  </a>&nbsp;&nbsp;
  <a href="https://ieee-collabratec.ieee.org/app/p/ASPrajwalBhat1180865">
    <img src="https://cdn.simpleicons.org/ieee/C4CEB8" height="24" alt="IEEE Collabratec"/>
  </a>
</p>

<p align="center">
  <img src="assets/header.svg" width="100%" alt="Header"/>
</p>

## About

I'm a final-year Electronics and Communication Engineering student at Bangalore Institute of Technology, Bengaluru, graduating in 2027.

My work spans digital design, FPGA development, computer architecture and embedded systems. I enjoy understanding how hardware works at the RTL level, building systems around microcontrollers, and developing software tools that make hardware design more accessible.

Currently, I'm particularly interested in **RTL design, FPGA development, digital verification and VLSI design**. I have also completed hands-on training in the RTL-to-GDSII flow using Cadence tools.

---

## Selected Projects

### 1. Pipelined RISC-V SoC for Edge Vision Intelligence

<p align="center">
  <img src="assets/soc.svg" width="100%" alt="RISC-V SoC"/>
</p>

**Verilog · RISC-V · FPGA · AXI4-Lite · BRAM · UART · DCT · CNN · Vivado**

A team-based major project focused on building a RISC-V-based system-on-chip that performs image processing and classification using dedicated hardware accelerators.

- Designed around a **5-stage pipelined RISC-V processor**, incorporating data forwarding, hazard detection and hardware multiply/divide support.
- Integrated memory-mapped peripherals through an AXI4-Lite bridge and an MMIO interconnect.
- Developed two hardware accelerators:
  - **8×8 Discrete Cosine Transform (DCT):** Processes image blocks for the image-processing pipeline.
  - **LeNet-5-inspired CNN:** Performs digit classification using int8 quantized weights.
- Implemented shared on-chip BRAM with arbitration to coordinate memory access between the processor and accelerators.
- Integrated UART communication for image input and classification output.

**Simulation flow:** A 32×32 digit image is transmitted through UART, processed by the DCT and CNN accelerators, and the predicted class is returned through UART. The complete flow has been exercised in Vivado behavioral simulation.

**Target platform:** Real Digital Blackboard (Zynq-7007S), 100 MHz.

<p align="center">
  <img src="assets/soc-diagram.svg" width="100%" alt="RISC-V SoC block diagram"/>
</p>

---

### 2. CEDA – EDA Logic Gate Compiler

<p align="center">
  <img src="assets/ceda.svg" width="100%" alt="CEDA project"/>
</p>

**C · Python · Tkinter · Compiler Design · Verilog · EDA**

A custom Electronic Design Automation toolchain developed to bridge the gap between digital circuit design and HDL generation.

The project started with the idea of creating a simpler way to describe digital circuits and translate them into hardware description code.

- Developed a compiler of approximately **2,300 lines of C** that translates a custom `.eda` hardware description language into synthesizable Verilog.
- Built the compiler around a structured translation flow, taking source descriptions through parsing and processing before generating Verilog.
- Developed graphical tools to make circuit construction and code generation more accessible.
- Added a visual circuit-building workflow where logic gates can be placed and connected to create a circuit representation.
- Included GUI utilities and browser-based editors alongside the compiler.

The project combines compiler development, digital logic, graphical interfaces and hardware description language generation.

---

### 3. Vedic Multiplier

<p align="center">
  <img src="assets/vedic.svg" width="100%" alt="Vedic multiplier"/>
</p>

**Verilog · Digital Logic Design · Hierarchical RTL · Vivado**

A 4-bit unsigned multiplier based on the **Urdhva Tiryagbhyam (Vertical and Crosswise)** Vedic multiplication technique.

- Implemented a hierarchical architecture using smaller 2×2 multiplier blocks.
- Combined partial products using adder logic to obtain the final 8-bit product.
- Structured the design using modular Verilog components.
- Verified the implementation against expected multiplication results across all **256 possible input combinations**.

The project provided practical experience in arithmetic circuit design, RTL modularity and exhaustive functional verification.

---

### 4. RoboSentinel – Intelligent Surveillance System

<p align="center">
  <img src="assets/robosentinel.svg" width="100%" alt="RoboSentinel"/>
</p>

**MATLAB · Computer Vision · Face Recognition · Embedded Firmware · Web Dashboard**

An intelligent surveillance system designed to detect, recognize and log people in real time.

- Implemented face detection and recognition using MATLAB vision algorithms.
- Added real-time logging of recognized individuals.
- Developed a web dashboard for monitoring activity and managing users.
- Integrated embedded firmware for control logic and real-time system decisions.

The project brings together computer vision, embedded control and a web-based monitoring interface.

---

### 5. BIOHAPTIK – Haptic Feedback System

**ESP32 · I2S · Embedded Systems · Sensors · Machine Learning · Haptics**

A wearable haptic feedback concept aimed at making environmental information more accessible to people with combined hearing and visual impairments.

- Designed a system to interpret environmental audio and spatial information and convert it into tactile feedback.
- Used an ESP32 as the central embedded controller.
- Incorporated an I2S microphone for audio acquisition and ultrasonic sensing for distance awareness.
- Planned audio classification to distinguish important environmental sounds such as voices, alarms and horns.
- Used vibration motors to communicate detected information through tactile patterns.

The prototype explores how embedded sensing and on-device intelligence can translate information from the surrounding environment into an alternative sensory interface.

---

### 6. ESP32 Vision Rover

**ESP32 · ESP32-CAM · HTML · CSS · JavaScript · Embedded Systems**

An internet-connected RC rover with browser-based control, live video streaming and real-time telemetry.

- Built around an ESP32 controller and ESP32-CAM for wireless control and video streaming.
- Developed a browser-based dashboard with a joystick interface for remote movement.
- Integrated sensor telemetry, including distance, IR, temperature, gas and battery information.
- Added communication and latency monitoring to observe system behaviour.
- Incorporated image-recognition alerts into the monitoring interface.

The project combines embedded firmware, wireless communication, sensor integration and a web-based user interface.

---

### 7. Additional Digital Design & Embedded Projects

**Round Robin Arbiter – Verilog**

Designed a round-robin arbitration circuit that provides cyclic and fair access to a shared resource among multiple requesters.

**Traffic Light Controller – Verilog**

Implemented a multi-phase traffic light controller using a finite-state machine, with state transitions and timing behaviour verified through simulation.

**IoT Smart Environment Monitoring – Python & Sensors**

Developed a real-time monitoring pipeline combining hardware sensor inputs, Python-based data processing and structured anomaly logging.

**Electronic Voting Machine – Verilog**

Designed an electronic voting machine while learning Verilog, applying digital logic and sequential design concepts.

---

## Technical Skills

| Domain | Technologies & Concepts |
|---|---|
| **Digital Design & RTL** | Verilog, RTL design, combinational and sequential logic, FSMs, arithmetic circuits, arbiters, testbenches |
| **FPGA & Verification** | Xilinx Vivado, XSim, behavioral simulation, functional verification, synthesis and implementation workflows |
| **Computer Architecture** | RISC-V, 5-stage pipelining, forwarding, hazard detection, memory-mapped I/O, AXI4-Lite, BRAM, hardware accelerators |
| **VLSI & EDA** | Cadence tools, RTL-to-GDSII flow, NGSpice, Xschem, Magic, Sky130 PDK |
| **Embedded Systems** | ESP32, ESP32-CAM, 8051, NXP FRDM-MCXN236, Arduino, sensor interfacing, UART, SPI, I²C |
| **Programming** | C, C++, Python, MATLAB, SQL |
| **Software & Development Tools** | Git, GitHub, Linux, WSL, Tkinter, HTML, CSS, JavaScript |

---

## Leadership & Activities

**General Secretary – IEEE Student Branch, BIT**  
*August 2025 – Present*

- Help coordinate student branch activities, technical workshops and hands-on competitions.
- Organized technical workshops covering areas such as Linux, TCL and VLSI.
- Led and coordinated technical events, including Arduino and Verilog-based activities.
- Hosted and coordinated **Smart Eco Sign**, a national-level hackathon with approximately 80 participants from across India.

**Secretary – IEEE CEDA & CAS Societies, BIT Student Branch**  
*December 2025 – Present*

- Contribute to technical initiatives and activities related to Electronic Design Automation and Circuits and Systems.

**Placement Coordinator – Bangalore Institute of Technology**

- Support placement-related coordination and communication among students.

**Associate Design Lead – IEEE CEDA & CAS Societies**  
*March – August 2025*

- Led a college-wide Verilog Design Competition.
- Helped organize the SmartEco+ Design Hackathon.

---

## Achievements & Training

- **Winner – IoT and Embedded Systems with ESP32 Hackathon**, Exovian Robotics, BIT (October 2025). College-level hackathon.
- **NPTEL Top 5% – The Joy of Computing using Python**, IIT Madras (86%, Elite + Silver).
- **IoT Intern – Emertxe**, working on an Edge AI-Based Smart EV Charging Station Optimizer (August–September 2026).
- **RTL to GDSII using Cadence Tools** – Five-day industry training at BIT (April 2026).
- **Student Internship Program 3.0** – IEEE CASS Bangalore Chapter (October–December 2025).

Additional certifications and details are available on my [portfolio](https://as-prajwal-bhat.github.io/AS_Prajwal_Bhat/).

---

## Connect

I'm interested in opportunities involving FPGA development, RTL design, digital verification and embedded hardware.

<p align="center">
  <a href="https://github.com/AS-Prajwal-Bhat">
    <img src="https://cdn.simpleicons.org/github/C4CEB8" height="26" alt="GitHub"/>
  </a>&nbsp;&nbsp;
  <a href="https://www.linkedin.com/in/a-s-prajwal-bhat-aa3717296/">
    <img src="https://cdn.simpleicons.org/linkedin/C4CEB8" height="26" alt="LinkedIn"/>
  </a>&nbsp;&nbsp;
  <a href="https://ieee-collabratec.ieee.org/app/p/ASPrajwalBhat1180865">
    <img src="https://cdn.simpleicons.org/ieee/C4CEB8" height="26" alt="IEEE Collabratec"/>
  </a>
</p>

<p align="center">
  <a href="mailto:prajwalbhat113@gmail.com">prajwalbhat113@gmail.com</a> · Bengaluru, India
</p>
