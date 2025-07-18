# 100 OS Interview Questions with Answers


## BASIC CONCEPTS

### 1. **What is an Operating System?**

An Operating System (OS) is a system software that acts as an interface between hardware and users. It manages computer hardware, software resources, and provides services for application programs.

### 2. **What are the main functions of an Operating System?**

- **Process Management**
- **Memory Management**
- **File System Management**
- **Device Management**
- **Security and Protection**
- **User Interface Management**


### 3. **What are the different types of Operating Systems?**

- **Batch OS**
- **Time-Sharing OS**
- **Distributed OS**
- **Real-Time OS**
- **Network OS**
- **Mobile OS**


### 4. **What is a kernel?**

The kernel is the core component of an OS that manages communication between hardware and software. It performs low-level tasks such as process scheduling, memory management, and device control.

### 5. **What is the difference between a kernel and an OS?**

- **Kernel** is the core that directly interacts with hardware.
- **OS** includes the kernel plus user interfaces, utilities, and applications.


### 6. **What is a process?**

A process is a program in execution. It includes program code, current activity, program counter, stack, and data segment.

### 7. **What is the difference between a process and a program?**

- **Program**: A passive collection of instructions.
- **Process**: An active execution of a program.


### 8. **What are process states?**

- **New**
- **Ready**
- **Running**
- **Waiting/Blocked**
- **Terminated**


### 9. **What is a thread?**

A thread is a lightweight process or the smallest unit of CPU execution. Multiple threads can run within a single process, sharing its resources.

### 10. **Difference between process and thread?**

| Feature | Process | Thread |
| :-- | :-- | :-- |
| Resource allocation | Has separate memory | Shares memory |
| Communication | Needs IPC | Faster, via shared memory |
| Creation | Heavyweight | Lightweight |
| Overhead | More | Less |

## PROCESS MANAGEMENT

### 11. **What is process scheduling?**

It’s the OS’s way of controlling which process gets CPU time. It uses various algorithms to select one of the ready processes.

### 12. **What are scheduling algorithms?**

- **FCFS (First Come First Serve)**
- **SJF (Shortest Job First)**
- **Priority Scheduling**
- **Round Robin**
- **Multilevel Queue Scheduling**


### 13. **What is context switching?**

Context switching is the process of storing a process's state and loading another. This allows multitasking by switching between processes.

### 14. **What triggers context switching?**

- Time slice expiry
- I/O request
- Process termination
- Higher priority task arrival


### 15. **What is throughput?**

Throughput is the number of processes completed per unit time.

### 16. **What is turnaround time?**

It’s the total time taken from process submission to process completion.

### 17. **What is waiting time?**

Time a process spends in the ready queue waiting for CPU.

### 18. **What is a job scheduler (long-term)?**

It selects jobs from job pool and loads them into main memory. It controls mix and degree of multiprogramming.

### 19. **What is a CPU scheduler (short-term)?**

It decides which of the ready, in-memory processes is to be executed next by the CPU.

### 20. **What is a medium-term scheduler?**

It temporarily removes processes from memory (swapping) to reduce load and control multitasking.

## MEMORY MANAGEMENT

### 21. **What is memory management?**

It involves managing the system’s memory resources, allocating and deallocating memory spaces as processes need them.

### 22. **What is virtual memory?**

Virtual memory is a technique to use secondary memory (like disk) as if it were part of the main RAM. It allows programs to use more memory than physically available.

### 23. **What is paging?**

Paging is a memory management technique where memory is divided into fixed-size blocks (pages/frames) and loaded on demand.

### 24. **What is segmentation?**

Segmentation divides memory into variable-sized segments according to the program’s logical divisions like code, stack, data, etc.

### 25. **Difference between paging and segmentation?**

| Feature | Paging | Segmentation |
| :-- | :-- | :-- |
| Size | Fixed | Variable |
| User view | Logical | Programmer-defined |
| External fragmentation | No | Yes |
| Internal fragmentation | Yes | No |

### 26. **What is fragmentation?**

- **Internal**: Wasted space inside an allocated memory block.
- **External**: Wasted space between allocated blocks.


### 27. **What is swapping?**

Swapping moves processes between RAM and disk to increase multitasking.

### 28. **What is a page fault?**

A page fault occurs when the OS tries to access a page not currently in RAM, requiring it to load the page from disk.

### 29. **What are page replacement algorithms?**

- FIFO
- LRU (Least Recently Used)
- Optimal
- Clock


### 30. **What is thrashing?**

A condition where the system spends more time swapping pages in and out of memory than executing processes.

## FILE SYSTEMS

### 31. **What is a file system?**

A file system organizes and stores data on a storage device and manages access, directory structure, naming, and retrieval of files.

### 32. **What are file attributes?**

- Name
- Type
- Size
- Creation/Modification date
- Permissions


### 33. **Types of file access methods?**

- Sequential Access
- Direct Access
- Indexed Access


### 34. **What are file operations?**

- Create
- Delete
- Read/Write
- Open/Close
- Seek
- Allocate


### 35. **What are directory structures?**

- Single-Level Directory
- Two-Level
- Tree-Structured
- Acyclic Graph
- General Graph


### 36. **What is inode?**

An inode stores metadata about a file like size, owner, location, access permissions—but not the filename.

### 37. **What are file allocation methods?**

- **Contiguous**: Simple, fast, causes external fragmentation.
- **Linked**: Avoids fragmentation, slow access.
- **Indexed**: Uses an index block to keep track of all file blocks.


### 38. **What is a mount operation?**

It makes a file system accessible at a certain point in the directory tree.

### 39. **What are file system permissions?**

Defines what a user or group is allowed to do with a file (e.g., read, write, execute).

### 40. **What is journaling in file systems?**

A technique to keep a log (journal) of changes to prevent corruption during crashes or power failures.

## DEVICE \& I/O MANAGEMENT

### 41. **How does OS manage I/O devices?**

Using device drivers and I/O control systems, the OS facilitates communication between devices and applications.

### 42. **What is a device driver?**

A device driver is a software component that allows the OS to interact with hardware devices.

### 43. **What is DMA (Direct Memory Access)?**

A method that allows devices to read/write memory without CPU intervention.

### 44. **What is interrupt?**

An interrupt is a signal to the CPU indicating that an event needs attention.

### 45. **Types of interrupts?**

- Hardware interrupt
- Software interrupt
- Timer interrupt
- I/O interrupt


## SECURITY \& PROTECTION

### 46. **What is the difference between security and protection?**

- **Protection**: Internal mechanisms to restrict access.
- **Security**: Actor-based mechanism to stop unauthorized access.


### 47. **What are access control lists (ACLs)?**

A list specifying which users or groups can access specific files and their permitted operations.

### 48. **What is authentication?**

Process of verifying a user’s identity usually through passwords, biometrics, etc.

### 49. **What is authorization?**

Determining what authenticated users are allowed to do.

### 50. **What is encryption?**

Process of converting data into a coded format to prevent unauthorized access.

## SYSTEM CALLS \& APIs

### 51. **What is a system call?**

System calls are functions that let programs request services from the OS, such as file manipulation, process control, etc.

### 52. **Examples of system calls?**

- `fork()`
- `exec()`
- `read()`, `write()`
- `open()`, `close()`
- `kill()`, `wait()`


### 53. **What are the categories of system calls?**

- Process control
- File management
- Device management
- Information maintenance
- Communication


## MULTITHREADING \& CONCURRENCY

### 54. **What is multithreading?**

Running multiple threads within a single process, allowing parallelism.

### 55. **What are the benefits of multithreading?**

- Faster execution
- Better resource utilization
- Simpler program structure for I/O-based applications


### 56. **What are types of threads?**

- User level threads
- Kernel level threads


### 57. **What are race conditions?**

A situation where two threads access shared data and try to change it at the same time, leading to inconsistent results.

### 58. **How to avoid race conditions?**

Using synchronization mechanisms like:

- Mutex
- Semaphores
- Monitors


## SYNCHRONIZATION

### 59. **What is synchronization?**

Coordination of threads to avoid conflicts or inconsistencies in shared data.

### 60. **What is a critical section?**

A block of code where shared data is accessed.

### 61. **What is a semaphore?**

An integer-based signaling mechanism used for controlling access to shared resources.

### 62. **What is a mutex?**

A locking mechanism to achieve mutual exclusion.

### 63. **Differences between mutex and semaphore?**

- Mutex has ownership, semaphore does not.
- Semaphore is a counter, mutex is binary (lock/unlock).


## DEADLOCK

### 64. **What is deadlock?**

A situation where processes are stuck waiting for resources held by each other, leading to no progress.

### 65. **Necessary conditions for deadlock (Coffman conditions)?**

- Mutual exclusion
- Hold and wait
- No preemption
- Circular wait


### 66. **Deadlock prevention vs avoidance vs detection?**

- **Prevention**: Ensures at least one condition is false.
- **Avoidance**: Uses information to avoid deadlock (e.g., Banker's algorithm).
- **Detection**: Detects and recovers from deadlock.


### 67. **What is Banker's algorithm?**

A deadlock avoidance algorithm that allocates resources only if it leads to a safe state.

## OS ARCHITECTURE \& DESIGN

### 68. **What is monolithic kernel?**

All OS services are bundled in one large block of code running in kernel mode.

### 69. **What is microkernel?**

Only essential services (like IPC, scheduling) run in kernel mode; others run in user mode.

### 70. **Advantages of microkernels?**

- Better security and reliability
- Easier updates
- Smaller kernel size


### 71. **Disadvantages of microkernels?**

- Slower performance due to context switches and IPC


### 72. **What is layered OS architecture?**

OS is divided into layers, each built on top of the lower one, making debugging and development easy.

## DISTRIBUTED \& NETWORK OS

### 73. **What is a distributed system?**

Multiple systems connected via network working together as one system.

### 74. **Features of distributed OS?**

- Transparency (location, replication)
- Fault tolerance
- Resource sharing
- Scalability


### 75. **What is network operating system?**

An OS that is designed for managing and supporting networking capabilities, like file sharing and communication.

## MISCELLANEOUS \& ADVANCED

### 76. **What is booting?**

Process of starting a computer and loading the OS.

### 77. **What is BIOS?**

Basic Input Output System; performs hardware initialization and boots the OS.

### 78. **What is UEFI?**

Unified Extensible Firmware Interface; a modern replacement for BIOS.

### 79. **What is caching?**

A faster storage layer to temporarily hold frequently accessed data.

### 80. **What is a hybrid kernel?**

Combines monolithic and microkernel features, e.g., Windows NT.

## PERFORMANCE \& TROUBLESHOOTING

### 81. **What are system performance metrics?**

- CPU utilization
- Memory usage
- I/O throughput
- Response time


### 82. **What causes high CPU usage?**

- Infinite loops
- Heavy computations
- Process contention
- System daemons


### 83. **How to reduce OS overhead?**

- Use lightweight processes
- Efficient scheduling
- Optimization of memory access


## COMMANDS \& PRACTICAL UNIX/LINUX

### 84. **List some Linux commands related to processes:**

- `ps`
- `top`
- `kill`
- `nice`
- `renice`


### 85. **Difference between `fork()` and `exec()`?**

- `fork()`: Creates a new process.
- `exec()`: Replaces current process with a new one.


### 86. **What is zombie process?**

A process that has completed execution but still has an entry in the process table (waiting for parent to read exit status).

### 87. **What is an orphan process?**

A process whose parent terminated before the child.

## VIRTUALIZATION \& CLOUD

### 88. **What is OS virtualization?**

Abstracting OS resources to run multiple isolated environments (VMs) on one host.

### 89. **Popular virtualization solutions?**

- VMware
- Hyper-V
- KVM
- VirtualBox


### 90. **Difference between VM and container?**

VM: Full OS running on hypervisor
Container: Lightweight, shares the host OS kernel

## REAL-TIME SYSTEMS

### 91. **What is a real-time OS (RTOS)?**

OS intended to process data without delay, used in time-critical systems.

### 92. **Types of RTOS?**

- Hard Real-Time
- Soft Real-Time


## MEMORY MODELS \& MISC

### 93. **What is demand paging?**

Pages are loaded from disk into RAM only when required.

### 94. **What is Belady’s anomaly?**

In some page replacement policies like FIFO, more frames result in more page faults (counterintuitive).

### 95. **What is working set?**

A set of pages a process is currently using; used to model memory demand.

### 96. **What is mmap()?**

Used to map files or devices into memory in UNIX/Linux.

## SYSTEM UTILITIES

### 97. **What’s the role of ‘init’ process in Linux?**

It's the first process started at boot and responsible for bringing up the entire user space.

### 98. **How is load average computed?**

Reflects the average number of runnable threads over time intervals (1, 5, 15 mins).

## TRICKY \& INTERVIEW-SPECIFIC

### 99. **How do you debug high memory usage in an OS?**

- Analyze with `top`, `htop`, `free`, `vmstat`
- Identify leaky processes
- Check swap usage


### 100. **How would you explain an OS to a non-technical person?**

An OS is like the manager of a hotel. It assigns rooms (memory), handles reception (I/O), and makes sure all guests (programs) are treated fairly and don't disturb each other.
