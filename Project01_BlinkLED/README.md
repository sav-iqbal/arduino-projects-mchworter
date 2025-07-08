# Project 01 – Blink LED

## 🔍 Description
This basic project turns an LED on and off repeatedly using the Arduino Uno’s digital output. It's the classic "Hello, World!" of embedded systems.

## 🎯 Objectives / Concepts Learned
- How to use `pinMode()` and `digitalWrite()`
- Using `delay()` for timing
- Understanding basic breadboarding and circuit wiring
- Running your first Arduino sketch

## 🛠️ Hardware Used
- Arduino Uno R3 (Elegoo)
- Breadboard
- 1x LED (any color)
- 220Ω resistor
- Jumper wires
- USB cable for power

## 🧠 How It Works
- Digital pin 13 is configured as an output
- The LED is wired in series with a resistor to GND
- The Arduino turns the LED on for 1 second, then off for 1 second, looping forever

## 🖼️ Circuit Diagram
![Blink LED Circuit](circuit_diagram.png)

## 💻 Code Snippet
```cpp
void setup() {
  pinMode(13, OUTPUT);
}

void loop() {
  digitalWrite(13, HIGH);   // turn the LED on
  delay(1000);              // wait for 1 second
  digitalWrite(13, LOW);    // turn the LED off
  delay(1000);              // wait for 1 second
}
