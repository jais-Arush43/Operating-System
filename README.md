# XV6 Operating System Enhancements

## Overview
This project involves extending the XV6 operating system with advanced **memory management** and **process scheduling** features. The enhancements focus on **paging**, **lazy memory allocation**, and implementing **Lottery Scheduling** and **Shortest Job First (SJF)** scheduling policies.  

---

## Features

### Memory Management
- **Paging:** Implemented virtual memory with page tables to map virtual addresses to physical memory.  
- **Lazy Memory Allocation:** Pages are allocated only when accessed (on-demand), improving memory efficiency.  

### Process Scheduling
- **Lottery Scheduling:** Each process is assigned tickets; CPU allocation is probabilistic based on ticket count, ensuring fairness.  
- **Shortest Job First (SJF):** CPU is allocated to the process with the shortest expected execution time, reducing average waiting time.  

---

## Implementation Details
- Modified XV6 kernel to add page table management and lazy allocation routines.  
- Extended process structures to support lottery ticket assignment and execution time tracking for SJF.  
- Added system calls for setting tickets, querying process info, and supporting scheduling algorithms.  
- Ensured backward compatibility with existing XV6 processes and system calls.  

---

## Testing & Validation
- Verified lazy allocation by monitoring page faults on first access.  
- Tested lottery scheduling using multiple processes with different ticket counts; validated probabilistic CPU allocation.  
- Tested SJF scheduling with processes of varying execution times; confirmed correct order of execution.  

---

## Tools & Environment
- **Language:** C  
- **Operating System:** XV6 (Unix-based teaching OS)  
- **Development:** GCC, QEMU for virtual machine testing  
- **Version Control:** Git  

---

