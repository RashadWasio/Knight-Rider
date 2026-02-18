# Knight Rider LED Chaser with Speed Control

## 📌 Project Overview
This project implements a **Knight Rider–style LED chaser effect** using **Arduino**.  
A sequence of LEDs lights up from left to right and then reverses direction, creating a continuous scanning effect.  
The speed of the animation is controlled in real time using a **potentiometer**.

This project is ideal for:
- Beginners in Arduino and embedded systems
- Learning arrays and loops
- Understanding analog input and mapping
- LED animation and timing control

---

## ⚙️ Components Used
- Arduino Uno
- 12 × LEDs
- 12 × Current-limiting resistors (220Ω–330Ω)
- Potentiometer (10kΩ recommended)
- Breadboard
- Jumper wires

---

## 🔌 Pin Configuration
### LED Connections
| LED | Arduino Pin |
|----|------------|
| LED 1 | 2 |
| LED 2 | 3 |
| LED 3 | 4 |
| LED 4 | 5 |
| LED 5 | 6 |
| LED 6 | 7 |
| LED 7 | 8 |
| LED 8 | 9 |
| LED 9 | 10 |
| LED 10 | 11 |
| LED 11 | 12 |
| LED 12 | 13 |

### Potentiometer
- Middle pin → **A0**
- Other two pins → **5V** and **GND**

---

## 🧠 Working Principle
1. Arduino reads the potentiometer value using the analog pin **A0**
2. The value is mapped to a delay range that controls LED speed
3. LEDs turn ON sequentially from pin 2 to 13
4. The sequence reverses direction to create the Knight Rider effect
5. The process repeats continuously

---

## 💻 Software & Logic
- Platform: **Arduino IDE**
- Language: **Arduino C/C++**
- Key concepts used:
  - Arrays for LED pin management
  - `for` loops for forward and backward scanning
  - `analogRead()` for speed control
  - `map()` for delay adjustment

---

## 🧪 Testing & Usage
- Rotate the potentiometer to adjust LED movement speed
- Clockwise rotation increases delay (slower movement)
- Counterclockwise rotation decreases delay (faster movement)

---

## 🚀 Future Improvements
- PWM brightness fading instead of simple ON/OFF
- Using `millis()` instead of `delay()` for non-blocking control
- Sound-reactive LED effect
- Shift register (74HC595) to reduce pin usage

---

## 👤 Author
**Rashad Wasio**  
Arduino Knight Rider LED Project

---

## 📜 License
This project is for **educational purposes**.  
You are free to use, modify, and share this project with proper credit.
