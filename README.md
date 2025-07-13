#  Energy and Area Efficient Image Multiplication Using Approximate Multipliers

This project presents an **8×8 approximate multiplier design** optimized for low-power, area-efficient image processing. It utilizes **compressor-based logic** (4:2 and 5:2 compressors) to trade off a small amount of accuracy for significantly improved energy and silicon area efficiency, particularly suited for **embedded systems** and **real-time image processing**.

---

##  Abstract

In modern image processing systems, multiplication is a power-intensive operation. This project focuses on the design and implementation of **approximate multipliers** to reduce energy consumption and area usage. Through MATLAB-based simulation, we show how replacing traditional multipliers with approximate ones can:
- Lower power dissipation
- Reduce area
- Maintain acceptable image quality

Key evaluation metrics include:
- **PSNR (Peak Signal-to-Noise Ratio)**
- **Power & Delay**
- **Image fidelity**

---

##  Objectives

- ✅ Design approximate multipliers for image processing
- ✅ Evaluate energy, area, delay, and image quality
- ✅ Perform pixel-wise image multiplication
- ✅ Compare with conventional multipliers

---

##  Methodology

1. **Image Selection**  
   Two grayscale images are selected (e.g., Cameraman, Rice).

2. **Compressor Design (MATLAB)**  
   Logic-level compressor circuits (4:2, 5:2) are implemented.

3. **8×8 Approximate Multiplier Design**  
   Using designed compressors.

4. **Image Multiplication (MATLAB)**  
   Perform pixel-wise image multiplication using the designed approximate multipliers.

5. **Output Analysis**  
   Evaluate using PSNR, visual inspection, and resource usage.

---

##  Results

###  Basic Image Multiplication

*Using MATLAB for exact multiplication of two images.*

![Basic Image Multiplication](results/basic_multiplication.png)

---

###  Approximate Multiplier Simulation Output

*Simulating binary multiplication using an approximate 8×8 multiplier.*

![Approximate Multiplier Design](results/approx_multiplier_design.png)

---

###  Output Using Existing 4:2 Multiplier

- **PSNR: ~2.11 dB**
- Highly distorted and poor image fidelity.

![Image with Existing Multiplier](results/existing_multiplier_output.png)

---

###  Output Using Proposed 5:2 Multiplier

- **PSNR: ~7.03 dB**
- Improved clarity and less visual distortion.

![Image with Proposed Multiplier](results/proposed_multiplier_output.png)

---

###  PSNR Comparison

Comparison of image quality between existing and proposed architectures.

![PSNR Comparison Chart](results/psnr_comparison_chart.png)

---

##  Performance Metrics Summary

| Architecture   | Power (W) | On-Chip Temp (°C) | PSNR (dB) |
|----------------|-----------|--------------------|-----------|
| Dadda          | 13.87     | 88.3               | N/A       |
| PM1 (4:2)      | 11.4      | 83.2               | 2.11      |
| PM2 (Hybrid)   | 10.9      | 81.7               | ~4.50     |
| **PM3 (5:2)**  | **8.2**   | **75.7**           | **7.03**  |

---

##  Tools & Technologies

- 🧪 MATLAB (Simulation & PSNR analysis)
- 💻 Verilog (Compressor design)
- 🔧 Xilinx Vivado (Implementation)
- 📉 Image Quality Metrics: PSNR, MSE

---

##  Citation

If you use this work, please cite:

```text
K. Maneesha, K. Teja, B. Eswar Naik,
"Energy and Area Efficient Image Multiplication Using Approximate Multipliers",
Velagapudi Ramakrishna Siddhartha Engineering College, May 2025.
