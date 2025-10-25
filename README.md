# STM32 Input Capture using TIM2 (STM32F446RE)

This project demonstrates **Input Capture mode** on the STM32F446RE microcontroller using **TIM2 Channel 1**.  
It measures the timer value when a rising edge occurs on the input pin.

---

## 🔧 Hardware Setup
- **MCU:** STM32F446RE (Nucleo Board)
- **Input Pin:** PA0 (TIM2_CH1)
- **Clock Source:** HSI (16 MHz)
- **Prescaler:** 15999 → Timer tick = 1 ms
- **Mode:** Input Capture (Rising Edge)

---

## 🧠 Functionality
- Starts Timer 2 in Input Capture interrupt mode.
- Captures the counter value at each rising edge.
- Stores live counter in variable `counter`.
- Captured value from interrupt stored in `capture`.

---

## 📂 Key Files
- `main.c` → Peripheral initialization and main loop.
- `stm32f4xx_it.c` → Interrupt handler for TIM2 capture.
- `main.h` → Function prototypes and includes.

---

## 🧰 Tools Used
- **STM32CubeIDE**
- **STM32CubeMX**
- **HAL Drivers**
- **C Language (C99)**

---

## ⚙️ How to Run
1. Open project in STM32CubeIDE.
2. Connect Nucleo-F446RE via USB.
3. Build and flash.
4. Monitor capture values via debugger or serial output.
