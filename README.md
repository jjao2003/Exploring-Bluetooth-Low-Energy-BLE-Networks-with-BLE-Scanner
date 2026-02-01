# Exploring Bluetooth Low Energy (BLE) Networks with BLE Scanner

## Course Assignment – Wireless / Mobile Networks  
**Exercise:** 3.3  
**Student:** Agozie Joel Onuigbo  
**Tool Used:** BLE Scanner (Android)  
**Submission:** GitHub Repository Link (via Moodle)

---

## 1. Objective

The objective of this exercise is to investigate nearby Bluetooth Low Energy (BLE)
devices and analyze their characteristics in different environments. The experiment
focuses on observing signal strength (RSSI), device visibility, and environmental
effects, while also reflecting on BLE security and privacy implications.

---

## 2. Tools and Experimental Setup

### 2.1 Hardware and Software
- **Smartphone:** Android device
- **Application:** BLE Scanner (Android)
- **Bluetooth:** Enabled
- **Location Services:** Enabled (required for BLE scanning)
- **Scan Mode:** Continuous scan

### 2.2 Measurement Procedure
- Each environment was scanned for approximately **2–3 minutes**
- Device RSSI values were observed and recorded
- Screenshots were taken to document scan results
- Data was collected without pairing to any BLE device

---

## 3. Scanning Environments

### 3.1 Room
- Indoor personal room
- Presence of smartphone, smartwatch, wireless earbuds
- Enclosed space with walls and furniture
- Moderate electronic interference

### 3.2 Kitchen
- Indoor shared space
- Presence of smart appliances and multiple smartphones
- Increased reflections from metallic surfaces
- Moderate human movement

### 3.3 Corridor
- Indoor hallway connecting rooms
- Fewer stationary devices
- Longer open space with fewer obstructions
- Lower device density compared to room and kitchen

---

## 4. Collected BLE Scan Data

### 4.1 Room Scan Results

| Device Name        | RSSI (dBm) | MAC Address / ID     | Estimated Device Type |
|--------------------|------------|----------------------|-----------------------|
| Galaxy Watch       | -42        | A4:7D:3F:XX:XX:01    | Wearable              |
| Redmi Buds         | -50        | B9:21:AC:XX:XX:02    | Audio Device          |
| Unknown Device     | -71        | Randomized           | Smartphone            |
| BLE Beacon         | -65        | C1:9A:7D:XX:XX:03    | IoT / Beacon          |

---

### 4.2 Kitchen Scan Results

| Device Name        | RSSI (dBm) | MAC Address / ID     | Estimated Device Type |
|--------------------|------------|----------------------|-----------------------|
| Smart TV           | -55        | D8:4E:12:XX:XX:04    | Smart Appliance       |
| Samsung Phone      | -60        | Randomized           | Smartphone            |
| Fitness Tracker    | -48        | E2:8B:9F:XX:XX:05    | Wearable              |
| Unknown Device     | -78        | Randomized           | IoT / Phone           |

---

### 4.3 Corridor Scan Results

| Device Name        | RSSI (dBm) | MAC Address / ID     | Estimated Device Type |
|--------------------|------------|----------------------|-----------------------|
| Smartphone         | -67        | Randomized           | Smartphone            |
| BLE Beacon         | -72        | F3:19:7A:XX:XX:06    | Beacon                |
| Unknown Device     | -85        | Randomized           | Distant BLE Device    |

---

## 5. Screenshots

Screenshots of each scan environment are provided in the `screenshots/` directory:
- `room_scan.png`
- `kitchen_scan.png`
- `corridor_scan.png`

Each screenshot clearly shows detected BLE devices and their RSSI values.

---

## 6. Analysis and Observations

### 6.1 RSSI and Estimated Distance

RSSI values provide an approximate indication of the distance between the scanning
device and BLE transmitters. Devices with RSSI values closer to 0 dBm (e.g., −40 dBm)
were physically closer, while devices with values below −80 dBm were either farther
away or obstructed by walls or other objects.

RSSI is influenced by environmental factors and should not be interpreted as a
precise distance measurement.

---

### 6.2 Device Density Across Environments

The room environment showed the highest number of detectable BLE devices due to
personal electronics such as wearables and audio devices. The kitchen environment
exhibited moderate device density, while the corridor had the fewest detected devices.

This demonstrates how BLE device visibility depends strongly on human activity and
space usage.

---

### 6.3 Signal Fluctuations and Anomalies

Some devices exhibited fluctuating RSSI values even when stationary. This behavior
can be attributed to:
- Human movement
- Multipath signal propagation
- Interference from Wi-Fi networks
- Device power-saving mechanisms

---

## 7. Environmental and Transmission Factors

Physical obstructions such as walls, furniture, and human bodies attenuate BLE
signals. Indoor environments introduce additional interference from electronic
devices and wireless networks.

The corridor environment showed weaker RSSI values due to increased distance and
reduced line-of-sight visibility.

---

## 8. Security and Privacy Considerations

### 8.1 BLE Usage in Everyday Devices
BLE is commonly used in:
- Smartwatches and fitness trackers
- Wireless audio devices
- Smart home appliances
- IoT sensors and beacons

---

### 8.2 Security and Privacy Risks

Potential risks associated with BLE include:

- **Device Tracking:**  
  Static identifiers can allow long-term tracking of users.

- **Identifier Exposure:**  
  Advertising packets may leak device information.

- **Passive Scanning:**  
  BLE devices can be detected without user interaction or consent.

---

### 8.3 Mitigation Techniques

Modern devices mitigate these risks through:
- MAC address randomization
- Limited advertising payloads
- Permission-based access controls
- Reduced advertising intervals

---

## 9. Conclusions

This exercise demonstrated how BLE device detection and signal characteristics vary
across different indoor environments. RSSI values provide useful but approximate
insights into device proximity and are strongly influenced by environmental factors.

The experiment also highlighted the widespread adoption of BLE technology and the
importance of privacy-preserving mechanisms in modern wireless systems.

---

## 10. Repository Contents

