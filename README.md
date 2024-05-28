# Smart Plant Care using the VSD_Squadron-MINI-BOARD

## Introduction
The "Smart Plant Care" project is an innovative IoT solution aimed at optimizing plant growth by monitoring essential environmental parameters. By leveraging advanced sensors and microcontrollers, our system measures the humidity and temperature of the atmosphere, as well as the moisture content of the soil. This information is crucial for maintaining optimal plant health and growth. The project addresses the increasing need for efficient plant care in both residential and agricultural settings, ensuring that plants receive the right amount of water at the right time.

## Overview
The Smart Plant Care system operates through a network of interconnected components that work together to provide real-time monitoring and automated watering solutions. The user can remotely monitor the plant’s environment and adjust the soil moisture threshold via a WiFi-connected interface. When the soil moisture level falls below the set threshold, the system automatically activates a water pump to deliver the necessary amount of water to the plant. This process helps in conserving water and ensuring that the plant remains healthy.

### User Flow
1. **Data Collection**: Sensors measure temperature, humidity, and soil moisture levels.
2. **Data Transmission**: The CH32V003F4U6 microcontroller collects data from the sensors and sends it to the ESP-01S ESP8266 WiFi Module.
3. **Remote Monitoring**: The ESP8266 transmits the data over WiFi, allowing the user to monitor real-time conditions through a web interface.
4. **Threshold Setting**: Users can set and adjust the soil moisture threshold via the web interface.
5. **Automated Watering**: When soil moisture falls below the threshold, the system activates the water pump to irrigate the plant.

### How It Works
1. **Sensor Data Acquisition**: The DHT11 sensor measures atmospheric temperature and humidity, while the soil moisture sensor checks the soil's moisture level.
2. **Data Processing**: The CH32V003F4U6 microcontroller processes the sensor data and determines if the soil moisture is below the user-defined threshold.
3. **Data Transmission**: Processed data is sent to the ESP-01S ESP8266 WiFi module, which transmits it to the user's web interface for real-time monitoring.
4. **Automated Response**: If the soil moisture is below the threshold, the microcontroller activates the water pump through a switch to irrigate the plant.
5. **User Interaction**: The user can monitor real-time data, set moisture thresholds, and control the watering system remotely via the web interface.

## Components Required
- **CH32V003F4U6 Microcontroller**: Acts as the central processing unit, managing sensor data and system operations.
- **ESP-01S ESP8266 WiFi Module**: Facilitates wireless communication, allowing remote data monitoring and control.
- **DHT11 Temperature and Humidity Sensor**: Measures atmospheric temperature and humidity.
- **Soil Moisture Sensor Module**: Detects the moisture content in the soil.
- **Water Pump**: Provides irrigation to the plant when needed.
- **Switch**: Manages the on/off states of the water pump.

## Circuit Connection Diagram
![Circuit Diagram]([Circuit_Diagram.png](https://github.com/1kushagra2/Smart-Plant-Care/blob/main/Smart%20Plant%20Care/Circuit_Diagram.jpg))

### Table For Pin Configuration

## Conclusion
The Smart Plant Care project integrates advanced IoT technology to provide an efficient and automated plant care system. By ensuring that plants receive the optimal amount of water based on real-time environmental data, this system enhances plant health and growth while conserving resources. With remote monitoring and control capabilities, users can manage their plants effortlessly, making Smart Plant Care a valuable tool for both hobbyists and professional growers.
