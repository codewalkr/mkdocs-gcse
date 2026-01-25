# The central processing unit

## **CPU**

* The **central processing unit (CPU)** is responsible for executing the instructions given to it via a program.

> **microprocessor dependencies:**
>
> - to allow users to input instructions
> - transfer the instructions to carry them out
> - carry out the command (execute) 

### **Buses**

* A bus is a collection of "wires" or tracks on a printed circuit board (PCB) that carry signals or communications between the various components.
* The **Control Bus** connects the **control unit (CU)** with other components.

> **buses:**
>
> - Control bus -> "instructions"
> - Data bus -> CPU/RAM
> - Address bus

### **Executing instructions**

* The **von Neumann architecture** works through the **fetch-execute cycle**

### **Fetch**

* Fetch part of cycle, instruction & data are moved from RAM to CPU

### **Execute**

* The CU decodes/interprets instructions and decides what to perform. Instructions -> ( CPU -> CU/ALU )

## **Components of CPU**

* ALU (addition/subtraction/multiplication/division/logical gates/comparisons)

> **components:**
>
> - ALU (**Arithmetic Logic Unit**)
> - The control unit (**clock & decoder**)
> - The clock (one instruction per pulse of the clock)
> - The decoder (Instructions to binary)
> - Registers (stroage location within the CPU itself)

### **Registers**

* the accumulator (A or ACC)
* the program counter (PC)
* the memory address register (MAR)
* the memory data register (MDR) or memory buffer register (MBR)

## **CPU Performance**

### **Clock speed**

* The rate at which instructions are processed.
* microprocessors generate large amounts of heat, which increases with clock speed.
* Overclocking is the process of increasing the clock speed beyond manufacture recommendations, which can cause damage to CPU.
* Clock speeds of 9Gz require cooling by liquid nitrogen!

### **Number of cores**

**multi-core** processors essential are multiple processors within one CPU, each has its own L1,L2 and L3 cache and can work independently. The ability for a CPU to process multiple instructions is called **Multi-core Processing**.

In the context of processing, **Asynchronous** (often shortened to "**async**") refers to a method of execution where a task can start, run in the background, and finish later without making the CPU wait around for it.

### **Cache size**

* Bottlenecks occur when one component cannot work as fast as another, and hinders progress.
* In the **fetch-execute** cycle this is caused by bottleneck between the CPU and RAM.
* CPU to/from RAM is quicker that RAM to/from DISK, but data buses are far slower than the inner working of the CPU itself.

The solution is to use much faster memory very close or with the CPU, this is called **cache**.

* **data caches** are **read/write**
* **instruction caches** are **read only**

* **RAM** - Dynamic random-access memory (**DRAM**) 
* **cache** - Static Random Access Memory (**SRAM**)

* **Caches** are located on the processor chip, the fastest is **Level 1** (L1), followed by **Level 2** (L2) and **Level 3** (L3).

**Bonus Info**:

*The "Waiter" Analogy*

To understand the difference between synchronous and asynchronous, imagine a restaurant:

**Synchronous (Blocking)**: A waiter takes your order, goes to the kitchen, and stands there staring at the chef until the food is ready. Only then does he bring it to you and move on to the next customer. The waiter is "blocked" and useless during the wait.

**Asynchronous (Non-blocking)**: A waiter takes your order, hands the ticket to the kitchen, and immediately goes to serve other tables. When the food is ready, a bell rings, and the waiter returns to pick it up. He stayed productive the whole time.

**Asynchronous programming** is a way for software to be more efficient, even on a single core, **but it works beautifully with multi-core systems**.

* Async vs. Parallelism

People often confuse these two, but they aren't the same thing:

| Feature  |Parallelism (Multi-core)                | Asynchrony (Async)                                           |
|----------|----------------------------------------|--------------------------------------------------------------|
| Goal     | Speed (doing things at the same time). | Responsiveness (not waiting for one thing to finish).        |
| Hardware | Requires multiple cores/processors.    | Can happen on a single core.                                 |
| Focus    | Solving a math problem faster.         | Handling "I/O" (waiting for internet, disks, or user input). |

**multi-core processors**: 

* the cores can work together on the same program **parallel processing**
* the core can wotrk on differnet programs at the same time **multi-tasking**

## **Embedded systems**

An embedded system is a computer built within a larger device such as a washing machine or digital camera. 

* An embedded system is built inti a larger device and carries out a limited number of functions.
* All components in an embedded system include microprocessor, meomry, input/output interfaces are all on a single PCB.
* The memory contains the program (ROM/EPROM)

* **ROM** (Read-Only Memory) Think "Very old game cartridges or basic hardware controllers".
* **EPROM** (Erasable Programmable Read-Only Memory)

## **Summary**

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

The CPU performance:

1. The clock speed cannot be increased indefinitely due to the heat generated
2. A processor with several CPUs is said to me **multi-core**
3. The processing speed of the CPU is limited byt the speed tha data can be supplied by the slower RAM
4. Cache memory store regularly used items of data for faster access.
5. When RAM is full, the OS will/can store data on disk (the virtual memory), also known as **swap**. This can be terrible for performance.

## **Key Terms**

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
* heat sink
* cache
* parallel processing
* multitasking
* hardware
