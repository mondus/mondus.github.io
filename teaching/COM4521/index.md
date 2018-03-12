---
title: Dr Paul Richmond - COM4521 & COM 6521 Introduction to Parallel Computing with GPUs
layout: homepage
---

# About the Course

Accelerator architectures are discrete processing units which supplement a base processor with the objective of providing advanced performance at lower energy cost. Performance is gained by a design which favours a high number of parallel compute cores at the expense of imposing significant software challenges. This module looks at accelerated computing from multi-core CPUs to GPU accelerators with many TFlops of theoretical performance. The module will give insight into how to write high performance code with specific emphasis on GPU programming with NVIDIA CUDA GPUs. A key aspect of the module will be understanding what the implications of program code are on the underlying hardware so that it can be optimised.
 
The modules aims, objectives and assessment details are available on the [modules public teaching page](http://www.dcs.shef.ac.uk/intranet/teaching/public/modules/level4/com4521.html).

# Lecture and Lab Location

Lectures will take place on Mondays 15:00 until 17:00 in Broad Lane Lecture Theater 11 (BROAD-LT11). In week 5 the second half of the lecture will be a MOLE quiz in Diamond high spec compute room (DIA-206). Week 11 will be an invited lecture in the usual lecture location.

Labs will take place on Tuesdays 9:00 until 10:50 in the Diamond high spec compute room (DIA-206). Week 10 will be a MOLE Quiz (9:00-10:00) followed by assignment help and week 11 will be for assignment help. There will be no lab in week 12.

# Lecture and Lab Material

Lectures notes and labs are available via [Google Drive](https://drive.google.com/drive/folders/1SYgShnHdLkZGX0QzY9Bw7Tv03aEIcS-S?usp=sharing) (you will need to login with your university credentials) or via the links below. Lecture material will be made available shortly before the lecture each week.

# Software for the Module

The module programming exercises are designed to be completed in the Diamond high spec compute room. The room has recently been upgraded with Visual Studio 2017 and CUDA 9.1. **IMPORTANT** If you intend to use your own machine for programming exercises (on the CUDA part of the module) then you **must** install an early version of Visual Studio 2017 (or Visual Studio 2015). Later versions of Visual Studio (such as the one from the official Microsoft site) have no CUDA support. Please read the [Visual Studio 2017 Guidance Page](./visual_studio) for instruction on how to install. If you want to complete the exercises in Linux then example Makefiles will be provided with the lab starting code and solution. It is not possible to build Linux CUDA programs in the high spec compute room, however there will be lab instructions on how to remotely build and execute CUDA code for the Universities High Performance (HPC) computing system (ShARC).

# Computers and Labs Available

The Diamond high spec compute room is booked for the lab classes and is always available to you during standard lab hours. Our side of lab times the room has a tendency to be quite busy, especially towards the end of term when assignments are due. The following options are available to you;

* The diamond high spec compute room - Lab has NVIDIA GPUs, Visual Studio 2017 and CUDA 9.1
* [The VAR Lab](https://www.sheffield.ac.uk/diamond/engineering/var) - This room has been made available to students on this module to provide additional GPU machines. The PCs are not on managed desktop but do have access to the software center. If Visual Studio or CUDA is not installed then Visual Studio 2017 and CUDA 9.1 should be installed from the software center (specifically in that order). The Room must be booked ([using the following form](https://script.google.com/a/macros/sheffield.ac.uk/s/AKfycbzBOn2dOVvNepZNhsJnCKEV4qhEeYUBMTY_lNIuOM45U9YkCw2C/exec)) and you will need to complete short induction.
* Your own Windows machine - You will need to install an old version of Visual Studio 2017 following the instructions from the [Visual Studio 2017 Guidance Page](./visual_studio) followed by CUDA 9.1.
* Your own Linux machine - Example makefiles are provided with the lab handouts and solutions. You will need to install CUDA 9.1.
* ShARC - In week 8, the lab class will guide you through how to use the ShARC facility to submit GPU jobs to the Universities HPC system. Instructions for ShARC usage will be made available before easter for those wishing to use the facility in advance of week 8.

# Lab Attendance Checking and Module Feedback

You are required to complete a lab register to indicate your progress with the lab exercises each week. You should fill this either once you have completed the lab exercises. It is not expected that you will be able to complete all of the lab exercises within the two hour lab slot, you are expected to undertake independent study but you must try and complete the labs before the start of the next lab. The purpose of the lab register is to monitor class progress to be able provide feedback, clarifications on difficult areas and additional assistance to you. please use the additional comments section to highlight if you found the content useful, too easy or difficult, or would you like some aspect of the course to be clarified?

[Lab Register and Feedback Form](https://goo.gl/0r73gD)

You will receive additional feedback from the module through discussion in the lab classes, MOLE quiz assessment and your assignment 1 handin.

# Assignments

There are two assignments for the module which contribute 80% of the total module mark

* Part 1 (30% of the assignemnt total) - Released Week 3, Due Tuesday week 7 (20/03/2018) at 17:00
* Part 2 (70% of the assignment total) - Released Week 6, Due Tuesday week 12 (15/05/2018) at 17:00

The remaining 20% of the module mark is from two mole quizes which are 

* Week 5 - During the second half of the lecture in Diamond high spec compute room (DIA-206)
* Week 10 - During the first half of the lab class in Diamond high spec compute room (DIA-206)

# Discussion, Announcements and Requests for Help

A [Google group](https://groups.google.com/a/sheffield.ac.uk/d/forum/com4521-group) has been created for announcements, help and discussion. Any changes to timetabling will be made via this group. All students enrolled on the module on the 1st Feb 2018 have been added to this group already. If you have transfered via Add/Drop then you will need to manually join the group yourself. The group is monitored by the teaching staff (including lab assistants) as well as additional PhD students who can provide help with the lab classes or assignment. This is a public (within the University of Sheffield) forum and therefore you should not post assignment code. If you require personal assistance then you should request this during the lab hours. Any lab class can be used for assignment help in addition to the lab exercises which are set.

[https://groups.google.com/a/sheffield.ac.uk/d/forum/com4521-group](https://groups.google.com/a/sheffield.ac.uk/d/forum/com4521-group)


# Teaching Material

## Week 01

### Lecture 01 - Introduction ([pdf](https://drive.google.com/file/d/1gzpVxLevd64Htc61l2HtT5p--BrGs0Ut/view?usp=sharing))

* Context and Hardware Trends
* Supercomputing
* Software and Parallel Computing
* Course Outline

### Lecture 02 - Introduction to C ([pdf](https://drive.google.com/file/d/1Bu5txgZ1WSyk5y9rbfw5Ub1EOdolGxiX/view?usp=sharing))

* Introduction to the C Programming Language
* Basic C Usage "Hello World"
* Functions and Scoping
* Arrays, Strings and Basic IO
* File IO
* Visual Studio 2017 Overview ([pdf](https://drive.google.com/file/d/1RoIziwJdneABVb2kMlEq4UrpUzUg-qm4/view?usp=sharing))

### Lab 01 - C Programming 

* [Lab Sheet](https://drive.google.com/file/d/1D36rRt3UpYkFH_MFLgorsqEdO2QlY7Ay/view?usp=sharing)
* [Source Code](https://github.com/mondus/com4521/archive/Lab01_src.zip)
* [Solution](https://github.com/mondus/com4521/archive/Lab01_sln.zip)

## Week02: 

### Lecture 03 - Memory ([pdf](https://drive.google.com/file/d/10itZqE3YEILYcTaxL4OUyRFMGZ-83_u6/view?usp=sharing))

* Pointers
* Advanced use of Pointers
* Dynamically Managed Memory
* Structures
* Binary Files

### Lecture 04 - Optimisation ([pdf](https://drive.google.com/file/d/1ng4JPE7MYS1zV7Aj7K79q5w1caBbb522/view?usp=sharing))

* Optimisation Overview
* Compute Bound Code
* Memory Bound Code

### Lab 02 - Memory and Performance

* [Lab Sheet](https://drive.google.com/file/d/1sUmGKBCqkh7T9BRgNK9GTHYiAlSLIxEu/view?usp=sharing)
* [Source Code](https://github.com/mondus/com4521/archive/Lab02_src.zip)
* [Solution](https://github.com/mondus/com4521/archive/Lab02_sln.zip)

## Week 03

### Lecture 05 - OpenMP ([pdf](https://drive.google.com/file/d/1TGJH3XE5KuHcyZhOb9WuS1LTfTxhRJsG/view?usp=sharing))

* Multi-core Systems and OpenMP
* Parallelising Loops
* Critical Sections and Synchronisation
* OpenMP Scoping
* Task Parallelism with Sections

### Lecture 06 - OpenMP Part II ([pdf](https://drive.google.com/file/d/1In38jp2oemomL0qrmW_IdPUcn0hdwBSX/view?usp=sharing))

* OpenMP TIming
* Parallel Reduction
* Scheduling
* Nesting

### Lab 03 - OpenMP

* [Lab Sheet](https://drive.google.com/file/d/1av2Dnig7yiX41jlVVQd9mU1Zjp_P6Top/view?usp=sharing)
* [Source Code](https://github.com/mondus/com4521/archive/Lab03_src.zip)
* [Solution](https://github.com/mondus/com4521/archive/Lab03_sln.zip)

## Week 04

### Lecture 07 - GPU Architectures ([pdf](https://drive.google.com/file/d/16wCEOYkEVKl09nQIM3xZFc4V9T8UmXJE/view?usp=sharing))

* What is a GPU?
* General Purpose Computation on GPUs (and GPU History)
* GPU CUDA Hardware Model
* Accelerated Systems

### Lecture 08 - Introduction to CUDA ([pdf](https://drive.google.com/file/d/1P8egjKhItHT1T4p_WZ5b__InbLtK81DS/view?usp=sharing))

* CUDA Programming Model
* CUDA Device Code
* CUDA Host Code and Memory Management
* CUDA Compilation and execution in Visual Studio

### Lab 04 - Introduction to CUDA

* [Lab Sheet](https://drive.google.com/file/d/1X7OxvYZmxXoXqbCSAZ7KeGtZYj-Byvm2/view?usp=sharing)
* [Source Code](https://github.com/mondus/com4521/archive/Lab04_src.zip)
* [Solution](https://github.com/mondus/com4521/archive/Lab04_sln.zip)


## Week 05

### Lecture 09 - CUDA Memory ([pdf](https://drive.google.com/file/d/1FPgi2nmDavd-_Sc6Rd7eDfDPQDBU-UVm/view?usp=sharing))

* Memory Hierarchy Overview
* Global Memory
* Constant Memory
* Texture and Read-only Memory
* Roundup & Performance Timing

### 5th March 2018 (16:00) - MOLE QUIZ (Diamond high spec compute room, Computer room 4)

### Lab 05 - Memory

* [Lab Sheet](https://drive.google.com/file/d/1itfrEHTyIT8zgLk_S8ay7pVMnVynfniZ/view?usp=sharing)
* [Source Code](https://github.com/mondus/com4521/archive/Lab05_src.zip)
* [Solution](https://github.com/mondus/com4521/archive/Lab05_sln.zip)


## Week 06

### Lecture 10 - CUDA Shared Memory ([pdf](https://drive.google.com/file/d/1CN977UxqI5DbVpIK5YxKKuSalnpv-7Wi/view?usp=sharing))

* Shared Memory
* Shared Memory Bank Conflicts
* 2D Shared Memory Bank Conflicts
* Boundary Conditions for Shared Memory Loading
* Host-side Configurations for Shared Memory
* [Shared Memory Bank Conflict Calculator](https://drive.google.com/file/d/173St-SBa9J3gtvt3CdTVrhPZqE-fNbY_/view?usp=sharing)

### Lecture 11 - CUDA Performance ([pdf](https://drive.google.com/file/d/1aeoY76E9mIlBdgWsHvg5NpmQEdpaf0Cp/view?usp=sharing))

* Global Memory Coalescing
* Global Memory Coalescing with the L1 Cache
* Occupancy and Thread Block Dimensions

### Lab 06 - Shared Memory and Occupancy

* [Lab Sheet](https://drive.google.com/file/d/1csN6DbbE6ooXIOVk4YVLpwftJhS3aiE-/view?usp=sharing)
* [Source Code](https://github.com/mondus/com4521/archive/Lab06_src.zip)
* Solution

## Week 07

### Lecture 12 - Warp Level CUDA (pdf)

* Warp Scheduling and Divergence
* Atomics
* Warp Operations
* [Excel cheat sheet for SM conflicts]()

### Lecture 13 - Parallel Patterns (pdf)

* Parallel Patterns Overview
* Reduction
* Scan

### Lab 07 - Atomics and Primitives

* Lab Sheet
* Source Code
* Solution

## EASTER VACTION

## Week 8

### Lecture 14 and 15 - Performance Optimisation (pdf)

* Profiling Introduction
* The Problem
* Visual Profiler Guided Analysis
* Profiling in the lab ([available as a separate download]())

### Lab 08 - ShARC Lab

* Lab Sheet
* Source Code
* Solution

## Week 09

### Lecture 16 - Sorting and Libraries (pdf)

* Sorting Networks
* Merge and Bitonic Sort
* Thrust Parallel Primitives Library
* Applications of Sorting (binning)

### Lecture 17 - CUDA Streams (pdf)

* Synchronous and Asynchronous execution 
* CUDA Streams
* Synchronisation
* Multi GPU Programming

### Lab 09 - Libraries and Streams

* Lab Sheet
* Source Code
* Solution

## Week 10

### Lecture 18 - Invited Talk

### 1st May 2018 (09:00) - MOLE QUIZ (Diamond high spec compute room, DIA-002, Computer room 2)

### Lab 10 - Assignment Help

## Week 11: BANK HOLIDAY

### Lab 11 - OpenGL and Assignment Help

* Lab Sheet
* Source Code
* Solution

## Week 12: No lectures or labs

# Calendar

You can add this calendar to your University of Sheffield Google Calendar by searching for COM4521 and COM6521

<iframe src="https://calendar.google.com/calendar/embed?src=sheffield.ac.uk_4gq0ug3uf8dlts9d21gp4l1des%40group.calendar.google.com&ctz=Europe/London" style="border: 0" width="800" height="600" frameborder="0" scrolling="no"></iframe>

# Recommended Reading

* Edward Kandrot, Jason Sanders, "CUDA by Example: An Introduction to General-Purpose GPU Programming", Addison Wesley 2010.
* Brian Kernighan, Dennis Ritchie, “The C Programming Language (2nd Edition)”, Prentice Hall 1988.
* NVIDIA, [CUDA C Programming Guide](http://docs.nvidia.com/cuda/cuda-c-programming-guide/)
