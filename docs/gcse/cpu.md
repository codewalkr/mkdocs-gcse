# The central processing unit

* The **central processing unit (CPU)** is responsible for executing the instructions given to it via a program.

> **microprocessor dependencies:**
>
> - to allow users to input instructions
> - transfer the instructions to carry them out
> - carry out the command (execute) 

## Buses

* A bus is a collection of "wires" or tracks on a printed circuit board (PCB) that carry signals or communications between the various components.
* The **Control Bus** connects the **control unit (CU)** with other components.

> **buses:**
>
> - Control bus -> "instructions"
> - Data bus -> CPU/RAM
> - Address bus

## Executing instructions

* The **von Neumann architecture** works through the **fetch-execute cycle**

## Fetch

* Fetch part of cycle, instruction & data are moved from RAM to CPU

## Execute

* The CU decodes/interprets instructions and decides what to perform. Instructions -> ( CPU -> CU/ALU )

# Components of CPU

* ALU (addition/subtraction/multiplication/division/logical gates/comparisons)

> **components:**
>
> - ALU
> - The control unit (**clock & decoder**)
> - The clock (one instruction per pulse of the clock)
> - The decoder (Instructions to binary)
> - Registers (stroage location within the CPU itself)

## Registers

* the accumulator (A or ACC)
* the program counter (PC)
* the memory address register (MAR)
* the memory data register (MDR) or memory buffer register (MBR)

# Summary

The CPU:

1. Consists of:
    1. control unit (CU)
    2. arithmetic and logic unit (ALU)
    3. registers
    
2. The **CU** controls the activities of the CPU by sending out control signals.
3. The **ALU** carries out arithmetic and logical operations
4. The **registers** are memory stores within the CPU.

The CPU processes data by these steps:

1. **Fetch**: instruction is transferred from memory to CPU
    a. Program counter supplies the address of the instruction to fetch
    b. The program counter is a register (or memory location) in the CPU
2. **Decode**: the CPU works out what the instructions mean.
3. **Execute**: The control unit (CU) carries out the instructions using ALU for logical or mathematical operations.

# Key Terms

* central processing unit (CPU)
* microprocessor
* control unit (CU)
* Arithmetic and logical unit (ALU)
* CPU bus
* registers
* input devices
* random access memory (RAM)
* output devices
* bus
* printed circuit board (PCB)

