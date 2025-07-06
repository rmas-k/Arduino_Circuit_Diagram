COD: 
int buttons[3] = {2, 3, 4};
int leds[3] = {8, 9, 10};

void setup() {
    for (int i = 0; i < 3; i++) {
        pinMode(buttons[i], INPUT_PULLUP);
        pinMode(leds[i], OUTPUT);
    }
}

void loop() {
    for (int i = 0; i < 3; i++) {
        int state = digitalRead(buttons[i]);
        digitalWrite(leds[i], !state);
    }
}

/////////

# 🔌 Arduino Circuit Diagram

This repository contains the circuit design files and Arduino code for a basic smart circuit project.

---

## 📁 Files Included

- Arduino-Circuit-Diagram.pdf – Visual representation of the circuit.
- Arduino-Circuit-Diagram.xml – File exported from the circuit design tool (Tinkercad or similar).
- code.ino – Arduino source code (to be added).

---

## 💡 Project Idea

This project is designed to control electronic components using Arduino.  
When a specific action is detected (such as motion or a button press), the circuit responds by activating an LED or another connected component. The goal is to demonstrate how sensors and outputs can be used together in an Arduino-based setup.

---

## 🔧 Components Used

- Arduino UNO  
- Breadboard  
- Jumper wires  
- LED  
- Resistor (220Ω)  
- Push button / sensor (optional)

---

## ⚙️ How It Works

1. The Arduino receives input from a sensor (or button).
2. Based on the input, the Arduino executes a code that controls the output.
3. For example, when the button is pressed, the LED lights up for a few seconds.

---

## 🧠 Tools Used

- Tinkercad – for designing the circuit diagram.  
- Arduino IDE – for writing and uploading the Arduino code.

---

## 📸 Circuit Diagram

View the file Arduino-Circuit-Diagram.pdf for the full layout of the circuit.  

---

## 📌 Notes

This is a simple educational project to demonstrate the use of Arduino in basic automation and electronics control. It can be expanded by adding more sensors, outputs, or logic conditions.

---
