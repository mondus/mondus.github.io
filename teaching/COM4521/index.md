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
* The VAR Lab - This room has been made available exclusively to students on this module to provide additional GPU machines. The PCs are not on managed desktop but do have access to the software center. If Visual Studio or CUDA is not installed then Visual Studio 2017 and CUDA 9.1 should be installed from the software center (specifically in that order).
* Your own Windows machine - You will need to install an old version of Visual Studio 2017 following the instructions from the [Visual Studio 2017 Guidance Page](./visual_studio) followed by CUDA 9.1.
* Your own Linux machine - Example makefiles are provided with the lab handouts and solutions. You will need to install CUDA 9.1.
* ShARC - In week 8, the lab class will guide you through how to use the ShARC facility to submit GPU jobs to the Universities HPC system. Instructions for ShARC usage will be made available before easter for those wishing to use the facility in advance of week 8.

# Week 01
## Lecture 01 - Introduction ([pdf]())

* Context and Hardware Trends
* Supercomputing
* Software and Parallel Computing
* Course Outline

## Lecture 02 - Introduction to C ([pdf]())

* Introduction to the C Programming Language
* Basic C Usage "Hello World"
* Functions and Scoping
* Arrays, Strings and Basic IO
* File IO
* Visual Studio 2013 Overview ([available as a separate download](https://drive.google.com/a/sheffield.ac.uk/file/d/0B2HbOiEppVPMcHBVR05GQkUwWEE/view?usp=sharing))

## Lab 01 - C Programming 

* [Lab Sheet]()
* [Source Code]()
* Solution

# Week02: 

## Lecture 03 - Memory (pdf])

* Pointers
* Advanced use of Pointers
* Dynamically Managed Memory
* Structures
* Binary Files

### Week 02: Lecture 04 - Optimisation ([pdf]())

* Optimisation Overview
* Compute Bound Code
* Memory Bound Code

### Week 03: Lecture 05 - OpenMP ([pdf]())

* Multi-core Systems and OpenMP
* Parallelising Loops
* Critical Sections and Synchronisation
* OpenMP Scoping
* Task Parallelism with Sections

### Week 03: Lecture 06 - OpenMP Part II ([pdf]())

* Parallel Reduction
* Scheduling
* Nesting

### Week 04: Lecture 07 - GPU Architectures ([pdf]())

* What is a GPU?
* General Purpose Computation on GPUs (and GPU History)
* GPU CUDA Hardware Model
* Accelerated Systems

### Week 04: Lecture 08 - Introduction to CUDA ([pdf]())

* CUDA Programming Model
* CUDA Device Code
* CUDA Host Code and Memory Management
* CUDA Compilation and execution in Visual Studio

### Week 05: Lecture 09 - CUDA Memory ([pdf]())

* Memory Hierarchy Overview
* Global Memory
* Constant Memory
* Texture and Read-only Memory
* Roundup & Performance Timing

### Week 05: MOLE QUIZ (Diamond high spec compute room, DIA-002, Computer room 2)

### Week 06: Lecture 10 - CUDA Shared Memory ([pdf]())

* Shared Memory
* Shared Memory Bank Conflicts
* 2D Shared Memory Bank Conflicts
* Boundary Conditions for Shared Memory Loading
* Host-side Configurations for Shared Memory
* [Shared Memory Bank Conflict Calculator]()

### Week 06: Lecture 11 - CUDA Performance ([pdf]())

* Global Memory Coalescing
* Global Memory Coalescing with the L1 Cache
* Occupancy and Thread Block Dimensions

### Easter Vacation

### Week 07: Lecture 12 - Warp Level CUDA ([pdf]())

* Warp Scheduling and Divergence
* Atomics
* Warp Operations
* [Excel cheat sheet for SM conflicts]()

### Week 07: Lecture 13 - Parallel Patterns ([pdf]())

* Parallel Patterns Overview
* Reduction
* Scan


### Week 8: Lecture 14 and 15 - Performance Optimisation ([pdf]())

* Profiling Introduction
* The Problem
* Visual Profiler Guided Analysis
* Profiling in the lab ([available as a separate download]())


### Week 09: Lecture 16 - Sorting and Libraries ([pdf](https://drive.google.com/a/sheffield.ac.uk/file/d/0B2HbOiEppVPMN2t2dEN3TWxBaUU/view?usp=sharing))

* Sorting Networks
* Merge and Bitonic Sort
* Thrust Parallel Primitives Library
* Applications of Sorting (binning)

### Week 09: Lecture 17 - CUDA Streams ([pdf](https://drive.google.com/a/sheffield.ac.uk/file/d/0B2HbOiEppVPMNUt6UkJieW9XX2c/view?usp=sharing))

* Synchronous and Asynchronous execution 
* CUDA Streams
* Synchronisation
* Multi GPU Programming

### Week 10: Lecture 18 - Invited Talk


### Week 11: BANK HOLIDAY


### Week 12: No lecture



# Labs

Lab sheets are available via Google Drive [Lab Sheets](https://drive.google.com/a/sheffield.ac.uk/folderview?id=0B2HbOiEppVPMdHdCQS1RZGVsNXM&usp=sharing), [Lab Solutions](https://drive.google.com/a/sheffield.ac.uk/folderview?id=0B2HbOiEppVPMV3VsSjA1SFo5ODQ&usp=sharing) (you will need to login with your university credentials).

A [Lab FAQ document](https://docs.google.com/a/sheffield.ac.uk/document/d/1w4k87mKyJke4bfbWbUVT7rpio2hN7_RUXRDZIT93j9g/edit?usp=sharing) has been prepared with common questions. This will be continually updated throughout the course.

### Lab 01 - C Programming 

* [Lab Sheet](https://drive.google.com/a/sheffield.ac.uk/file/d/0B2HbOiEppVPMc0tzQ2lCNzdSNkk/view?usp=sharing)
* [Source Code](https://drive.google.com/a/sheffield.ac.uk/file/d/0B2HbOiEppVPMY0ExNjg0TGxQWlk/view?usp=sharing)
* [Solution](https://drive.google.com/a/sheffield.ac.uk/file/d/0B2HbOiEppVPMWXR4ZFFWQmowcWM/view?usp=sharing)

### Lab 02 - Memory and Performance

* [Lab Sheet](https://drive.google.com/a/sheffield.ac.uk/file/d/0B2HbOiEppVPMSUNzVGxBMVd4dE0/view?usp=sharing)
* [Source Code](https://drive.google.com/a/sheffield.ac.uk/file/d/0B2HbOiEppVPMTWlHQnZlczhSNGM/view?usp=sharing)
* [Solution](https://drive.google.com/a/sheffield.ac.uk/file/d/0B2HbOiEppVPMaVNwNGY1NzFKTzA/view?usp=sharing)

### Lab 03 - OpenMP

* [Lab Sheet](https://drive.google.com/a/sheffield.ac.uk/file/d/0B2HbOiEppVPMazFrakdrSTNOVm8/view?usp=sharing)
* [Source Code](https://drive.google.com/a/sheffield.ac.uk/file/d/0B2HbOiEppVPMTUcyRWtzUkxLUmM/view?usp=sharing)
* [Solution](https://drive.google.com/a/sheffield.ac.uk/file/d/0B2HbOiEppVPMNkJyMlZDMEpiQ1U/view?usp=sharing)

### Lab 04 - Introduction to CUDA

* [Lab Sheet](https://drive.google.com/a/sheffield.ac.uk/file/d/0B2HbOiEppVPMalBCUTBsc181cXM/view?usp=sharing)
* [Source Code](https://drive.google.com/a/sheffield.ac.uk/file/d/0B2HbOiEppVPMcnRSUjFHZnFiYmc/view?usp=sharing)
* [Solution](https://drive.google.com/a/sheffield.ac.uk/file/d/0B2HbOiEppVPMN1RfM0dtMGNBUms/view?usp=sharing)

### Lab 05 - Memory

* [Lab Sheet](https://drive.google.com/a/sheffield.ac.uk/file/d/0B2HbOiEppVPMTUhRaGRIcm5ZbE0/view?usp=sharing)
* [Source Code](https://drive.google.com/a/sheffield.ac.uk/file/d/0B2HbOiEppVPMZ3VTdEYtWUF4dmc/view?usp=sharing)
* [Solution](https://drive.google.com/a/sheffield.ac.uk/file/d/0B2HbOiEppVPMUm9zb1N6UWxjUlU/view?usp=sharing)

### Lab 06 - Shared Memory and Occupancy

* [Lab Sheet](https://drive.google.com/a/sheffield.ac.uk/file/d/0B2HbOiEppVPMOFQxbGJneWNXZW8/view?usp=sharing) 
* [Revised Lab sheet with row major access](https://drive.google.com/a/sheffield.ac.uk/file/d/0B2HbOiEppVPMLXFqaHBlcHRuVTQ/view?usp=sharing)
* [Source Code](https://drive.google.com/a/sheffield.ac.uk/file/d/0B2HbOiEppVPMNjBxbnRwVy1oZTA/view?usp=sharing) 
* [Revised Source Code with row major access](https://drive.google.com/a/sheffield.ac.uk/file/d/0B2HbOiEppVPMMlp1Y0E3dlhUU1E/view?usp=sharing)
* [Solution for orginal lab sheet](https://drive.google.com/open?id=0B2HbOiEppVPMTE5YQ2xKZGpNYXM)
* [Solution for revised row major version](https://drive.google.com/open?id=0B2HbOiEppVPMM2ZaS0NNczBON28)
 
### Lab 07 - Atomics and Primitives

* [Lab Sheet](https://drive.google.com/open?id=0B2HbOiEppVPMSXJRb2E2aFhrTjQ)
* [Source Code](https://drive.google.com/open?id=0B2HbOiEppVPMOTRFQXRYRTQwem8)
* [Solution](https://drive.google.com/open?id=0B2HbOiEppVPMVUhNMGRmOHdfeTQ)

### Lab 08 - Libraries and Streams

* [Lab Sheet](https://drive.google.com/a/sheffield.ac.uk/file/d/0B2HbOiEppVPMVzhKYVc2OUVtTVk/view?usp=sharing)
* [Source Code](https://drive.google.com/a/sheffield.ac.uk/file/d/0B2HbOiEppVPMV0FPVVhjSHpSUUE/view?usp=sharing)
* [Solution](https://drive.google.com/a/sheffield.ac.uk/file/d/0B2HbOiEppVPMeE9heUlLRmtneFU/view?usp=sharing)

### No Lab Sheet Exercise or Code for Week 09 - Assignment Help

* [Profiling in the Diamond Lab](https://drive.google.com/a/sheffield.ac.uk/file/d/0B2HbOiEppVPMTEV3dmprek5UZnc/view?usp=sharing)
* Review the profiling code form the lectures 

### Lab 09 - CUDA OpenGL Interop

* [Lab Sheet](https://drive.google.com/a/sheffield.ac.uk/file/d/0B2HbOiEppVPMSW15clJuYXRCQ1E/view?usp=sharing)
* [Source Code](https://drive.google.com/a/sheffield.ac.uk/file/d/0B2HbOiEppVPMTUE1TF9Pb2RZZGc/view?usp=sharing)
* [Solution](https://drive.google.com/a/sheffield.ac.uk/file/d/0B2HbOiEppVPMemtCbmU1SVlOV0E/view?usp=sharing)

# Feedback

Anonymous feedback can be provided for the course content at any time by [visiting the feedback form](https://goo.gl/0r73gD). For example have you found the content useful, too easy or difficult, or would you like some aspect of the course to be clarified?

# Discussion and Announcements

Discussion and announcements will be made via the modules Gooogle Group.

[https://groups.google.com/a/sheffield.ac.uk/d/forum/com4521-group](https://groups.google.com/a/sheffield.ac.uk/d/forum/com4521-group)

# Calendar

You can add this calendar to your University of Sheffield Google Calendar by searching for COM4521 and COM6521

<iframe src="https://calendar.google.com/calendar/embed?src=sheffield.ac.uk_4gq0ug3uf8dlts9d21gp4l1des%40group.calendar.google.com&ctz=Europe/London" style="border: 0" width="800" height="600" frameborder="0" scrolling="no"></iframe>

# Recommended Reading

* Edward Kandrot, Jason Sanders, "CUDA by Example: An Introduction to General-Purpose GPU Programming", Addison Wesley 2010.
* Brian Kernighan, Dennis Ritchie, “The C Programming Language (2nd Edition)”, Prentice Hall 1988.
* NVIDIA, [CUDA C Programming Guide](http://docs.nvidia.com/cuda/cuda-c-programming-guide/)
