**Project HAI-Helmet-Based Accident Indicator System**

This smart helmet system integrates various modules to ensure real-time accident detection, notification, and data capture. Below are the key features and the components used:

### 1. **Accident Detection & Alert System:**
   - **Phone Call Alert:** Upon detecting an accident, the system uses a **GSM Module 800A** to initiate **three consecutive phone calls** to a pre-set contact, alerting them of the incident.
   - **Location Sharing:** The system uses a **GPS NEO 6M** module to send the rider's **current location** along with the phone call alerts, allowing immediate identification of the accident spot.

### 2. **Accelerometer for Accident Detection:**
   - The system relies on an **ADXL345 Accelerometer Sensor** to detect sudden impacts or unusual movement patterns indicative of an accident. When a threshold is crossed, the system triggers the alert and recording functions.

### 3. **QR Code for Rider Information:**
   - A **QR code** is placed on the helmet, which can be scanned to access **basic details** about the rider, such as their name, emergency contacts, and medical information. This helps emergency responders identify the rider quickly.

### 4. **On-Helmet Camera:**
   - An **ESP32-CAM Module** is mounted on the helmet to continuously capture photos. These images are stitched together to create a video, providing a visual record of the accident. This helps in **determining the cause of the accident** and **identifying any mistakes** made by the involved parties.

### 5. **Control System:**
   - The system is powered by an **Arduino Mega 2560**, which manages the integration of all modules, including accident detection, alert triggers, and data transmission.

### Benefits:
   - **Immediate Response:** The GSM module ensures quick communication, while the GPS and camera modules provide crucial data for accident analysis and rider identification.
   - **Accident Analysis:** The camera footage, along with location and accelerometer data, helps in reconstructing the accident scenario.
This modular design improves the overall safety of riders by providing timely alerts and relevant data to ensure faster responses during accidents.
