# WPT_ELECTROINC_WORKSHOP # 

## 🔌 ESP8266 Pinout & Explanation  

The **ESP8266** is a low-cost Wi-Fi microchip with full TCP/IP stack and microcontroller capability. It is widely used in **IoT projects**, **smart devices**, and **wireless automation**.  

### 📍 Pinout Diagram (NodeMCU ESP8266 Example)  
<img width="238" height="141" alt="image" src="https://github.com/user-attachments/assets/115e7ede-e98c-4477-8f01-00f78a711692" />


| Pin Name | GPIO No. | Function | Notes |
|----------|----------|----------|-------|
| D0       | GPIO16   | Digital I/O | No PWM, no interrupts |
| D1       | GPIO5    | Digital I/O, I2C (SCL) | Can be used for I2C |
| D2       | GPIO4    | Digital I/O, I2C (SDA) | Can be used for I2C |
| D3       | GPIO0    | Digital I/O | Pull-up needed at boot |
| D4       | GPIO2    | Digital I/O, Built-in LED | Pull-up at boot |
| D5       | GPIO14   | Digital I/O, SCLK | Commonly used for SPI |
| D6       | GPIO12   | Digital I/O, MISO | Commonly used for SPI |
| D7       | GPIO13   | Digital I/O, MOSI | Commonly used for SPI |
| D8       | GPIO15   | Digital I/O, CS | Pull-down at boot |
| RX       | GPIO3    | UART RX | Serial communication |
| TX       | GPIO1    | UART TX | Serial communication |
| A0       | Analog 0 | ADC (0–1V input) | Only **one analog pin** |
| GND      | –        | Ground | Connect to GND |
| 3V3      | –        | Power (3.3V) | Do NOT use 5V directly |
| VIN      | –        | Power Input (5V) | Onboard regulator to 3.3V |

---

### ⚡ Key Notes
- **Operating Voltage**: 3.3V (⚠️ do not supply 5V directly to pins).  
- **Digital Pins**: Most GPIOs support **PWM, I2C, SPI, UART**.  
- **Boot Restrictions**: GPIO0, GPIO2, and GPIO15 affect boot mode (must be pulled high/low accordingly).  
- **Analog Pin**: Only **1 analog input (A0)** with a 10-bit resolution (0–1023).  
- **Flash & Reset**: Some pins are reserved internally, so not all GPIOs are free for general use.


<img width="1407" height="766" alt="image" src="https://github.com/user-attachments/assets/87f43e9d-5c90-41b6-a2a3-1458b56c3710" />

