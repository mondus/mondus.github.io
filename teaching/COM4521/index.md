---
title: Dr Paul Richmond - COM4521 & COM 6521 Introduction to Parallel Computing with GPUs 2017
layout: homepage
---

# About the Course

Accelerator architectures are discrete processing units which supplement a base processor with the objective of providing advanced performance at lower energy cost. Performance is gained by a design which favours a high number of parallel compute cores at the expense of imposing significant software challenges. This module looks at accelerated computing from multi-core CPUs to GPU accelerators with many TFlops of theoretical performance. The module will give insight into how to write high performance code with specific emphasis on GPU programming with NVIDIA CUDA GPUs. A key aspect of the module will be understanding what the implications of program code are on the underlying hardware so that it can be optimised.
 
The modules aims, objectives and assessment details are available on the [modules public teaching page](http://www.dcs.shef.ac.uk/intranet/teaching/public/modules/level4/com4521.html).


# Assessment

## Assignment

The assignment makes up 80% of the total marks for this module and is split into two related parts. The handout will be available on MOLE from week 3 and week 6 and will be handed in in two stages.  

* Part 1 is due Tuesday 28th March (5pm) - Week 8
* Part 2 is due Wednesday 16th May (5pm) -  Week 12.

## MOLE Quizes

Two quizes, each 10% of the module mark will be held under exam conditions on 

* Monday the 6th March (16:00-17:00) - Week 5 (This is during the second half of the lecture, location to be confirmed)
* Tuesday the 25th April (9:00-10:00) - Week 9 (This will take place during normal lab hours)


# Lecture Notes

Lectures will take place on Mondays 15:00 until 17:00 in Diamond lecture theatre DIA-LT09. In week 5 the second half of the lecture will be a MOLE quiz. Week 11 will be an invited lecture.

## Week 01: 

#### Lecture 01 - Introduction ([pdf](https://drive.google.com/file/d/0B2HbOiEppVPMSzlYdVJ4WFFaUjQ/view?usp=sharing))

* Context and Hardware Trends
* Supercomputing
* Software and Parallel Computing
* Course Outline


#### Lecture 02 - Introduction to C ([pdf](https://drive.google.com/file/d/0B2HbOiEppVPMd2NkM2txQ2tJVlE/view?usp=sharing))

* Introduction to the C Programming Language
* Basic C Usage "Hello World"
* Functions and Scoping
* Arrays, Strings and Basic IO
* File IO

#### Additional Notes on Visual Studio ([pdf](https://drive.google.com/file/d/0B2HbOiEppVPMMW1ZY1Q0Q2MzY2M/view?usp=sharing))

* Visual Studio 2013 Overview

## Week 02: 

#### Lecture 03 - Memory ([pdf](https://drive.google.com/file/d/0B2HbOiEppVPMMzZ4U2doNUhDT2M/view?usp=sharing))

* Pointers
* Advanced use of Pointers
* Dynamically Managed Memory
* Structures
* Binary Files

#### Lecture 04 - Optimisation ([pdf](https://drive.google.com/file/d/0B2HbOiEppVPMSm8xYXk1YUViUk0/view?usp=sharing))

* Optimisation Overview
* Compute Bound Code
* Memory Bound Code

#### NSS - National Stduent Survey ([pdf](https://drive.google.com/file/d/0B2HbOiEppVPMRDFBSFRLaDJtUlk/view?usp=sharing))

## Week 03: 

#### Lecture 05 - OpenMP 

* Multi-core Systems and OpenMP
* Parallelising Loops
* Critical Sections and Synchronisation
* OpenMP Scoping
* Task Parallelism with Sections

#### Lecture 06 - OpenMP Part II 

* Parallel Reduction
* Scheduling
* Nesting

## Week 04: 

#### Lecture 07 - GPU Architectures 

* What is a GPU?
* General Purpose Computation on GPUs (and GPU History)
* GPU CUDA Hardware Model
* Accelerated Systems

#### Lecture 08 - Introduction to CUDA 

* CUDA Programming Model
* CUDA Device Code
* CUDA Host Code and Memory Management
* CUDA Compilation and execution in Visual Studio

## Week 05: 

#### Lecture 09 - CUDA Memory 

* Memory Hierarchy Overview
* Global Memory
* Constant Memory
* Texture and Read-only Memory
* Roundup & Performance Timing

#### MOLE QUIZ

## Week 06: 

#### Lecture 10 - CUDA Shared Memory 

* Shared Memory
* Shared Memory Bank Conflicts
* 2D Shared Memory Bank Conflicts
* Boundary Conditions for Shared Memory Loading
* Host-side Configurations for Shared Memory
* [Shared Memory Bank Conflict Calculator](https://drive.google.com/a/sheffield.ac.uk/file/d/0B2HbOiEppVPMYlVQU2t4Y3NJWUE/view?usp=sharing)

#### Lecture 11 - CUDA Performance 

* Global Memory Coalescing
* Global Memory Coalescing with the L1 Cache
* Occupancy and Thread Block Dimensions

## Week 07: 

#### Lecture 12 - Warp Level CUDA 

* Warp Scheduling and Divergence
* Atomics
* Warp Operations

#### Lecture 13 - Parallel Patterns 

* Parallel Patterns Overview
* Reduction
* Scan

## Week 08: 

#### Lecture 14 - Sorting and Libraries 

* Sorting Networks
* Merge and Bitonic Sort
* Thrust Parallel Primitives Library
* Applications of Sorting (binning)

#### Lecture 15 - CUDA Streams 

* Synchronous and Asynchronous execution 
* CUDA Streams
* Synchronisation
* Multi GPU Programming

## Easter Vacation

## Week 09: 

#### Lecture 16 and 17 - Performance Optimisation 

* Profiling Introduction
* The Problem
* Visual Profiler Guided Analysis
* Profiling in tha lab

## Week 10: BANK HOLIDAY 

## Week 11: Invited Talk

## Week 12: NO LECTURE

# Labs

Labs will take place on Tuesdays 9:00 until 10:50 in the Diamond High Spec Lab (DIA-206). Week 9 lab will be a MOLE quiz followed by assignment help. Week 11 (full lab) will be for assignment help. Assignment help will also be availble during any of the normal lab sessions. There will be no lab in week 12.

A [Lab FAQ document](https://docs.google.com/a/sheffield.ac.uk/document/d/1w4k87mKyJke4bfbWbUVT7rpio2hN7_RUXRDZIT93j9g/edit?usp=sharing) has been prepared with common questions. This will be continually updated throughout the course.

## Lab Register ##

The lab register **must** be completed by every student following the completion and review of the exercises. You should complete this only when you have completed the lab **and** reviewed the solutions. You are not expected to complete this during the lab class but you should complete it by the end of the teaching week.

Lab Register Link: [https://goo.gl/0r73gD](https://goo.gl/0r73gD)

#### Lab 01 - C Programming 

* Lab Sheet ([pdf](https://drive.google.com/file/d/0B2HbOiEppVPMUHp1N19RRlNZN3c/view?usp=sharing))
* Source Code ([zip](https://github.com/mondus/com4521/archive/Lab01_src.zip))
* Solution ([zip](https://github.com/mondus/com4521/archive/Lab01_sln.zip))

#### Lab 02 - Memory and Performance

* Lab Sheet ([web](./lab02/)) ([pdf](https://drive.google.com/file/d/0B2HbOiEppVPMMVhrQlZXLUNHTjQ/view?usp=sharing))
* Source Code ([zip](https://github.com/mondus/com4521/archive/Lab02_src.zip))
* Solution

#### Lab 03 - OpenMP

* Lab Sheet
* Source Code
* Solution

#### Lab 04 - Introduction to CUDA

* Lab Sheet
* Source Code
* Solution

#### Lab 05 - Memory

* Lab Sheet
* Source Code
* Solution

#### Lab 06 - Shared Memory and Occupancy

* Lab Sheet
* Source Code
* Solution
 
#### Lab 07 - Atomics and Primitives

* Lab Sheet
* Source Code
* Solution

#### Lab 08 - Libraries and Streams

* Lab Sheet
* Source Code
* Solution

#### Lab 09 - MOLE QUIZ 2,  Profiling and Assignment Help

* Assignment help
* Profiling your own code in the Diamond Lab

#### Lab 10 - CUDA OpenGL Interop

* Lab Sheet
* Source Code
* Solution

#### Lab 11 - Profiling and Assignment Help

* Assignment help
* Profiling your own code in the Diamond Lab

# Discussion, Announcements and Help

Discussion, announcements and help requests (outside of the labs) should be made via the modules public Gooogle Group.

[https://groups.google.com/a/sheffield.ac.uk/d/forum/com4521-group](https://groups.google.com/a/sheffield.ac.uk/d/forum/com4521-group)

# Calendar

You can add this calendar to your University of Sheffield Google Calendar by searching for COM4521 and COM6521

<iframe src="https://calendar.google.com/calendar/embed?src=sheffield.ac.uk_4gq0ug3uf8dlts9d21gp4l1des%40group.calendar.google.com&ctz=Europe/London" style="border: 0" width="800" height="600" frameborder="0" scrolling="no"></iframe>

# Recommended Reading

* Edward Kandrot, Jason Sanders, "CUDA by Example: An Introduction to General-Purpose GPU Programming", Addison Wesley 2010.
* Brian Kernighan, Dennis Ritchie, “The C Programming Language (2nd Edition)”, Prentice Hall 1988.
* NVIDIA, [CUDA C Programming Guide](http://docs.nvidia.com/cuda/cuda-c-programming-guide/)
