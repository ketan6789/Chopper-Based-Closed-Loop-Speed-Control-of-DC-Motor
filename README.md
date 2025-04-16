[![View Chopper-Based-Closed-Loop-Speed-Control-of-DC-Motor on File Exchange](https://www.mathworks.com/matlabcentral/images/matlab-file-exchange.svg)](https://in.mathworks.com/matlabcentral/fileexchange/180817-chopper-based-closed-loop-speed-control-of-dc-motor)

# Closed-Loop DC Motor Control Using Four-Quadrant Chopper

![image](https://github.com/user-attachments/assets/3fd69160-a10f-4df1-9b06-246b574f9fe6)


This repository contains a MATLAB Simulink model for implementing **closed-loop speed control of a DC motor** using a **four-quadrant chopper (E-type)**. The model supports bidirectional motor operation, including motoring and regenerative braking in both directions.

---

## 🌀 Features

- Full H-bridge (four-quadrant) chopper
- Closed-loop speed control with PID
- PWM-based switching logic with quadrant selector
- Current feedback control
- Supports operation in all four quadrants:
  - Quadrant I: Forward Motoring
  - Quadrant II: Forward Braking
  - Quadrant III: Reverse Motoring
  - Quadrant IV: Reverse Braking

---

## ⚠️ Current Limitation

While Quadrants I and III (motoring modes) operate correctly, the expected braking behavior in Quadrants II and IV (i.e., **speed decreasing to zero**) is **not observed** in this model.  
This is due to the **absence of a reverse current path or energy dissipation mechanism** (e.g., a brake resistor or regenerative sink) on the DC supply side.

---

## 🚀 How to Use

1. Clone the repository:
   ```bash
   git clone https://github.com/ketan6789/Chopper-Based-Closed-Loop-Speed-Control-of-DC-Motor.git
   ```
2. Open MATLAB and navigate to the folder.
3. Launch the Simulink model:
   ```matlab
   open('ClosedLoopDCMotor.slx')
   ```
4. Run the simulation and observe motor behavior in different quadrants.

---

## 📜 License

This project is licensed under the **MIT License**.

---

## 🙌 Acknowledgment

Developed by Ketan Singh for academic experimentation in closed-loop control and power electronics simulation.

🚀 Simulate | 🔁 Regenerate | 🧠 Learn

