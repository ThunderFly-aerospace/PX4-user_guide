
# ThunderFly TFHT01 Hygrometer

The ThunderFly TFHT01 is open-source a high-precision hygrometer designed specifically for aviation applications. It offers fast response times and high durability, making it an ideal choice for integration into various aviation systems.

## Key Features:
- **High Precision:** Equipped with the SHT35 sensor for accurate humidity and temperature measurements.
- **Fast Response Time:** Enhanced with a thin PCB and minimal thermal conductivity for rapid adaptation to environmental changes.
- **Durable Casing:** Encased in a robust plastic housing to withstand mechanical stress and harsh conditions.


## Specifications

- **Sensor Type:** SHT35
- **Measurement Range:** 0% to 100% RH (humidity), -40°C to 125°C (temperature)
- **Accuracy:** ±1.5% RH, ±0.2°C
- **Response Time:** Fast adaptation to environmental changes due to minimal thermal mass and efficient PCB design
- **Power Supply:** 5V DC
- **Interface:** I2C pixhawk compatibile

## User Manual

##### 1. Sensor Overview

The TFHT01 hygrometer consists of a high-precision SHT35 sensor mounted on a thin PCB, encased in a durable plastic housing. The sensor is designed for easy integration with autopilot systems, providing reliable humidity and temperature data.

##### 2. Connecting to Autopilot

To connect the TFHT01 sensor to a Pixhawk-compatible autopilot:
1. Use the provided 4-pin JST-GH cable.
2. Connect the cable to the I2C port on the autopilot.
3. Upon powering the autopilot, a green LED on the sensor will illuminate, indicating power availability.

##### 3. Mounting Methods

Given its compact size and lightweight design, the TFHT01 can be easily mounted on a drone. Recommended methods include:
- Velcro strips
- Zip ties
- Double-sided adhesive tape

##### 4. Maintenance and Handling

To ensure the longevity and accuracy of the TFHT01 sensor:
- Avoid exposing the sensor to extreme mechanical stress.
- Regularly check the connections and casing for any signs of wear or damage.
- If removal from the casing is necessary, unscrew the two screws, gently press the exposed edge of the PCB near the sensor with a flat object, and carefully slide it out towards the connector.

