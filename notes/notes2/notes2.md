# Lecture 2 Introduction to Linux Notes

1. ## What is an Operating System?
An operating system provides all fundamental software features of a computer. An OS enables you to use the computer's hardware providing you the basic tools that make the computer useful. All of those features relay on the OS's kernel. Other OS features are owed to additional program that run atop the kernel. 

2. ## What is a kernel?
An OS kernel is a software component that's responsible for managing low-level features of the computer, including the following managing system hardware, memory allocation, CPU time, and program to program interaction. 

3. ## Which other parts aside from the kernel identify an OS?
- Command-Line Shells
This was the de facto way of using computers before the Graphical Interface was invented.
- Graphical User Interfaces
GUIs rely on icons, menus, and a mouse pointer for the user interaction. Linux relies on a GUI known as the X Window System in combination with desktop environment program suites.
- Utility and Productivity Programs
Tools like web browsers, document processors and text editors.
- Libraries
Libraries are collections of programming functions that can be used by a variety of programs. 

4. ## What is linux?
Linux is a Unix-like Operating System popular in academic and business environments. Linux consists of a kernel, libraries and utilities that make up the entire operating system. Linux is available in many distributions. 

5. ## What is a linux distribution?
A complete operating system based on the Linux kernel that includes a collection of software packages, utilities, and libraries. 

6. ## List at least 4 linux characteristics:
- A linux kernel
- Core Unix Tools
- Supplemental Software
- Startup Scripts
- An Installer

7. ## What is Ubuntu?
**Ubuntu** is a Linux distribution based on Debian and composed mostly *free and open-source software*. **Ubuntu** is officially released in three editions: Desktop, Server, and Core for Internet of things devices and robots. All the editions can run on the computer alone, or in a virtual machine. 

8. ## What is Debian?
Debian is an all-volunteer organization dedicated to developing free software and promoting the ideals of the Free Software community. Debian is known to be the Grandfather of all Linux distributions alongside Slackware and Open suse. 

9.  ## List and define the different types of licensing agreements.
- **Open Source**: the software may be distributed for a fee or free. The source code is distributed with the software.
- **Closed Source**: the software is not distributed with the source code. The user is restricted from modifying the code. 
  - Freeware: the software is free but the source is not available.
  - Shareware: the software is free on a trial basis.
- **Free Software**: the software is distributed with the source code. The software can eb free of charge or obtained by a fee. 

10.   ## What is Free Software? Define the 4 freedoms.
Free Software(FSF) is a critical force in the open source world.
- **Freedom 0**: use the software for any purpose
- **Freedom 1**: examine the source code and modify it as you see fit
- **Freedom 2**: redistribute the software
- **Freedom 3**: redistribute your modified software

11.   ## What is virtualization?
Virtualization is defined as creating virtual versions of something. Virtualization is often used to let multiple OSs run on one physical machine at the same time. Virtualization allows admin to divide the hardware and create multiple computers inside a single physical computer.

12.   ## List 3 benefits of virtualization
- Allows running multiple OSs on one machine without dual booting.
- Allows applications to be tested before installing them on a host machine.
- Reduces costs by decreasing the physical hardware that must be purchased for a network. 
- Offers the ability to save the state of a machine at a given time and roll it back or forward. 

13.   ## What is a hypervisor? Include definitions of the 2 types
Hypervisor/Virtual Machine Manager (VMM): Software or Hardware in charge of creating, managing, and running virtual machines. 
- There are two types of Hypervisors:
  - **Type 1 (bare-metal hypervisor)**: This type of hypervisor runs directly on the hardware. The hypervisor is basically the operating system for the physical machine. Type 1 has better performance than Type 2, because there is no host OS involved and the system is dedicated to supporting virtualization. 
  - **Type 2** hypervisor its an application that runs on top of an operating system. This is most commonly used in client-side virtualization. 

14.  ## What is the difference between Guest OS and Host OS?
Host OS is the operating system that is running in the computer where the hypervisor is installed. 
Guest OS is the operating system that is being virtualized in the virtual machine. 

15.  ## What is virtualbox?
Virtualbox is a powerful x86 and **AMD64/Intel64** virtualization product for enterprise as well as home use. Not only is Virtualbox an extremely feature rich, high performance product for enterprise customers, it is also the only professional solution that is freely available as Open Source Software. 
