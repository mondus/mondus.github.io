---
title: Dr Paul Richmond - COM4521 & COM 6521 Introduction to Parallel Computing with GPUs
layout: homepage
---


# About the Course

Welcome to the 2020 module page for COM4521/COM6521.

Accelerator architectures are discrete processing units which supplement a base processor with the objective of providing advanced performance at lower energy cost. Performance is gained by a design which favours a high number of parallel compute cores at the expense of imposing significant software challenges. This module looks at accelerated computing from multi-core CPUs to GPU accelerators with many TFlops of theoretical performance. The module will give insight into how to write high performance code with specific emphasis on GPU programming with NVIDIA CUDA GPUs. A key aspect of the module will be understanding what the implications of program code are on the underlying hardware so that it can be optimised.
 
The modules aims, objectives and assessment details are available on the [modules public teaching page](http://www.dcs.shef.ac.uk/intranet/teaching/public/modules/level4/com4521.html).

# Lecture and Lab Location

Lectures will usually take place on Tuesdays 9:00 until 11:00 in Broad Lane Lecture Theatre 7 (BROAD-LT7). In week 5 the **first** half of the lecture (9:00) will be a MOLE quiz in Diamond Computer Room 3. In week 10 the **second** half of the lecture (10:00) will be a MOLE quiz in Diamond Computer Room 1. *Note: Any other changes to lectures will be added to the course calendar with an email sent to the course mailing list.*

Labs are double taught, you only need to attend one two lab session per week. You should have been allocated a group by the teaching admin team. 

* Group 1 lab is run on Tuesdays 13:00-15:00 (on week 5 the lab is 11:00-13:00). 
* Group 2 lab is Wednesday 9:00-11:00 (in week 6 the lab is on Friday 20th March 10:00-1200, and there is no lab in week 10).

# Lecture and Lab Material

Lectures notes and labs are available via [Google Drive](https://drive.google.com/drive/u/1/folders/1AY762sikTwFzg9IhmQfbfHe_oWS37314) (you will need to login with your university credentials) or via the links below. Lecture material will be made available shortly before the lecture each week. Lab solutions will be released after both labs have finished.

# Software for the Module

The module programming exercises are designed to be completed in the Diamond high spec compute room. The room has recently been upgraded with Visual Studio 2017 and CUDA 10. If you intend to use your own machine for programming exercises (on the CUDA part of the module) then you **must** install the latest Community version of Visual Studio 2019 before you install the CUDA toolkit. Some versions of Visual Studio 2017 are not compatible with CUDA.

If you want to complete the exercises in Linux then example Makefiles will be provided with the lab starting code and solution. It is not possible to build Linux CUDA programs in the high spec compute room, however there will be lab instructions on how to remotely build and execute CUDA code for the Universities High Performance (HPC) computing system (ShARC).

# Computers and Labs Available

The Diamond high spec compute room is booked for the lab classes and is always available to you during standard lab hours. Our side of lab times the room has a tendency to be quite busy, especially towards the end of term when assignments are due. The following options are available to you;

* The Diamond high spec compute room (compute room 4)- The room has been block booked for participants in this module and Computer Science project students ([See list of bookings](https://docs.google.com/spreadsheets/d/1sIeNWsJgY_ylXT-yW1qtv2bP8zkr_zE0L5lOb30ZTMs/edit?usp=sharing)). If the room is occupied then machines must be  vacated to provide space for you. If people are unwilling to move then consult the Diamond reception desk.
* Diamond **bookable** high spec laptops - Available to borrow from the lockers on Diamond Level 4 (for use within the Diamond building only) after completing an induction. To arrange an induction contact [James Screaton](mailto:j.screaton@sheffield.ac.uk).
* Your own Windows/Linux machine - Follow the instructions under "software for this module".
* Your own Linux machine - Example makefiles are provided with the lab handouts and solutions. You will need to install CUDA 10.0
* ShARC - In week 8, a lab will be provided to guide you through how to use the ShARC facility to submit GPU jobs to the Universities HPC system.

# Lab Attendance Checking and Module Feedback

You are required to complete a lab register to indicate your progress with the lab exercises each week. You should fill this in once you have completed the lab exercises and reviewed the solutions. It is not expected that you will be able to complete all of the lab exercises within the two hour lab slot, you are expected to undertake independent study but you must try and complete the labs before the start of the next lab. The purpose of the lab register is to monitor class progress to be able provide feedback, clarifications on difficult areas and additional assistance to you. please use the additional comments section to highlight if you found the content useful, too easy or difficult, or would you like some aspect of the course to be clarified?

[Lab Register and Feedback Form](https://bit.ly/3b77Lhy)

*Note: There is a form section per lab class. Please only complete this form once and edit your last submission each week to update.*

# Feedback

You will receive feedback from the lab registers during lectures and lab classes. Feedback will be provided through the MOLE quizes and via marking of the assignment. Importantly your first assignment will provide feedback which you can use to improve your assignment 2 hand in.

# Assignments

There are two assignments for the module which contribute 80% of the total module mark

* Part 1 (30% of the assignment total) - Released Week 3, Due Monday week 7 (23/03/2020) at 15:00
* Part 2 (70% of the assignment total) - Released Week 6, Due Monday week 12 (18/05/2020) at 15:00

The remaining 20% of the module mark is from two mole quizes which are 

* Week 5 - During the first half of the lecture (9:00 10/03/2020) in Diamond compute room 3
* Week 10 - During the second half of the lecture (10:00 05/05/2020) in Diamond compute room 1

# DDP students and staff candidates

PhD students and research/academic staff are not required to undertake assessment but are asked to complete the lab feedback form as evidence of participation in the module. You are free to attend either lab session subject to availability however please note that the lab space is prioritised for undergraduate and masters students. 

# Discussion, Announcements and Requests for Help

A [Google group](https://groups.google.com/a/sheffield.ac.uk/d/forum/com4521-group) has been created for announcements, help and discussion. Any changes to timetabling will be made via this group. All students enrolled on the module on the 29th January 2020 have been added to this group already. If you have transferred via Add/Drop then you will need to manually join the group yourself. The group is monitored by the teaching staff (including lab assistants) as well as additional PhD students who can provide help with the lab classes or assignment. This is a public (within the University of Sheffield) forum and therefore you should not post assignment code. If you require personal assistance then you should request this during the lab hours. Any lab class can be used for assignment help in addition to the lab exercises which are set.

[https://groups.google.com/a/sheffield.ac.uk/d/forum/com4521-group](https://groups.google.com/a/sheffield.ac.uk/d/forum/com4521-group)


# Teaching Material

## Week 01

### Lecture 01 - Introduction ([pdf](https://drive.google.com/open?id=11_tQK9gFufXWy4b5wWlwv6QEnUFSu48u))

* Context and Hardware Trends
* Supercomputing
* Software and Parallel Computing
* Course Outline

### Lecture 02 - Introduction to C ([pdf](https://drive.google.com/open?id=1XTLiobUquK3exL8LypViyh-QITw__WqK))

* Introduction to the C Programming Language
* Basic C Usage "Hello World"
* Functions and Scoping
* Arrays, Strings and Basic IO
* File IO
* Extra Material: Visual Studio 2017 Overview ([pdf](https://drive.google.com/open?id=1qO9UURhX3tFKzZmkCbMO3nnKemIxssxJ))

### Lab 01 - Introduction to Visual Studio and C Programming 

* [Lab Sheet](https://drive.google.com/open?id=10fxV71JuTdhe4Vu6WIzcoeckiy6TOa4z)
* [Source Code](https://github.com/mondus/com4521/archive/Lab01_src.zip)
* [Solution](https://github.com/mondus/com4521/archive/Lab01_sln.zip)

## Week02: 

### Lecture 03 - Memory ([pdf](https://drive.google.com/open?id=1gJGZvDRfFYVN1sFxXR-66QrL-lpdywEL))

* Pointers
* Advanced use of Pointers
* Dynamically Managed Memory
* Structures
* Binary Files

### Lecture 04 - Optimisation ([pdf](https://drive.google.com/open?id=11BGw2468XqRscLEPn9eT7jIh3aQ-VO74))

* Optimisation Overview
* Compute Bound Code
* Memory Bound Code

### Lab 02 - Memory and Performance

* [Lab Sheet](https://drive.google.com/open?id=1cNzLsdZUbHKJSh5eERzdmd9mLYbS1CFN)
* [Source Code](https://github.com/mondus/com4521/archive/Lab02_src.zip)
* [Solution](https://github.com/mondus/com4521/archive/Lab02_sln.zip)

## Week 03

### Lecture 05 - OpenMP ([pdf](https://drive.google.com/open?id=1Xw_NP923Go_VXUNFIOMVZB02AdL8r2IC))

* Multi-core Systems and OpenMP
* Parallelising Loops
* Critical Sections and Synchronisation
* OpenMP Scoping
* Task Parallelism with Sections

### Lecture 06 - OpenMP Part II ([pdf](https://drive.google.com/open?id=1sYG1xrjRNvSsvoXvycL6l4714mfWtkmq))

* OpenMP TIming
* Parallel Reduction
* Scheduling
* Nesting

### Lab 03 - OpenMP

* [Lab Sheet](https://drive.google.com/open?id=1wR9zEYKdKyg1UhqvflDZY46NV7rvo8ME)
* [Source Code](https://github.com/mondus/com4521/archive/Lab03_src.zip)
* [Solution](https://github.com/mondus/com4521/archive/Lab03_sln.zip)

## Week 04

### Lecture 07 - GPU Architectures ([pdf](https://drive.google.com/open?id=1TJwdnBiYieouUMN32wsiruKLjn9PJoIM))

* What is a GPU?
* General Purpose Computation on GPUs (and GPU History)
* GPU CUDA Hardware Model
* Accelerated Systems

### Lecture 08 - Introduction to CUDA ([pdf](https://drive.google.com/open?id=1yA8X9yuCMBGpjetIEI6JEhNpGE0704c4))

* CUDA Programming Model
* CUDA Device Code
* CUDA Host Code and Memory Management
* CUDA Compilation and execution in Visual Studio

### Lab 04 - Introduction to CUDA

* [Lab Sheet](https://drive.google.com/open?id=1Mr-K6IdOuzeckEDG3RjJ4qmaNO-Do3qK)
* [Source Code](https://github.com/mondus/com4521/archive/Lab04_src.zip)
* [Solution](https://github.com/mondus/com4521/archive/Lab04_sln.zip)


## Week 05

### Quiz BEFORE lecture 9

### Lecture 09 - CUDA Memory ([pdf](https://drive.google.com/open?id=1m6qrDEICELdp8SMhXEzBxsJP-Afy36ck))

* Memory Hierarchy Overview
* Global Memory
* Constant Memory
* Texture and Read-only Memory
* Roundup & Performance Timing

### Lab 5 - CUDA Memory

* [Lab Sheet](https://drive.google.com/open?id=1qys-DrrvJgA1wPKDlKdQIvjYynQIhRj8)
* [Source Code](https://github.com/mondus/com4521/archive/Lab05_src.zip)
* [Solution](https://github.com/mondus/com4521/archive/Lab05_sln.zip)


## Week 6

### Encore

Weeks 6 lectures (e.g. Lecture 10 and 11) are pre-recorded on encore. Follow the link below for the lecture content.

[https://echo360.org.uk/media/70096996-3c13-4b31-970c-9b1b384ba0d9/public](https://echo360.org.uk/media/70096996-3c13-4b31-970c-9b1b384ba0d9/public)

### Lecture 10 - CUDA Shared Memory [pdf](https://drive.google.com/open?id=1CN977UxqI5DbVpIK5YxKKuSalnpv-7Wi)

* Shared Memory
* Shared Memory Bank Conflicts
* 2D Shared Memory Bank Conflicts
* Boundary Conditions for Shared Memory Loading
* Host-side Configurations for Shared Memory
* Shared Memory Bank Conflict Calculator

### Lecture 11 - CUDA Performance [pdf](https://drive.google.com/open?id=1aeoY76E9mIlBdgWsHvg5NpmQEdpaf0Cp)

* Global Memory Coalescing
* Global Memory Coalescing with the L1 Cache
* Occupancy and Thread Block Dimensions

### Lab 6 - Shared Memory

* [Lab Sheet](https://drive.google.com/open?id=1vDkYtG3DiEZxFqGxSaUh6sep-wgaJkjF)
* [Source Code](https://github.com/mondus/com4521/archive/Lab06_src.zip)
* [Solution](https://github.com/mondus/com4521/archive/Lab06_sln.zip)
* [Solution Explanation](https://drive.google.com/open?id=1xDo9HAYDPax8c3d3EFffKoZH5nUV7Vjm)

## Week 07

Due to COVID-19 Week 7 Has been removed from the teaching semester.

## EASTER VACATION

## Week 8

## Encore

Weeks 8 lectures are pre-recorded on encore. Follow the link below for the lecture content.

[https://echo360.org.uk/media/2f39e288-7206-4cb1-99b8-7b481dc03cec/public](https://echo360.org.uk/media/2f39e288-7206-4cb1-99b8-7b481dc03cec/public)

### Lecture 12 - Warp Level CUDA ([pdf](https://drive.google.com/open?id=1rn8nwnDcgT4x8Ld1vFfXPE4k38xEnlxC))

* Warp Scheduling and Divergence
* Atomics
* Warp Operations
* Excel sheet for SM conflicts

### Lecture 13 - Parallel Patterns ([pdf](https://drive.google.com/open?id=1q0kCiPk6p6wWU0zDMuFWetDVtMIBWQfP))

* Parallel Patterns Overview
* Reduction
* Scan

### Lab 07 - Atomics and Primitives

* [Lab Sheet](https://drive.google.com/open?id=1L-1v2QROFVbR0gJk7jnrJCRUxZA8gUV2)
* [Source Code](https://github.com/mondus/com4521/archive/Lab07_src.zip)
* Solution

## Week 9


### Encore

Weeks 9 lectures are pre-recorded on encore. Follow the link below for the lecture content.

[https://echo360.org.uk/media/1df87c02-cf1c-4b5d-818a-c2596f8185b3/public](https://echo360.org.uk/media/1df87c02-cf1c-4b5d-818a-c2596f8185b3/public)

### Lecture 14 and 15 - Performance Optimisation ([pdf](https://drive.google.com/open?id=1MpXx4TuEwomtdZkJkIVnW5nA44DINFM0))

* Profiling Introduction
* The Problem
* Visual Profiler Guided Analysis
* Profiling on instancehub ([available as a separate download](https://drive.google.com/open?id=1qQw0Ut2lggbdJm8PF_TO0xsJZlpPKLW-))

### Lab 08 - Profiling Example

Note: As labs have moved to instancehub there is no need to undertake a lab on ShARC which is extreemly busy with remote research work.

* [Profile Lecture Example Code](https://github.com/mondus/com4521/archive/lab09_sln.zip)


## Week 10

### Encore

Weeks 9 lectures are pre-recorded on encore. Follow the link below for the lecture content.

[https://echo360.org.uk/media/5eacecd1-eb25-4850-b378-019549500bb7/public](https://echo360.org.uk/media/5eacecd1-eb25-4850-b378-019549500bb7/public)

### Lecture 16 - Sorting and Libraries ([pdf](https://drive.google.com/open?id=1lMx_jEFtOxl02FRh09oxHRUHoMC5bwT5))

* Sorting Networks
* Merge and Bitonic Sort
* Thrust Parallel Primitives Library
* Applications of Sorting (binning)

### Lecture 17 - CUDA Streams ([pdf](https://drive.google.com/open?id=1zhGV8WmMlsLI-PpTYO6b2i3XaDH6cRRe))

* Synchronous and Asynchronous execution 
* CUDA Streams
* Synchronisation
* Multi GPU Programming

### Lab 09 - Libraries and Streams

* [Lab Sheet](https://drive.google.com/open?id=1oksunLWVfePbXrRRmnNF_njlBlyKahdV)
* [Source Code](https://github.com/mondus/com4521/archive/Lab08_src.zip)
* Solution

## Week 11

### MOLE Quiz during lecture time

This MOLE quiz will no longer be assessed but can still be taken and the answeres reviewed. It is **stronly** encouraged to take this quiz as it provides formative feedback which will help you to undertsnad your learning.

### Lab 10 - Assignment Help

## Week 12:

## No Lectures

Please Find below a list of previous invited lectures

* [Acclerating Road Network Simulations using GPUs](https://echo360.org.uk/media/de75ffe6-c839-49de-af50-ddb270dd529f/public)
* [Optimising Pedestrian Simulations](https://echo360.org.uk/media/6f8ed7dd-f3d8-4c25-acf2-03c36e40ea9e/public)

### Lab 11 - Optional OpenGL Lab and Assignment Help

*Note: The OpenGL lab is only suitable for those who have completed the undergraduate Computer Graphics module. The content of this lab is entirely optional and is not assesed as part of the module.*

* [Lab Sheet](https://drive.google.com/open?id=1q32RwV1XiiqplIut17ovO_OQJ3w83DzK)
* [Source Code](https://github.com/mondus/com4521/archive/Lab10_src.zip)
* Solution

# Calendar

You can add this calendar to your University of Sheffield Google Calendar by searching for COM4521 and COM6521

<iframe src="https://calendar.google.com/calendar/embed?src=sheffield.ac.uk_4gq0ug3uf8dlts9d21gp4l1des%40group.calendar.google.com&ctz=Europe/London" style="border: 0" width="800" height="600" frameborder="0" scrolling="no"></iframe>

# Recommended Reading

The following are useful resources but not required reading.

* Edward Kandrot, Jason Sanders, "CUDA by Example: An Introduction to General-Purpose GPU Programming", Addison Wesley 2010.
* Brian Kernighan, Dennis Ritchie, “The C Programming Language (2nd Edition)”, Prentice Hall 1988.
* NVIDIA, [CUDA C Programming Guide](http://docs.nvidia.com/cuda/cuda-c-programming-guide/)
