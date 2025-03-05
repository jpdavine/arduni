# arduni
arduino board url
https://arduino.esp8266.com/stable/package_esp8266com_index.json

# ESP8266 LittleFS Uploader Tool
## Installation Instructions:
1. Download this tool from this repository.
2. Place it in the Arduino tools folder:
3. Restart Arduino IDE.
4. You will now see **"ESP8266 LittleFS Data Upload"** under **"Tools"**.
Use this tool to upload **web files (HTML, CSS, JS, images, etc.)** to ESP-01 LittleFS.


# ESP8266 WebSockets Library

## Purpose:
This library enables **real-time communication** between the ESP8266 and a web interface using WebSockets.

## Installation:
1. Place this folder in:
2. Restart Arduino IDE.
3. You can now use:
```cpp
#include <WebSocketsServer.h>




# ESP8266_PWM Library

This repository contains the **ESP8266_PWM** library, which provides software-based PWM control for the **ESP8266** microcontroller.

## 📌 Features
- Software PWM for **ESP8266**, allowing control of motors, LEDs, and other PWM-based components.
- Works with **GPIO pins on ESP-01** and other ESP8266 modules.
- Supports **variable duty cycles** for smooth transitions.

## 📂 Installation
1. Download this repository as a ZIP file.
2. Extract it to your **Arduino libraries** folder:
3. Restart **Arduino IDE** and include the library in your sketch.

## 🔧 Usage Example
```cpp
#include <ESP8266_PWM.h>

#define PWM_PIN 2  // GPIO2 (Change if needed)

ESP8266_PWM pwm;

void setup() {
 pwm.setup(PWM_PIN, 1000, 50);  // Set 1kHz frequency, 50% duty cycle
}

void loop() {
 pwm.setDutyCycle(PWM_PIN, 75);  // Adjust to 75% duty cycle
 delay(1000);
 pwm.setDutyCycle(PWM_PIN, 25);  // Adjust to 25% duty cycle
 delay(1000);
}
