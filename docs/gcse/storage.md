# Storage

## **Primary Storage**

* Storage that can be accessed directly by the CPU. Usually referred to as **"memory"**
* Random Access Memory (RAM)
* Read Only Memory (ROM)

* **byte** a group of 8 bits
* **address** a number assigned to the storage location 
* **volatile** data is lost when power goes
* **BIOS** Basic Input/Output System - control computer when powered on, tests sys hardware and load OS

!!! note
    The **BIOS** is stored in **ROM**, where RAM is "volatile" ROM is not!

## **Virtual Memory**

When your computer runs out of physical RAM, it uses a trick called **Virtual Memory** (or **Swap** on Linux/macOS) to keep things running.

* **Expansion**: It simulates additional RAM by using a portion of your hard drive or SSD as if it were memory.
* **The "Swap" Process**: When RAM is full, the operating system moves inactive data into a **Page File** or **Swap Partition** on the disk.
* **Performance Hit**: Accessing data from a drive is significantly slower than accessing it from RAM. 
* **Stability**: It prevents programs from crashing immediately when you hit your RAM limit, giving the system a "buffer" to manage heavy workloads.

## Secondary Storage

* **Magnetic media**, electromagnets in read-write heads read and write data on discs coasted with magnetic materials
* **Optical media**, light from lasers read and write data on specifically prepared discs
* **Electrical or solid stat storage**, data is stored electrically
* **Cloud storage**, off-site storage accessed over the internet
* **Block Storage** Best for Virtual Machine disks, high-performance databases, and transactional applications.
*  **Object Storage** Best for Static assets like photos/videos, backups, logs, and massive "data lakes" for AI training.

## Units

Any system involving two states is called a **binary system**

| Unit     | Symbol | Size in Bytes   |
|----------|--------|-----------------|
| Nibble   |-       | -               |
| Byte     | B      | -               |
| Kilobyte | KB     | 1000 bytes      |
| Megabyte | MB     | 1000 kilobytes  |
| Gigabyte | GB     | 1000 megabytes  |
| Terabyte | TB     | 1000 gigabytes  |
| Petabyte | PB     | 1000 terabytes  |

## **Summary**

* Random access memory (**RAM**) acts as a temporary store of program instructions and data.
* RAM consists of billions of memory locations with unique addresses.
* The addresses can be accessed in any order
* RAM is volatile and can be written to.
* Dynamic RAM (**DRAM**) is slower that static RAM (**SRAM**) but is far cheaper.
* Read-only memory is used to store basic info and instructions that a computer need to start-up. 
* Read-only memory (ROM) is non-volatile but cannot be written to. 

* **Magnetic media**, electromagnets in read-write heads read and write data on discs coasted with magnetic materials
* **Optical media**, light from lasers read and write data on specifically prepared discs
* **Electrical or solid stat storage**, data is stored electrically
* **Cloud storage**, off-site storage accessed over the internet
* **Block Storage** Best for Virtual Machine disks, high-performance databases, and transactional applications.
*  **Object Storage** Best for Static assets like photos/videos, backups, logs, and massive "data lakes" for AI training.

* Billions of transistors in the CPU carry out millions of calculations per second.
* Transistors act as switches, either **on** or **off**
* These two states are represented byt either **0** or **1**
* All programs and data consist of billions of 1s & 0s which are called **bits**
* Bits are grouped into the units:
    * **Nibble (4 bits)**
    * **byte (8 bits)**
    * **kilobyte (1024 Bytes, 8192 Bits)**
    * **megabyte (1024 kilobytes, 8388608 bits)**
    * And so on! 

!!! note
    Example of working out how many bits are in a megabyte is `1024 x 1024 x 8`.

## **Key Terms**

* Primary storage
* Secondary storage
* byte
* address
* volatile (ephemeral)
* BIOS
* applications
* execution
* secondary storage devices
* optical storage
* electrical storage
* magnetic storage
* binary digits 
* bits
