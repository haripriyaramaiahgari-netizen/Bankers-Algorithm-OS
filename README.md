#Banker's Algorithm for Deadlock Avoidance in Operating Systems

## Author
**R. Haripriya**

## Introduction
Banker's Algorithm is a deadlock avoidance algorithm used in Operating Systems. It checks whether granting a resource request keeps the system in a safe state. If a safe sequence exists, resources are allocated; otherwise, the request is denied to prevent deadlocks.

## Problem Statement
In modern computer systems, multiple processes compete for limited resources such as memory, CPU time, printers, and storage devices. Improper resource allocation may lead to deadlocks, where processes wait indefinitely. This project demonstrates how Banker's Algorithm prevents such situations by ensuring safe resource allocation.

## Objectives
- Implement Banker's Algorithm in C.
- Calculate the Need matrix.
- Check whether the system is in a safe state.
- Display the safe sequence.
- Prevent deadlocks through safe resource allocation.

## Algorithm 
1. Input the Allocation, Maximum and Available resource matrices.
2. Calculate the Need Matrix using:
   Need = Maximum − Allocation
3. Find a process whose Need is less than or equal to the Available resources.
4. Allocate resources to that process and mark it as completed.
5. Release the allocated resources after execution.
6. Repeat until all processes are completed or no safe sequence exists.
7. Display the safe sequence if the system is safe.

## Technologies used
• Programming Language : C
• Compiler : OnlineGDB
• Platform : GitHub

## Advantages 
• Prevents deadlocks.
• Improves resource utilization.
• Ensures system stability.
• Increases process efficiency.

## Limitations 
• Requires maximum resource requirements in advance.
• Not suitable for highly dynamic systems.

## Real World Use Cases
-Cloud Computing: Allocates CPU, memory, and storage safely among multiple virtual machines.
-Hospital Management: Ensures ICU beds, ventilators, and medical equipment are allocated without resource conflicts.
-Online Banking: Prevents deadlocks while processing thousands of simultaneous transactions.
-Railway and Airline Reservation Systems: Handles multiple booking requests safely without system conflicts.
-Manufacturing Industry: Coordinates robots and machines that share common resources.
-Data Centers: Distributes CPU, memory, and storage efficiently among applications while maintaining system stability.

## Result
The program successfully checks whether the system is in a safe state and prints the safe sequence of processes.

## Conclusion
The Banker's Algorithm is an effective deadlock avoidance technique that ensures safe resource allocation among multiple processes. It improves system reliability by checking whether the system remains in a safe state before allocating resources.

## References
1. Abraham Silberschatz, Peter B. Galvin, Greg Gagne – Operating System Concepts.
2. William Stallings – Operating Systems: Internals and Design Principles.
3. OnlineGDB Compiler – https://www.onlinegdb.com/