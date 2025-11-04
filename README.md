# STM32F401 Black Pill SPI Driver

A custom SPI driver for the STM32F401 Black Pill microcontroller with support for full-duplex communication, hardware slave management, and configurable SPI speed. Includes a timer library for precise delay functionality using General Purpose Timer 2.

---

## File Structure

- **main.c**
  - Sample script demonstrating SPI communication with MPU9250 IMU sensor
  - SPI frame size: 16 bits

- **SPI.h / SPI.c**
  - Custom SPI driver implementation
    - Full-duplex operation
    - Hardware slave management
    - SPI baud rate configurable (default: HSI/64; modify using BR[2:0] bits in SPI1_CR1 register)

- **Timer.h / Timer.c**
  - Timer library for delays
    - Uses General Purpose Timer 2

---

## Features

- Full-duplex SPI communication
- Hardware slave management
- Flexible SPI speed via register configuration
- Accurate delays using hardware timer


