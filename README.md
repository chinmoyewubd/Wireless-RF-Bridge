# Wireless Data Transmission System using RF Modules

![Project Status](https://img.shields.io/badge/status-completed-brightgreen)
![License](https://img.shields.io/badge/license-MIT-blue)

## 📌 Overview

This project demonstrates a wireless data transmission system using RF (Radio Frequency) transmitter and receiver modules. The system successfully transmits data wirelessly through unguided media, specifically using RF technology, which is one of the two main types of wireless transmission (RF and optical).

## 🎯 Features

- Wireless data transmission using RF modules
- Push-button controlled input on transmitter side
- LED indicators on receiver side for visual feedback
- HT12E Encoder IC for data encoding
- HT12D Decoder IC for data decoding
- Real-time wireless communication demonstration

## 🛠️ Hardware Components

### Transmitter Circuit
- RF Transmitter Module (434 MHz)
- HT12E Encoder IC
- Push buttons (4 switches)
- LEDs for status indication
- Resistors and connecting wires
- Power supply (5V)

### Receiver Circuit
- RF Receiver Module (434 MHz)
- HT12D Decoder IC
- LEDs (4 for output indication)
- Resistors and connecting wires
- Power supply (5V)

## 📋 How It Works

1. **Power Supply**: When power is supplied to both circuits, all LEDs initially glow due to internal pull-up resistors in the encoder IC.

2. **Data Transmission**: 
   - Pressing a push-button on the transmitter circuit connects the corresponding data pin to ground
   - The encoder IC processes this input and sends it through the RF transmitter
   - The RF receiver captures the signal and the decoder IC processes it

3. **Output Indication**:
   - The corresponding LED on the receiver circuit turns OFF
   - For example: Pressing Switch 1 (connected to AD11/pin13 of Encoder) turns OFF the LED connected to D11/pin13 of Decoder

## 📊 Block Diagram

```
Transmitter Side:
[Push Buttons] → [HT12E Encoder] → [RF Transmitter Module] → Antenna
↓
Wireless Medium
↓
Receiver Side:
Antenna → [RF Receiver Module] → [HT12D Decoder] → [LED Indicators]
```

## 🔧 Setup Instructions

1. **Assemble the Transmitter Circuit**:
   - Connect HT12E encoder IC according to the circuit diagram
   - Attach push buttons to pins D8-D11
   - Connect RF transmitter module to encoder output
   - Provide 5V power supply

2. **Assemble the Receiver Circuit**:
   - Connect HT12D decoder IC as per circuit diagram
   - Attach LEDs to output pins D8-D11
   - Connect RF receiver module to decoder input
   - Provide 5V power supply

3. **Testing**:
   - Power on both circuits
   - Verify all LEDs are glowing
   - Press individual push buttons and observe corresponding LEDs turning OFF

## 📈 Results

The project successfully demonstrates wireless data transmission where:
- Input from push buttons is wirelessly transmitted via RF
- The receiver circuit accurately decodes and displays the transmitted data
- LED status changes confirm successful data transmission and reception

## 🚀 Future Improvements

- Increase transmission range with better antennas
- Add more input/output channels
- Implement data encryption for security
- Integrate with microcontroller for automated operations
- Develop real-life applications like remote controls or sensor networks

## 📚 Applications

- Remote control systems
- Wireless sensor networks
- Home automation
- Industrial monitoring
- Short-range data communication

## 👥 Contributors

- Project Team, CSE345

## 🙏 Acknowledgments

- Thanks to the course instructors of CSE345
- RF module documentation and resources
- Open-source hardware community

---

**Note**: This project was developed as part of an academic project for CSE345 course. For any queries or suggestions, please feel free to open an issue or submit a pull request.
