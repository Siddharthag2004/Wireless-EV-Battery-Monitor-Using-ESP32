# Wireless EV Battery Monitor Using ESP32

This project wirelessly monitors voltage, current, and temperature from an EV battery using the ESP32. It uses:

- ADS1115 for voltage sensing
- ACS712 for current sensing
- DS18B20 for temperature sensing
- ESP32 with WebSocket server for real-time data

## Live Monitoring via WebSocket

Data is streamed to connected clients using WebSocket on port 81.

## Hardware Components

- ESP32 Dev Module
- ADS1115 ADC
- ACS712 Current Sensor
- DS18B20 Temperature Sensors (x3)
- Jumper wires and Breadboard

## How to Use

1. Flash `main.ino` to your ESP32.
2. Connect to your Wi-Fi by updating `ssid` and `password` in the code.
3. Open Serial Monitor for debug logs.
4. Connect a WebSocket client to `ws://<ESP32_IP>:81` to receive JSON data.

## 🖼️ Wiring Diagram

![Wiring](docs/images/wiring_diagram.jpg)

## 📄 License

MIT License
