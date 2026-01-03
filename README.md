# nostd ESP32C3 Blinky
A bare metal blinking led for ESP32-C3 microcontroller using Rust's no_std environment, simulated on wokwi
## Prerequisites
- Rust Toolchain: Stab=le rust with ESP32_C3 target
- espup 9ESP-IDF Rust Installer)
- espflash (Flashing tool)
- wokwi account
## Hardware Requirements 
- ESP32-C3 board
- USB-C CABLE
- LED connected on GPIO4 or onboard LED
## Setup
1. Create new project
2. Configure cargo.toml
### Building and flashing
1. Build the project: cargo build --release
2. Flash to ESP32-C3 :espflash flash --monitor target/risc32imc-unknown-none-elf/release/blinking-led-esp32c3
## Overview
The main code (main.rs) handles 
- GPIO configuration for LED pin
- Delay loop for blinking
### LED pin
The LED was connected on GPIO4 pin.

This is a nostd project. Delay is implemented as a simple loop. For non-blocking delays, consider using timer peripherals.

## Useful resources
- esp-rs Book
- esp32c3-hal Documentation
- wokwi documentation
## Contributing
1. Fork the repository
2. Create a feature branch
3. Submit a pull request



