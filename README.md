# G-Board

This project consists of two components: the **G-Base** and the **G-Board**, currently in the version **G-Board-G070**, featuring the **STM32G070CBT6** microcontroller.

---

## Project Structure

### G-Base (Base Board)

The G-Base provides the following components and interfaces:

- 4 tactile push buttons  
- 4 LEDs  
- UART to USB bridge  
- 2 analog potentiometers  
- PI filter for clean analog power supply  
- USB interface  
- SWD programming/debug interface  
- BOOT0 and RESET signals are handled via the G-Base

### G-Board-G070 (Controller Board)

The controller board features:

- STM32G070CBT6 microcontroller  
- 8 MHz crystal oscillator  
- 32.768 kHz crystal (for RTC and low-power operation)  
- All GPIOs are routed through headers and made accessible via the G-Base

---

## Images

Images of the boards are located in the `/Pictures` directory.

### G-Base

![G-Base Isometric](/Pictures/G-Base_1_isometric.JPEG)  
*G-Base – Isometric View*

![G-Base Top View](/Pictures/G-Base_1.JPEG)  
*G-Base – Top View*

### G-Board

![G-Board G070](/Pictures/G-Board_G070.JPEG)  
*G-Board-G070 – Controller Board*

---

## Notes

- The **BOOT0** and **RESET** signals are controlled via the G-Base for easier firmware uploading and debugging.
- The PI filter ensures a clean analog voltage supply, especially useful when working with ADC inputs or analog sensors.
