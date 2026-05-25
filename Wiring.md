## Pin Mapping

| Component | Component Pin | ESP32-S3 GPIO |
| :--- | :--- | :--- |
| **BME688 Sensor** | SCL | **GPIO 4** |
| | SDA | **GPIO 5** |
| **Waveshare 2.4" LCD**| MOSI | **GPIO 11** |
| | SCLK / CLK | **GPIO 12** |
| | CS | **GPIO 10** |
| | DC | **GPIO 9** |
| | RST | **GPIO 14** |
| | BL | **GPIO 21** |
| **Noctua Fan** | PWM Signal | **GPIO 15** |
| | Tachometer| **GPIO 16** |
| **Up Button** | Prong 1 | **GPIO 6** |
| **Down Button**| Prong 1 | **GPIO 7** |

## Power Rail

* **Main Input:** 12V DC Barrel Jack → 12V Heavy-Duty Rocker Switch (Hard Cut)
* **High-Power Rail (12V):** Feeds Noctua Industrial Fan (+) and LM2596 Buck Converter (IN+)
* **Logic-Power Rail (5V):** LM2596 (OUT+) → ESP32-S3 (5V Pin) to power the microcontroller.
* **Sensor/Screen Rail (3.3V):** Powered by the ESP32-S3 3.3V regulator output pins.