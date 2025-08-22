# Lessons Learned: Bare-Metal Embedded C

This file contains structured notes (AI-read from whiteboard) and takeaways from working through  
*Bare Metal Embedded C Programming: Develop High-Performance Embedded Systems with C for ARM microcontrollers*.

## RUNNING NOTES

### 1. Overview

The journey of a `.c` file through the GNU toolchain into an executable for ARM Cortex-M. 

### 2. Key Notes

* Preprocessor strips comments/macros → `.i` file
* Compiler converts to assembly → `.s` file
* Assembler creates object files → `.o`
* Linker produces ELF, relocatable until placed
* Locator + linker script assigns memory → final binary

### 3. Commands & Examples

```sh
arm-none-eabi-gcc -c -mcpu=cortex-m4 -mthumb main.c -o main.o
```

* `-c`: compile/assemble only, don’t link
* `-mcpu=cortex-m4`: target CPU core
* `-mthumb`: use Thumb instruction set
* `main.c`: input source file
* `-o main.o`: output object file

### 4. Practical Pins / Hardware Mapping

* Green LED → PB0
* Blue LED → PB7
* Red LED → PB14

### 5. Takeaways

* ELF is not directly executable — needs locator & linker script.
* Toolchain steps: source → preprocessed → assembly → object → ELF → executable.
* Clear separation of preprocessing, compilation, assembly, and linking stages.

### 6. Next Steps

* Build a minimal “blink” project using this toolchain.
* Explore how a linker script defines memory regions.