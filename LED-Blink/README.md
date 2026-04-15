# LED Blink using STM32

## 📌 Description
This project demonstrates how to blink an LED using an STM32 microcontroller. It is a basic embedded systems project used to understand GPIO configuration and delay generation.

## 🎯 Objective
- To learn GPIO output configuration
- To control an LED using STM32
- To understand basic embedded programming using HAL libraries

## 🛠️ Components Required
- STM32F103C8T6 (Blue Pill)
- LED
- Resistor (220Ω)
- Breadboard
- Connecting wires
- ST-Link Programmer

## ⚙️ Working Principle
The STM32 microcontroller is programmed to toggle a GPIO pin at a fixed interval. This causes the LED connected to that pin to turn ON and OFF repeatedly, creating a blinking effect.

## 🔌 Circuit Connections
- LED Anode (+) → GPIO Pin (e.g., PA5 or PC13)
- LED Cathode (−) → Resistor → GND

## 💻 Code Snippet

```c
HAL_GPIO_TogglePin(GPIOC, GPIO_PIN_13);
HAL_Delay(500);
