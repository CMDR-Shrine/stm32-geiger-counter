# Lesson 01 Notes: Meet the Machine

- apbr2 bus thing address offset: 0x0C
- RCC (reset and clock constrol) Boundary addr is: 0x4002 1000 - 0x4002 13FF
- Exact MCU marking: **STM32F103CBT6**
- Processor core: Arm® 32-bit Cortex®-M3 CPU core 
- Instruction set used by this project: Thumb instruction set
- Flash start address: 0x0800 0000 n [DS5319, §4 “Memory mapping”](<https://www.st.com/resource/en/datasheet/stm32f103c8.pdf>)
- Guaranteed flash size for the CB part: 128 Kbytes [DS5319, Table 2](<https://www.st.com/resource/en/datasheet/stm32f103c8.pdf>).  
- SRAM start address: its here s 0x2000 0000    [DS5319, Table 2](<https://www.st.com/resource/en/datasheet/stm32f103c8.pdf>) 
- SRAM size: 20Kbytes
- Initial clock source after reset: internal RC 8 MHz oscillator isselected as the default CPU clock on reset [DS5319, §2.3.7 “Clocks and startup](<https://www.st.com/resource/en/datasheet/stm32f103c8.pdf>)
- Initial clock frequency: 8Mhz [DS5319, §2.3.7 “Clocks and startup](<https://www.st.com/resource/en/datasheet/stm32f103c8.pdf>)
- Onboard LED pin: pc13
- Electrical level that turns the LED on: it needs 0 v.
    - 3.3 V > resistor > LED > PC13 > GPIO transistor > ground
    - pc13 is inside the cpu, its a transistor that can connect to ground



## docs

[DS5319: STM32F103x8/xB datasheet](https://www.st.com/resource/en/datasheet/stm32f103c8.pdf) 

[RM0008: STM32F10xxx reference manual](https://www.st.com/resource/en/reference_manual/cd00171190-stm32f101-103-105-107-stm32f100-series-armbased-32bit-mcus-stmicroelectronics.pdf) 
[PM0056: Cortex-M3 programming manual](https://www.st.com/resource/en/programming_manual/pm0056-stm32f10xxx20xxx21xxxl1xxxx-cortex-m3-programming-manual-stmicroelectronics.pdf) 
[ES096: STM32F103x8/B errata](https://www.st.com/resource/en/errata_sheet/es096-stm32f101x8b-stm32f102x8b-and-stm32f103x8b-mediumdensity-device-limitations-stmicroelectronics.pdf) 
[Common Blue Pill schematic](https://stm32-base.org/assets/pdf/boards/original-schematic-STM32F103C8T6-Blue_Pill.pdf) 

## Build observations

- ELF entry-point address:
- Address of `.isr_vector`:
- Initial stack-pointer value:
- Address of `Reset_Handler`:
- Address of `main`:# Lesson 01 Notes: Meet the Machine

- apbr2 bus thing address offset: 0x0C
- RCC (reset and clock constrol) Boundary addr is: 0x4002 1000 - 0x4002 13FF
- Exact MCU marking: **STM32F103CBT6**
- Processor core: Arm® 32-bit Cortex®-M3 CPU core 
- Instruction set used by this project: Thumb instruction set
- Flash start address: 0x0800 0000 n [DS5319, §4 “Memory mapping”](https://www.st.com/resource/en/datasheet/stm32f103c8.pdf)
- Guaranteed flash size for the CB part: 128 Kbytes [DS5319, Table 2](<https://www.st.com/resource/en/datasheet/stm32f103c8.pdf>).  
- SRAM start address: its here s 0x2000 0000    [DS5319, Table 2](<https://www.st.com/resource/en/datasheet/stm32f103c8.pdf>) 
- SRAM size: 20Kbytes
- Initial clock source after reset: internal RC 8 MHz oscillator isselected as the default CPU clock on reset [DS5319, §2.3.7 “Clocks and startup](<https://www.st.com/resource/en/datasheet/stm32f103c8.pdf>)
- Initial clock frequency: 8Mhz [DS5319, §2.3.7 “Clocks and startup](<https://www.st.com/resource/en/datasheet/stm32f103c8.pdf>)
- Onboard LED pin: pc13
- Electrical level that turns the LED on: it needs 0 v.
    - 3.3 V > resistor > LED > PC13 > GPIO transistor > ground
    - pc13 is inside the cpu, its a transistor that can connect to ground

## Build observations

- ELF entry-point address:
- Address of `.isr_vector`:
- Initial stack-pointer value:
- Address of `Reset_Handler`:
- Address of `main`:
