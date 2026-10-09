# STM32G431 + DRV8323 Brushless DC Motor ESC – PCB Design

A complete 4-layer STM32G431-based brushless DC motor electronic speed controller designed from the ground up in KiCad.

The design covers schematic architecture, component selection and validation, footprint assignment, net-class definition, impedance-controlled routing rules, and 3D board verification.

## Highlights

- **Power architecture** — Multi-stage buck conversion (12 V → 5 V → 3.3 V) with proper sequencing and filtering for the MCU and gate driver
- **Gate driver & power stage** — DRV8323S smart gate driver (SPI configuration, complementary PWM, integrated current-sense amplifiers) driving parallel CSD19503KCS MOSFETs
- **Current & voltage sensing** — Precision low-side current sensing (INA180 + 1 mΩ shunts) and battery voltage monitoring for closed-loop control and protection
- **Fault handling & communication** — nFAULT, over-current and thermal protection plus CAN and UART interfaces
- **Net-class system** — Dedicated classes for high-current power, 85–100 Ω differential pairs, and controlled-impedance high-speed signals
- **Layout** — Optimised for EMI reduction, return-path integrity, and thermal performance under continuous 40–50 A loads

