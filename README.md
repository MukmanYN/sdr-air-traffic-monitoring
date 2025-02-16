# SDR Air Traffic Communication Monitoring  

## 🛫 Project Overview  
This project implements a **Software-Defined Radio (SDR)** system to intercept and analyze live air traffic communications from the **Frederick Douglass Greater Rochester International Airport**. Using an **ADALM-PLUTO SDR** and a **simple dipole antenna**, the system demodulates **AM signals** from the **118-136 MHz aviation band** and processes them with **MATLAB** for signal analysis.  

The primary goal was to explore the capabilities of **SDRs for aviation communication** and understand the behavior of **AM signals** in real-world conditions.  

---

## ⚙️ System Architecture and Setup  

### 📡 **Hardware:**  
- **ADALM-PLUTO SDR:** Modified for extended frequency range (70 MHz to 6 GHz)  
- **Simple Dipole Antenna:** Tuned to 1.87 feet for the target frequency  
- **Power Supply:** Standard USB connection for Pluto SDR  

### 🖥️ **Software:**  
- **SDR#:** For signal demodulation and live frequency scanning  
- **PuTTY:** For terminal access to the SDR  
- **MATLAB:** For signal processing and audio enhancement  

### 🛠️ **SDR Modification:**  
- Overcame the Pluto SDR's frequency limitation (`325 MHz - 3800 MHz`) by modifying its firmware, expanding its range to **70 MHz - 6 GHz** with a **56 MHz bandwidth**.  
- Used an **older version of SDR#** for compatibility with the modified Pluto SDR.  

---

## 📊 Key Features and Technologies Used  

### ✅ **Signal Reception:**  
- Tuned the dipole antenna length to **1.87 feet**, calculated for optimal reception at **124.824 MHz**.  
- Scanned and recorded real-time air traffic control communications.  

### ✅ **AM Demodulation:**  
- Configured **SDR#** to **AM modulation** for listening to **air traffic control frequencies (118-136 MHz)**.  

### ✅ **MATLAB Signal Processing:**  
- Processed audio signals from the SDR to improve clarity.  
- Experimented with noise filtering methods in MATLAB.  

### ✅ **Frequency Range Modification:**  
- Modified the **Pluto SDR** to bypass its default frequency limitation.  

---

## 🚧 Challenges Faced and Lessons Learned  

### ❌ **Signal Amplification Issues:**  
- Attempted to improve signal clarity using an external amplifier. However, it increased **both signal and noise**, leading to poor results.  

### ❌ **Audio Extraction Problems:**  
- Could not directly extract clear audio from **SDRSharp** due to file compatibility issues.  
- Used **MATLAB** to attempt audio reconstruction but results remained noisy.  

### ❌ **Limited Air Traffic Activity:**  
- Testing opportunities were limited due to sparse air traffic during the recording period.  

---

## 🚀 Results and Future Improvements  

### 📌 **Results:**  
- Successfully intercepted and recorded **live air traffic control signals**.  
- Demonstrated the effectiveness of a **modified SDR** for aviation band reception.  
- Identified areas for **improving signal processing** techniques.  

### 💡 **Future Improvements:**  
- Implement a **directional antenna** for better signal isolation.  
- Use a more effective **RF amplifier** with noise filtering.  
- Develop advanced **MATLAB filters** for noise reduction.  

---
