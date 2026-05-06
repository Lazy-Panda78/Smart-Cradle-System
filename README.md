# IoT-Based Smart Cradle System

A smart baby cradle prototype developed using ESP32, sensors, and embedded automation to assist in baby monitoring and basic caregiving tasks.

This project was built as a 4th semester IoT field project at GLA University, Mathura.

---

## Project Overview

The main idea behind this project was to create a simple and practical smart cradle system that can automatically respond to different conditions around a baby.

The system continuously monitors:
- Baby crying using a sound sensor
- Temperature and humidity using DHT11
- Environmental conditions around the cradle

Based on the sensor readings, the cradle can automatically:
- Swing when crying is detected
- Turn on a cooling fan during high temperature
- Trigger alerts using a buzzer
- Display system status on an LCD screen

The goal of the project was to explore how IoT and embedded systems can be applied in real-life caregiving applications.

---

## Features

- Automatic cradle swinging mechanism
- Cry detection using sound sensor
- Temperature monitoring
- Humidity monitoring
- Automatic fan control
- Real-time LCD status display
- Buzzer alert system
- ESP32-based automation

---

## Components Used

- ESP32 Development Board
- DHT11 Temperature & Humidity Sensor
- Sound Sensor
- Relay Module
- L298N Motor Driver
- DC Motor
- LCD I2C Display
- Buzzer
- Jumper Wires & Breadboard

---

## How the System Works

### Cry Detection
The sound sensor continuously checks sound intensity levels.  
When the sound crosses a predefined threshold, the ESP32 activates the motor, which swings the cradle for a fixed duration.

### Temperature Monitoring
The DHT11 sensor monitors temperature in real time.  
If the temperature rises above the set threshold, the relay module turns on the fan automatically.

### Humidity Monitoring
The system also monitors humidity levels.  
If humidity exceeds the safe range, the buzzer is activated to alert nearby users.

### LCD Feedback
The LCD displays different system states such as:
- MONITORING
- FAN ON
- CRY MOTOR ON
- FAN + CRY ACTIVE

---

## Project Images

### Prototype Demonstration

![Prototype](images/image2.jpeg)

---

### Hardware Setup

![Hardware Setup](images/image1.jpeg)

---

## Demonstration Video

Project walkthrough and prototype demonstration:

🔗 https://www.linkedin.com/posts/yash-upadhyay-a23491326_heres-a-quick-walkthrough-of-our-iot-based-ugcPost-7457118015705231361-i7dE?utm_source=share&utm_medium=member_desktop&rcm=ACoAAFJL9XsBwGK-CF5UpRQNf6Fz2qoehhFEAW4

The video includes:
- Hardware explanation
- Sensor integration
- Working demonstration
- Cradle movement
- LCD monitoring
- Fan automation

---

## Project Structure

```bash
Smart-Cradle-System/
│
├── images/
│   ├── image1.jpeg
│   └── image2.jpeg
│
├── smart_cradle.ino
├── README.md