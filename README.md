# Common-Source-Amplifier-Report-with-PMOS-and-NMOS-Transistors
# Circuit Description
This circuit is a common-source amplifier made using both a PMOS (M2) and NMOS (M1) transistor. The main components are:
![Screenshot 2025-02-17 231357](https://github.com/user-attachments/assets/48384385-2988-47c2-8d0f-446269e7fbd9)

VDD (Supply Voltage): 1.8V
Input Signals (V1 and V2):
V1: 0.48V peak sine wave, 1 kHz frequency.
V2: 0.9V peak sine wave, 1 kHz frequency.
Output Node: Vout (connected between the transistors).
Analysis Overview
I ran different simulations to check how the amplifier works in various conditions:

# 1. DC Operating Point Analysis
Goal: Find out the steady-state (resting) conditions of the circuit.
What I Noticed:
Both transistors are set up so they are in the correct mode for amplification.
![WhatsApp Image 2025-02-17 at 23 28 00_c9016efb](https://github.com/user-attachments/assets/90de7fc8-0e61-4e6d-94ea-8d3e3329bb8f)

# 2. DC Transfer Characteristics
Goal: See how output voltage (Vout) changes when the input voltage (Vin) is swept.
Results:
The output changes with input in a way that looks like a typical amplifier curve.
There is a phase inversion (output goes down as input goes up), which is expected.
![WhatsApp Image 2025-02-17 at 23 28 01_d9fdfa82](https://github.com/user-attachments/assets/60095a07-8e31-4af1-bbae-3f2cd14c197c)


# 3. AC Analysis
Goal: Check the amplifier’s gain and frequency behavior.
Results:
The gain was about -1.2, meaning the signal gets inverted.
The circuit works best at low frequencies.
![WhatsApp Image 2025-02-17 at 23 28 00_bb4e8b56](https://github.com/user-attachments/assets/0904c0f3-6465-461b-acd8-f794169a4461)
![WhatsApp Image 2025-02-17 at 23 28 01_b0a1c695](https://github.com/user-attachments/assets/32dd879f-7e06-47d5-9e28-6cfd12f6a708)



# 4. Transient Analysis
Goal: Look at how the circuit handles a sine wave over time.
Results:
The output followed the input, but there was some distortion at the peaks for larger input signals.
Observations
The amplifier works like it should, flipping the signal upside down.
The gain is okay, but not super high.
It’s best for low-frequency signals, but it could be improved for higher frequencies.
Keeping the input small avoids distortion.
![WhatsApp Image 2025-02-17 at 23 28 02_78dcd81d](https://github.com/user-attachments/assets/bb97268c-68f2-467d-9d34-00487d69749c)

# inference 

Higher Gain: Replacing R_D with PMOS increases output resistance, boosting voltage gain.

 Better Stability: PMOS current source maintains a steady drain current, improving biasing.
 
 Lower Power Consumption: Uses less voltage headroom than a large resistor.
 
 Frequency Response Shift: Higher impedance increases gain-bandwidth product but introduces a dominant pole.
 

Conclusion: The PMOS active load enhances performance, making the amplifier more efficient and suitable for high-gain applications.



Prepared by: shwetha m
Date: [17/02/2025]
Simulation Tool Used: [LTSpice or Ngspice]

