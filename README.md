# Analog-to-Digital-and-Digital-to-Analog-Converter
In this task, a complete 2-bit Analog-to-Digital (ADC) and Digital-to-Analog (DAC) conversion chain was designed, simulated, and tested on a breadboard. The system includes all major signal-processing stages required in a practical data-conversion pipeline.

🔧 System Overview

The AD/DA system was developed with the following major components:

•	4th-Order Butterworth Low-Pass Filters (LPF)

Used at both the input (anti-aliasing filter) and output (reconstruction filter) stages.

These unity-gain Butterworth filters ensure:

  o	Flat passband response
  
  o	No ripple
  
  o	Smooth signal reconstruction
  
  o	Effective reduction of high-frequency noise and aliasing
•	Sample-and-Hold Circuit
Captures and holds the analog input signal for stable conversion during each clock cycle.
•	Comparator-based 2-bit ADC
Implemented using LM358P op-amps and discrete comparators to generate 2-bit digital output levels.
•	Resistor-based DAC (R-2R Ladder / Weighted Resistor Network)
Converts the 2-bit digital signal back into an analog output.
•	Reconstruction Filter (4th-order Butterworth LPF)
Smoothens the DAC output and removes stair-step behavior.

📈 Adaptive Peak Detection
To improve system accuracy, an adaptive peak detection algorithm was implemented using op-amp rectifiers and peak-hold capacitive circuits.
This resulted in:
•	More stable digital level transitions
•	Reduced error in 2-bit quantization
•	Better reconstruction quality after the DAC stage

🛠️ Components Used
•	LM358P operational amplifiers
•	4th-order unity-gain Butterworth filters
•	MOSFET switching elements
•	Comparators
•	Weighted-resistor DAC or R-2R DAC
•	Peak detector circuits

🧪 Verification & Testing
The full system was tested using:
•	Simulation (LTspice/Multisim/Proteus)
  — Verified frequency response, sampling behavior, comparators, and DAC levels.
•	Breadboard Implementation
  — Validated real-world signal flow
  — Measured ADC thresholds and DAC output
  — Ensured filter behavior matched design targets
  
📌 Outcome
Task 1 successfully demonstrated a fully functional 2-bit AD/DA conversion system with practical filtering, sampling, conversion, and signal reconstruction stages. The inclusion of adaptive peak detection and 4th-order Butterworth filters significantly improved overall performance and signal integrity.

