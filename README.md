# Sonoff SNZB-02P Driver for Hubitat

## Overview
This custom driver is designed for the **Sonoff SNZB-02P** Zigbee temperature and humidity sensor, allowing seamless integration with the Hubitat Elevation platform. With this driver, you can unlock advanced capabilities, configure reporting intervals, and monitor device presence in real time.

---

## Features
- **Temperature and Humidity Reporting**:
  - Accurate and configurable measurement reporting for both temperature and humidity.
  - Define minimum and maximum reporting intervals and change thresholds.

- **Battery Level Monitoring**:
  - Displays the battery percentage of your Sonoff SNZB-02P sensor.
  - Configurable reporting intervals to optimize performance and battery life.

- **Presence Detection**:
  - Monitors the sensor's activity and triggers a **presence** state.
  - Marks the sensor as "not present" after consecutive failed recovery attempts.

- **Configurable Recovery Mechanism**:
  - Automatically attempts to recover the sensor if it fails to report data.
  - Define how many recovery attempts are allowed before marking the device as "not present."

- **Flexible Configuration**:
  - Customizable preferences for:
    - Temperature reporting intervals and change thresholds.
    - Humidity reporting intervals and change thresholds.
    - Battery reporting intervals and thresholds.
    - Recovery interval (time between recovery checks).
    - Presence trigger (number of failed recovery attempts).

- **Comprehensive Logging**:
  - Debug logging to monitor the driver's activity and interactions with the sensor.

---

## How to Use

### Install the Driver
1. Copy the driver code from this repository.
2. Log into your Hubitat Elevation hub and navigate to **Drivers Code** > **New Driver**.
3. Paste the code and save it.

### Pair the Sonoff SNZB-02P Sensor
1. Put your sensor into pairing mode and add it to Hubitat.
2. Assign the **Sonoff SNZB-02P Driver** to the device.

### Configure Preferences
1. Open the device settings in Hubitat.
2. Adjust the preferences for temperature, humidity, battery reporting, and recovery intervals to suit your needs.

---

## Device States and Attributes
- **Temperature**: Current temperature reported by the device (°C).
- **Humidity**: Current relative humidity (%).
- **Battery**: Remaining battery level (%).
- **Presence**: Indicates whether the device is "present" or "not present."

---

## Advanced Configuration
- **Recovery Interval**: Set how often the device should check for activity.
- **Presence Trigger**: Define the number of failed recovery attempts allowed before marking the device as "not present."
- **Custom Reporting Thresholds**: Optimize performance by adjusting reporting intervals and thresholds for temperature, humidity, and battery.

---

## Requirements
- Hubitat Elevation Hub (C-5, C-7, or later).
- Sonoff SNZB-02P Zigbee temperature and humidity sensor.

## HPM
It is better to add this driver via HPM
Open the Hubitat Package Manager app in your Hubitat hub.
Go to Repositories > Add a Repository.
Enter the URL to repository file
https://raw.githubusercontent.com/Bitikus/Sonoff-SNZB-02P-Driver/main/repository.json


---

## Contributing
Contributions are welcome! If you have suggestions, feature requests, or bug reports, feel free to open an issue or submit a pull request.

---

## License
This project is licensed under the [MIT License](LICENSE). You are free to use, modify, and distribute this software.
