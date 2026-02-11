# WeldRight-Real-Time-Weld-Defect-Detection

WeldRight is an AI-powered system that detects weld defects in real-time using acoustic sensing and machine learning.

This repository contains the full technical documentation for the V0 prototype, including system architecture, enclosure design, electrical schematics, microphone mounting, verification testing, and ML development.

📄 **Full Technical Report:**  
[View the Final Report (PDF)](./Final%20Technical%20Report.pdf)

Problem:

Traditional weld inspection occurs after welding is complete, leading to costly rework and downtime. The goal of WeldRight was to create a non-intrusive add-on system capable of detecting weld defects during the welding process.

The primary technical challenges were:

- Severe electromagnetic interference (EMI) from welding arcs
- Conditioning extremely low-amplitude acoustic signals (~36 mV)
 -Designing an industrial enclosure that functioned as a Faraday cage
- Achieving high-resolution acoustic capture without obstructing the welder

My Contributions:

My team and I were responsible for the electrical and mechanical system design of the V0 prototype, including:

- Electrical Design
- Multi-stage signal amplification and filtering
- Bessel low-pass anti-aliasing filter
- Level shifting for 0–3.6V ADC compatibility
- Voltage spike protection in high-EMI environments

EMI Mitigation & Enclosure

- Designed and grounded a steel enclosure acting as a Faraday cage
- Integrated bulkhead connectors and optimized grounding paths
- Designed isolated mounting plates for PCB and amplifier

Microphone Mount

- 3D modeled and fabricated non-conductive mount
- Integrated grounded mesh spark shield
- Iteratively optimized placement for signal quality vs. user intrusion

Outcome:

The final V0 prototype successfully operated in a live welding environment. EMI shielding and signal conditioning reduced interference to acceptable levels, enabling stable acquisition of weld acoustic signatures between 0.6–15 kHz. Clean data allowed successful feature extraction and defect classification using machine learning models.

The system evolved from a noisy proof-of-concept to a reliable, industrially viable prototype.

Technologies:

- Analog signal conditioning
- PCB prototyping
- EMI shielding design
- SolidWorks CAD
- Python (STFT, SVM classification)
- Industrial hardware integration
