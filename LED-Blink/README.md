# LED Blink using STM32 (Built-in LED)

## 📌 Description
This project demonstrates blinking the onboard (built-in) LED of the STM32 microcontroller without using any external components.

## 🎯 Objective
- To understand basic GPIO output configuration
- To control the onboard LED using STM32
- To get started with embedded programming

## 🛠️ Hardware Used
- STM32F103C8T6 (Blue Pill)
- ST-Link Programmer

## ⚙️ Built-in LED Details
- The onboard LED is connected to **PC13**
- Logic is **inverted**:
  - LOW → LED ON
  - HIGH → LED OFF

## ⚙️ Working Principle
The microcontroller toggles the GPIO pin (PC13) at regular intervals. Since the LED is internally connected, it blinks without any external wiring.

## 💻 Code Snippet

```c
HAL_GPIO_WritePin(GPIOC, GPIO_PIN_13, GPIO_PIN_RESET); // LED ON
HAL_Delay(500);

HAL_GPIO_WritePin(GPIOC, GPIO_PIN_13, GPIO_PIN_SET);   // LED OFF
HAL_Delay(500);
