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

| Device Name        |  MAC Address / ID| Signal Strength (RSSI) |Estimated Distance |
|--------------------|------------------|------------------------|-------------------|
| TV | DE:23:4E:9D:C7:A1 | -87 dBm | 44.27 m |
| fhw2_fb943c34190... | 6D:68:5D:32:04:45 | -91 dBm | 59.95 m |
| N/A (Apple) | 4E:B0:21:7F:A3:F8 | -89 dBm | 51.07 m |
| N/A | 77:E1:9F:8E:2F:B4 | -76 dBm | 14.13 m |
| N/A | 61:0D:E3:1F:25:70 | -81 dBm | 21.41 m |
---

### 4.2 Kitchen Scan Results

| Device Name        |  MAC Address / ID| Signal Strength (RSSI) |Estimated Distance |
|--------------------|------------------|------------------------|-------------------|
| Philips 57944 | C1:DB:79:20:BD:1C | -75 dBm | 13.00 m |
| b1_E14PT33V_S1 | D0:E2:EE:9D:61:9F | -82 dBm | 24.16 m |
| N/A (Apple) | 26:93:17:73:96:D2 | -72 dBm | 10.00 m |
| N/A | 49:6F:11:00:83:8F | -85 dBm | 35.20 m |
| N/A | 65:42:C2:59:B5:14 | -81 dBm | 21.20 m |

---

### 4.3 Corridor Scan Results

| Device Name        |  MAC Address / ID| Signal Strength (RSSI) |Estimated Distance |
|--------------------|------------------|------------------------|-------------------|
| JEREMIAH'S Samsung | B1:E6:31:01:E3:6B | -67 dBm | 5.61 m |
| Philips 57945| C1:E4:71:E5:58:3B | -83 dBm | 28.31 m |
| N/A (Apple) | 4F:04:1E:22:96:B3 | -88 dBm | 46.27 m |
| N/A | 65:31:6C:51:B1:91 | -83 dBm | 28.31 m | 
| N/A | 45:65:21:A2:35:E2 | -81 dBm | 21.41 m |
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

