# SoundFrequencyMonitoring
Real-time sound frequency monitoring and alert system using MATLAB and Arduino with LED and buzzer notifications.

## Introduction

Unexpected machine failures represent a major challenge in industrial environments, often leading to costly downtime, production losses, and expensive repairs. Numerous studies emphasize that a significant percentage of industrial maintenance budgets is consumed by unplanned breakdowns, which usually occur without any early warning. Early detection of abnormal machine behavior has become a crucial requirement for improving reliability and reducing overall maintenance costs.

This project proposes a simplified machine health monitoring system. A microphone sensor captures the acoustic signature of the machine, and the Arduino microcontroller processes the signal using the Zero-Crossing method to estimate the instantaneous frequency. The system provides visual and audible alerts using LEDs and a buzzer to classify the machine’s condition:

- **Green LED:** Frequency within the normal operating range  
- **Yellow LED:** Minor deviation indicating a slight abnormality  
- **Red LED + Buzzer:** Critical deviation indicating a potential major fault  

Additionally, the measured frequency is transmitted to MATLAB for real-time visualization, filtering, and FFT analysis to enhance diagnostic accuracy.

---

## Project Structure
MyAudioProject/
├─ MATLAB/
│ ├─ audio_fft.m
│ └─ arduino_fft.m
├─ Arduino/
│ └─ audio_leds.ino
├─ AudioFiles/
│ └─ sample.wav
├─ README.md
├─ LICENSE
└─ .gitignore

---

## Features

- Real-time sound frequency monitoring  
- LED and buzzer alerts for abnormal conditions  
- MATLAB visualization with FFT analysis  
- Easy integration with Arduino  
- Lightweight and non-invasive setup  

---

## Hardware & Software Requirements

**Hardware:**  
- Arduino Uno   
- Sound Detector sensor  
- LEDs (Green, Yellow, Red)  
- Buzzer  
- Jumper wires & breadboard  

**Software:**  
- MATLAB   
- Arduino IDE 

---

## Usage

1. Connect the Arduino to your PC.  
2. Upload the Arduino sketch (`audio_leds.ino`) using Arduino IDE.  
3. Open MATLAB scripts (`audio_fft.m` or `arduino_fft.m`) and run them.  
4. Place any audio files in the `AudioFiles` folder if needed.  
5. Observe real-time monitoring via MATLAB GUI and LED/buzzer alerts on Arduino.  

---

## Screenshots / Demo
[ https://github.com/666060/SoundFrequencyMonitoring/blob/main/Screenshot%202025-12-06%20191240.png ]
---

## How It Works
Microphone → Arduino → MATLAB → GUI → LED/Buzzer Alerts

- Microphone captures sound signals from the machine  
- Arduino processes signals and sends frequency data to MATLAB  
- MATLAB visualizes time-domain and FFT spectrum  
- LEDs and buzzer provide real-time alerts  

---

## Future Improvements

- Support multiple Arduino devices simultaneously  
- Store frequency data for long-term analysis  
- Alerts via email or mobile notifications  
- Advanced signal processing algorithms  

---

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.  

---

## References

1.(https://www.mdpi.com/3466738)
2.(https://www.extrica.com/article/21928)
3.(https://arxiv.org/abs/2403.11037?utm_source=chatgpt.com)
4.(https://www.mdpi.com/2886958)

## Contributors
- [ Fata Nagah ](https://www.linkedin.com/in/fatma-nagah-b437a236b?utm_source=share&utm_campaign=share_via&utm_content=profile&utm_medium=android_app)
- [ Hoda Mahmoud ](https://www.linkedin.com/in/hoda-mahmoud-b3327736b?utm_source=share&utm_campaign=share_via&utm_content=profile&utm_medium=android_app)
- [ Nesreen Elemairy ](https://www.linkedin.com/in/nesreen-elemairy-a9078635a?utm_source=share&utm_campaign=share_via&utm_content=profile&utm_medium=android_app)
- [ Sama Mohammed ](https://www.linkedin.com/in/sama-mohamed-005425357?utm_source=share&utm_campaign=share_via&utm_content=profile&utm_medium=android_app)
- [ Fatma Elsaber ](https://www.linkedin.com/in/fatma-elsaber-9ab1b830b?utm_source=share_via&utm_content=profile&utm_medium=member_android)
- [ Zamzam Ali ](https://www.linkedin.com/in/zamzam-ali-6314b4372?lipi=urn%3Ali%3Apage%3Ad_flagship3_profile_view_base_contact_details%3BMtnGzqh3TPiQYCLysbAGTw%3D%3D)

