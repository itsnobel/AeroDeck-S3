# AeroDeck-S3
ESP32-S3 &amp; CC1101 based portable wireless security auditing &amp; RF analysis tool.

October 6, 2026: Day 1 - Research, Feasibility & Component Selection
Session Summary:

Started the AeroDeck-3S project from absolute scratch! Since I am new to custom PCB design and RF hardware, I spent today's entire session understanding the core mechanics of the project. I brainstormed the project scope, compared ESP32-S3 against other controllers (like Flipper Zero's STM32), and finalized the Bill of Materials (BOM).

Key Learnings & Progress:

Understood how the ESP32-S3 serves as the main brain, running dual-core Wi-Fi/BLE processing alongside SPI and I2C peripherals.

Researched the CC1101 Sub-1GHz RF module to learn how it captures and transmits 315/433/868/915 MHz radio waves.

Designed the power architecture: USB Type-C ➔ TP4056 Battery Charger ➔ 3.3V LDO Voltage Regulator.

Decided on adding a 6-pin expansion header (UART/I2C) for future add-ons like GPS, I2S Microphones, or Speakers.

No physical PCB traces drawn yet, but gained 80%  clarity on component selection and schematic architecture.

October 7, 2026: Day 2 - Deep Dive into ESP32-S3 Pinouts & Module Workflows
Session Summary:

Dedicated today's session entirely to technical learning and understanding module compatibility via YouTube tutorials and technical documentation. Focus was placed on mapping out the ESP32-S3 architecture and making sure I don't accidentally assign peripheral functions to restricted or strapping pins.

Key Learnings & Progress:

Researched ESP32-S3 GPIO allocations: learned which pins are safe for general use, which are dedicated for flash/PSRAM, and which pins support native hardware SPI/I2C.

Studied power regulations and voltage requirements for individual modules (ensuring 3.3V tolerance on CC1101 and OLED).

Explored code upload workflows, USB-to-UART bridging versus Native USB flashing on the ESP32-S3, and basic firmware structure for driving the CC1101 transceiver.

No schematic drawing started in this session, but built the technical groundwork required before launching EasyEDA.

Time spent this session: 2.5 hours


