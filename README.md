# SoundFrequencyMonitoring
Real-time sound frequency monitoring and alert system using MATLAB and Arduino with LED and buzzer notifications.

## Introduction

Unexpected machine failures represent a major challenge in industrial environments, often leading to costly downtime, production losses, and expensive repairs. Numerous studies emphasize that a significant percentage of industrial maintenance budgets is consumed by unplanned breakdowns, which usually occur without any early warning. As highlighted by recent research such as “A Review on Vibration Monitoring Techniques for Predictive Maintenance of Rotating Machinery” (MDPI, 2023) and “Vibration Signal Analysis for Intelligent Rotating Machinery Diagnosis and Prognosis” (MDPI, 2024), early detection of abnormal machine behavior has become a crucial requirement for improving reliability and reducing overall maintenance costs.

One of the most effective non-invasive methods for early fault detection is vibration and acoustic analysis. According to established studies, machines typically operate within a stable and predictable vibration or sound frequency range. Any deviation from this range often indicates underlying mechanical issues, such as imbalance, bearing wear, misalignment, or loose components. Case studies—such as “Vibration and Faults Prediction for Air Blowers – Case Study” (EKB, 2019)—prove the real-world effectiveness of vibration monitoring in identifying potential failures before they escalate into critical faults.

Based on these principles, this project proposes a simplified machine health monitoring system. A microphone sensor captures the acoustic signature of the machine, and the Arduino microcontroller processes the signal using the Zero-Crossing method to estimate the instantaneous frequency. This frequency is then compared with the predefined normal operating range of the machine. The system provides visual and audible alerts using LEDs and a buzzer to classify the machine’s condition:

- **Green LED:** Frequency within the normal operating range
- **Yellow LED:** Minor deviation indicating a slight abnormality
- **Red LED + Buzzer:** Critical deviation indicating a potential major fault

Additionally, the measured frequency is transmitted to MATLAB for further processing, real-time visualization, filtering, and FFT analysis to enhance diagnostic accuracy.

The proposed system aligns with recent research and predictive maintenance strategies by offering an early-warning mechanism that helps prevent unexpected breakdowns, reduce downtime, and lower maintenance costs.

---

## Project Structure
MyAudioProject/
│
├─ MATLAB/
│   └─ audio_fft.m
│   └─ arduino_fft.m
│
├─ Arduino/
│   └─ audio_leds.ino
│
├─ AudioFiles/
│   └─ sample.wav
│
└─ README.md

---

## Usage

1. **Connect the Arduino** to your PC.  
2. **Upload the Arduino sketch** (`audio_leds.ino`) using Arduino IDE.  
3. **Open MATLAB scripts** (`audio_fft.m` or `arduino_fft.m`) and run them.  
4. **Place the audio files** in the `AudioFiles` folder if needed.  
5. **Observe real-time monitoring** via MATLAB GUI and LED/buzzer alerts on Arduino.  

---

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.

---

## References

1. “A Review on Vibration Monitoring Techniques for Predictive Maintenance of Rotating Machinery” (MDPI, 2023)  
2. “Vibration Signal Analysis for Intelligent Rotating Machinery Diagnosis and Prognosis” (MDPI, 2024)  
3. “Vibration and Faults Prediction for Air Blowers – Case Study” (EKB, 2019)

