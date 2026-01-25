# Take the quiz

1. Name the parts of the CPU that perform the following functions:
    1. carries out arithmetic and logical computations                  (**Arithmetic Logic Unit** (ALU))
    2. stores data within the CPU itself                                (**Registers**)
    3. coordinates the activities of the CPU and computer               (**control unit** (CU))


* The CPU consists of integrated circuits in the **microprocessor** of a computer.

* The CPU is responsible for **processing** information and controlling the computer.

* In the CPU are the **control unit**, which manages the execution of the instructions, and the **ALU**, which performs mathematical and logical computations.

* In the CPU are storage locations called **registers**.

* One of these is the program **counter** which contains the location of the current instructions.

* The CPU communicates with other components such as memory through bundles of signal wires called **buses**

## Fetch execute cycle

* Instructions and data are stored in **RAM**

* A register called the **program counter** holds address of the next instruction to be **executed**

* This is transmitted through the **data bus**.

* The instruction is **decoded** by the **control unit** and passed to the **arithmetic and logic unit**, which carries out the instruction. 

## CPU Performance

1. To increase the speed of a computer, users often increase the clock frequency, what is this called? **Overclocking**

2. A user who increased the clock frequency noticed the computer is noisier, why?

* **Increased Fan Speed (RPM)**, modern computers use **PWM (Pulse Width Modulation)** fans. 
* The motherboard monitors the CPU temperature via internal sensors, as you overclock, the **CPU temperature rises**.
* The motherboard’s BIOS detects this heat and tells the fans to spin faster to move more air across the heatsink.
* Faster-spinning fans create more turbulence and mechanical noise, resulting in a louder "whirring" or "rushing" sound.

3. The main reason why manufacturers are finding it difficult to produce faster microprocessors is? **the amount of heat generated**

A computer has a quad-core processor:

1. What is meant by "quad-core" and how does it improve the performance of the computer?

**It means the CPU has four independent processing units (cores) integrated into a single physical chip**

2. Explain how using cache memory also improves the performance.

**Cache Memory improves performance, by reducing the "Speed Gap" between the CPU and your RAM.**

## Embedded systems

1. Explain what is meant by an "embedded system"

**An embedded system is a computer system designed to perform one specific, dedicated function within a larger device or electrical system.**

2. List three devices that contain embedded systems.

* **Microwave Oven**
* **Anti-lock Braking System (ABS)**
* **Digital Thermostat**
* **Smart Watch**
* **Traffic Light Controllers**
* **Digital Cameras**

## Final

1. State the roles of the following in the fetch-execute cycle:
    1. The program counter **Holds the address of the next instruction**
    2. The address bus **Tells memory where to look for data**
    3. The data bus **Carries the actual data/instruction**

2. A new laptop with 1.6GHz dual-core CPU and 512KB Level 1 cache, describe what is meant by:
    1. 1.6GHz CPU **The "clock" inside the CPU acts like a metronome, pulses 1.6 billion times per second.**
    2. dual-core CPU **A dual-core processor means there are two cores housed on a single CPU chip**
    3. L! cache **L1 (Level 1) Cache is a very small, extremely fast type of memory located directly inside the CPU core.**