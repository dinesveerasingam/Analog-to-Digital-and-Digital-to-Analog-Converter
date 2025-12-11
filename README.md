# Analog-to-Digital-and-Digital-to-Analog-Converter


This task focuses on building a complete **2-bit Analog-to-Digital (ADC) and Digital-to-Analog (DAC)** system using practical analog components. The design includes filtering, sampling, conversion, and signal reconstruction, verified through both simulation and hardware testing

### 🔧 System Overview
The AD/DA system consists of the following stages:

- **4th-Order Butterworth Low-Pass Filters (LPF)**  
  - Used as the **anti-aliasing filter** (input) and **reconstruction filter** (output)  
  - Unity-gain configuration  
  - Provides flat passband response and smooth signal reconstruction  
  - Suppresses high-frequency noise and aliasing effects  

- **Sample-and-Hold Circuit**  
  - Captures the analog input at each clock cycle  
  - Ensures stable signal levels during ADC conversion  

- **Comparator-Based 2-bit ADC**  
  - Implemented using LM358P op-amps and discrete comparators  
  - Converts the sampled signal into 2-bit digital outputs  

- **Resistor-Based DAC (Weighted Resistor / R-2R Type)**  
  - Reconstructs the analog signal from the 2-bit digital output  

- **Reconstruction Low-Pass Filter (4th-order Butterworth)**  
  - Removes DAC step artifacts  
  - Smoothens the analog output waveform  


### 📈 Adaptive Peak Detection
An **adaptive peak detection circuit** was integrated to enhance conversion accuracy.

Benefits:
- More stable quantization levels  
- Reduced error during 2-bit threshold detection  
- Improved reconstructed output quality  


### 🛠️ Components Used
- LM358P operational amplifiers  
- 4th-order unity-gain Butterworth filters  
- Comparators  
- MOSFETs for switching  
- Weighted resistor network / R-2R DAC  
- Peak detector circuit components  

### 🧪 Verification & Testing

**Simulation Testing**
- Verified frequency response of filters  
- Checked comparator switching thresholds  
- Tested sampling behavior and DAC output waveform  

**Breadboard Testing**
- Real hardware validation  
- Measured ADC thresholds and DAC levels  
- Confirmed LPF response and reconstructed signal performance  

### 📌 Outcome
Task 1 successfully demonstrates a complete **2-bit AD/DA conversion system**, including:

- Anti-aliasing and reconstruction filtering  
- Sample-and-hold operation  
- Comparator-based ADC  
- Resistor-based DAC  
- Adaptive peak detection  
- Full simulation and hardware validation  

This establishes a reliable and accurate analog signal processing chain suitable for low-bit data conversion experiments.




