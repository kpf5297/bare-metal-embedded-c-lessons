# Bare-Metal Embedded C Lessons

![License](https://img.shields.io/github/license/kpf5297/bare-metal-embedded-c-lessons?style=flat-square)  
![GitHub Repo stars](https://img.shields.io/github/stars/kpf5297/bare-metal-embedded-c-lessons?style=flat-square)  
![GitHub forks](https://img.shields.io/github/forks/kpf5297/bare-metal-embedded-c-lessons?style=flat-square)  
![Last Commit](https://img.shields.io/github/last-commit/kpf5297/bare-metal-embedded-c-lessons?style=flat-square)  
![Issues](https://img.shields.io/github/issues/kpf5297/bare-metal-embedded-c-lessons?style=flat-square)

A collection of structured notes, code examples, and lessons learned while working through *Bare Metal Embedded C Programming: Develop High-Performance Embedded Systems with C for ARM microcontrollers*.  
This repo serves as both a personal learning log and a resource for others exploring ARM Cortex-M microcontrollers and bare-metal C programming.

---

## 📘 Book Reference
This repository is based on the concepts and exercises from *Bare Metal Embedded C Programming*.  
> ⚠️ Note: No copyrighted book content is reproduced. This is strictly a collection of personal notes, implementations, and insights.

---

## 📂 Repository Structure
```

/chapter01\_intro/       # Toolchain setup, first project
/chapter02\_registers/   # Register-level programming examples
/chapter03\_io/          # GPIO, UART, timers
/chapter04\_interrupts/  # NVIC, ISRs
/chapter05\_drivers/     # Abstractions and modular drivers
/lessons.md             # Running log of insights and notes

```

---

## 📝 Lessons Learned
Each chapter folder contains:
- **Source code examples** tested on STM32 boards
- **Notes** explaining key concepts
- **Practical takeaways** about embedded C programming

A running summary is also kept in [`lessons.md`](lessons.md).

---

## ⚡ How to Use
1. **Hardware**  
   - ARM Cortex-M board (e.g., STM32 Nucleo, Discovery kit, or similar)

2. **Toolchain**  
   - ARM GCC toolchain (`arm-none-eabi-gcc`)  
   - OpenOCD or ST-LINK for flashing/debugging  

3. **Build & Run**  
   ```sh
   cd chapter01_intro
   make flash
  ```


embedded-c bare-metal arm-cortex-m stm32 firmware-development real-time-systems embedded-systems microcontrollers low-level-programming learning-notes

```

