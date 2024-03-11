# TFSIK01 Telemetry Modem

### Overview

The [TFSIK](https://github.com/ThunderFly-aerospace/TFSIK01/) represents a cutting-edge advancement in UAV telemetry solutions, offering dual antenna diversity and exceptional noise immunity. Developed as open-source hardware, it integrates the latest Si10xx series chip, the [Si1060](https://www.silabs.com/wireless/proprietary/si10xx-sub-ghz-mcps/device.si1060), and is complemented by the [Si4463 EZRadioPRO](https://www.silabs.com/wireless/proprietary/ezradiopro-sub-ghz-ics) Transceiver for robust communication capabilities. Designed with a focus on resistance to out-of-band frequency jamming, the TFSIK01 ensures reliable operation even in environments with signal interference, making it an ideal choice for UAV applications requiring high levels of data integrity and security.

### Key Features

- **High Noise Immunity**: Enhanced by a hardware-based RF front design, it operates effectively near out-of-band signal jammers.
- **Hardware Design**: Encased in a customizable 3D printed box with electromagnetic shielding, ensuring durability and adaptability.
- **Antenna Diversity**: Supports dual external antennas via MCX connectors, offering flexibility across various frequency bands, by default optimized for 433 MHz. 
- **Advanced Communication Technologies**:
  - Frequency-Hopping Spread Spectrum (FHSS)
  - Adaptive Time Division Multiplexing (TDM)
  - Support for Listen Before Talk (LBT) and Adaptive Frequency Agility (AFA)
- **High Performance**:
  - Transparent serial link
  - Air data rates up to 250kbps
  - MAVLink protocol framing and status reporting
  - Effective range of several kilometers with a small whip antenna
- **Open Source and Configurable**: Equipped with SiK firmware, it offers customizable settings via AT and RT commands, supporting MAVLink 2 protocol and available for multiple frequency bands.

### Applications

The TFSIK01A is specifically designed for UAV command and control applications, ensuring reliable, long-distance communication between the UAV and the ground control station. It also serves effectively in ROS2 environments for robotics, providing a dependable long-range wireless datalink.

### Installation and Configuration

The modem can be easily integrated into UAV systems, requiring a Pixhawk compatible JST-GH UART link for connection. External antennas are attached through MCX connectors, with optimal placement essential for achieving the best performance.

#### Connecting to Autopilot

The TFSIK01 modem is connected to the autopilot through a JST-GH cable with a 6-pin connector. By default, PX4 autopilot systems expect the telemetry data link to be connected to the TELEM1 port. However, after configuring the necessary parameters within the PX4 firmware, the modem can be connected to any available UART port.

#### Connecting to a Ground Station

##### Direct UART Connection

The TFSIK01 can be directly connected to a ground station using its UART interface. This capability allows for straightforward integration with Raspberry Pi or similar one-board computers (OBC) that have 3.3V UART pins available. The direct UART connection is particularly useful for setups requiring minimal latency and direct control over the data link.

##### Connection to USB

For setups requiring connection to a computer, a USB to UART converter is necessary. The [TFUSBSERIAL01](https://github.com/ThunderFly-aerospace/TFUSBSERIAL01) module is specifically designed for this purpose, featuring an FTDI VCP circuit for reliable data transmission. It includes a USB-C connector, for connection to computers or mobile devices, and a UART JST-GH connector for direct connection to the TFSIK01 modem.

This setup ensures that the modem can be utilized in diverse operational environments, from desktop-based ground control stations to field-deployable systems with embedded computers.

### Where to Buy

The TFSIK01A modem can be purchased directly from the developer and manufacturer, [ThunderFly](https://www.thunderfly.cz/). To inquire about purchasing, please contact ThunderFly via [email](mailto:info@thunderfly.cz). Additionally, the modem is available for online purchase through the [Tindie marketplace](https://www.tindie.com/products/thunderfly/).


### Frequency Options

By default, ThunderFly offers the TFSIK01A modem configured for the [433 MHz band](https://en.wikipedia.org/wiki/ISM_radio_band). However, if there is a need for operation on a different frequency, ThunderFly is capable of modifying the modem to accommodate various frequency requirements. About possibilities of frequency customization, please contact ThunderFly directly at [info@thunderfly.cz](mailto:info@thunderfly.cz) for more detailed information.

:::note
Before using the modem, always ensure that it complies with local conditions and laws regarding the operation of your selected frequency band. Additionally, verify whether you need any specific permissions or licenses to operate the device in your area.
:::
