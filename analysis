# Technical Analysis & Security Discussion

## 1. Relationship Between RSSI and Distance
The Received Signal Strength Indicator (RSSI) is measured in decibels (dBm). In our data, we observed a non-linear relationship where the signal drops off sharply as distance increases. This follows the **Log-Distance Path Loss Model**:

$$P(d) = P(d_0) - 10n \log_{10}\left(\frac{d}{d_0}\right)$$



In the **Room** scan, the RSSI was **-67 dBm** (Strong), while in the **Corridor**, it dropped to **-91 dBm** (Very Weak). This confirms that physical distance is the primary factor in signal degradation.

## 2. Environmental Factors
* **Physical Obstructions:** In the Kitchen environment, appliances likely caused signal attenuation.
* **Environmental Noise:** 2.4 GHz interference from other devices (Wi-Fi, Microwaves) can cause "jitter" in RSSI values, leading to inconsistent distance estimations.

## 3. Security and Privacy Reflections

### Potential Risks
* **Device Tracking:** BLE devices broadcast their presence continuously. A static MAC address allows third parties to track a user's habits and location without consent.
* **Identifier Exposure:** The scan revealed names like "JEREMIAH'S Samsung." This is a privacy leak that associates a physical person with a specific device.
* **Passive Scanning:** Attackers can "sniff" BLE packets silently. Unlike classic Bluetooth, BLE does not always require a "pairing" handshake to be visible, making it vulnerable to data harvesting.

## 4. Final Conclusion
While BLE is essential for the IoT ecosystem due to its low power consumption, it lacks inherent privacy by design. Users should rename their devices to generic terms and manufacturers should implement aggressive MAC randomization to protect user anonymity.
