---
title: Dr Paul Richmond - COM4521 & COM 6521 Introduction to Parallel Computing with GPUs
layout: homepage
---

Welcome to the 2020 module page for COM4521/COM6521.

# About the Course

Accelerator architectures are discrete processing units which supplement a base processor with the objective of providing advanced performance at lower energy cost. Performance is gained by a design which favours a high number of parallel compute cores at the expense of imposing significant software challenges. This module looks at accelerated computing from multi-core CPUs to GPU accelerators with many TFlops of theoretical performance. The module will give insight into how to write high performance code with specific emphasis on GPU programming with NVIDIA CUDA GPUs. A key aspect of the module will be understanding what the implications of program code are on the underlying hardware so that it can be optimised.
 
The modules aims, objectives and assessment details are available on the [modules public teaching page](http://www.dcs.shef.ac.uk/intranet/teaching/public/modules/level4/com4521.html).

# Lecture and Lab Location

Lectures will take place on Tuesdays 9:00 until 11:00 in Broad Lane Lecture Theatre 7 (BROAD-LT7). In week 5 the **first** half of the lecture (9:00) will be a MOLE quiz in Diamond Computer Room 3. In week 10 the **second** half of the lecture (10:00) will be a MOLE quiz in Diamond Computer Room 1.

Labs are double taught, you only need to attend one two lab session per week. You should have been allocated a group by the teaching admin team. 

* Group 1 lab is run on Tuesdays 13:00-15:00 (with no lab in week 5). 
* Group 2 lab is Wednesday 9:00-11:00 (in week 6 the lab is on Friday 20th March 10:00-1200, and there is no lab in week 10).

# Lecture and Lab Material

Lectures notes and labs are available via [Google Drive](https://drive.google.com/drive/u/1/folders/1AY762sikTwFzg9IhmQfbfHe_oWS37314) (you will need to login with your university credentials) or via the links below. Lecture material will be made available shortly before the lecture each week. Lab solutions will be released after both labs have finished.

# Software for the Module

The module programming exercises are designed to be completed in the Diamond high spec compute room. The room has recently been upgraded with Visual Studio 2019 and CUDA 10. If you intend to use your own machine for programming exercises (on the CUDA part of the module) then you **must** install the latest Community version of Visual Studio 2019 before you install the CUDA toolkit.

If you want to complete the exercises in Linux then example Makefiles will be provided with the lab starting code and solution. It is not possible to build Linux CUDA programs in the high spec compute room, however there will be lab instructions on how to remotely build and execute CUDA code for the Universities High Performance (HPC) computing system (ShARC).

# Computers and Labs Available

The Diamond high spec compute room is booked for the lab classes and is always available to you during standard lab hours. Our side of lab times the room has a tendency to be quite busy, especially towards the end of term when assignments are due. The following options are available to you;

* The Diamond high spec compute room (compute room 4)- The room has been block booked for participants in this module and Computer Science project students ([See list of bookings]()). If the room is occupied then machines must be  vacated to provide space for you. If people are unwilling to move then consult the Diamond reception desk.
* Diamond loanable high spec laptops - details to follow
* Your own Windows/Linux machine - Follow the instructions under "software for this module".
* Your own Linux machine - Example makefiles are provided with the lab handouts and solutions. You will need to install CUDA 10.0
* [ShARC](./sharc) - In week 5, a self paced lab class (outside of normal lab hours) will be provided to guide you through how to use the ShARC facility to submit GPU jobs to the Universities HPC system. You can ask for assistance with this lab during any normal lab hours.

# Lab Attendance Checking and Module Feedback

You are required to complete a lab register to indicate your progress with the lab exercises each week. You should fill this in once you have completed the lab exercises and reviewed the solutions. It is not expected that you will be able to complete all of the lab exercises within the two hour lab slot, you are expected to undertake independent study but you must try and complete the labs before the start of the next lab. The purpose of the lab register is to monitor class progress to be able provide feedback, clarifications on difficult areas and additional assistance to you. please use the additional comments section to highlight if you found the content useful, too easy or difficult, or would you like some aspect of the course to be clarified?

[Lab Register and Feedback Form](https://goo.gl/0r73gD)

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

### Lecture 01 - Introduction 

* Context and Hardware Trends
* Supercomputing
* Software and Parallel Computing
* Course Outline

### Lecture 02 - Introduction to C 

* Introduction to the C Programming Language
* Basic C Usage "Hello World"
* Functions and Scoping
* Arrays, Strings and Basic IO
* File IO
* Visual Studio 2017 Overview 

### Lab 01 - Introduction to Visual Studio and C Programming 

* Lab Sheet
* Source Code
* Solution

## Week02: 

### Lecture 03 - Memory 

* Pointers
* Advanced use of Pointers
* Dynamically Managed Memory
* Structures
* Binary Files

### Lecture 04 - Optimisation 

* Optimisation Overview
* Compute Bound Code
* Memory Bound Code

### Lab 02 - Memory and Performance

* Lab Sheet
* Source Code
* Solution

## Week 03

### Lecture 05 - OpenMP 

* Multi-core Systems and OpenMP
* Parallelising Loops
* Critical Sections and Synchronisation
* OpenMP Scoping
* Task Parallelism with Sections

### Lecture 06 - OpenMP Part II 

* OpenMP TIming
* Parallel Reduction
* Scheduling
* Nesting

### Lab 03 - OpenMP

* Lab Sheet
* Source Code
* Solution

## Week 04

### Lecture 07 - GPU Architectures

* What is a GPU?
* General Purpose Computation on GPUs (and GPU History)
* GPU CUDA Hardware Model
* Accelerated Systems

### Lecture 08 - Introduction to CUDA

* CUDA Programming Model
* CUDA Device Code
* CUDA Host Code and Memory Management
* CUDA Compilation and execution in Visual Studio

### Lab 04 - Introduction to CUDA

* Lab Sheet
* Source Code
* Solution


## Week 05

### MOLE Quiz 1 - No lectures

### Lab 5

* No lab on Tuesday 10/03/202
* Wednesday 11/03/2020 9:00-11:00 Drop in Assignment help open to all


## Week 6

### Lecture 09 - CUDA Memory 

* Memory Hierarchy Overview
* Global Memory
* Constant Memory
* Texture and Read-only Memory
* Roundup & Performance Timing



### Lab 05 - Memory

* Lab Sheet
* Source Code
* Solution


## Week 06

### Lecture 10 - CUDA Shared Memory ([pdf](https://drive.google.com/file/d/1CN977UxqI5DbVpIK5YxKKuSalnpv-7Wi/view?usp=sharing))

* Shared Memory
* Shared Memory Bank Conflicts
* 2D Shared Memory Bank Conflicts
* Boundary Conditions for Shared Memory Loading
* Host-side Configurations for Shared Memory
* [Shared Memory Bank Conflict Calculator](https://drive.google.com/file/d/173St-SBa9J3gtvt3CdTVrhPZqE-fNbY_/view?usp=sharing)

### Lecture 11 - CUDA Performance ([pdf](https://drive.google.com/file/d/1aeoY76E9mIlBdgWsHvg5NpmQEdpaf0Cp/view?usp=sharing))

* Lab Sheet
* Source Code
* Solution

### Lab 06 - Shared Memory and Occupancy

* [Lab Sheet](https://drive.google.com/file/d/1csN6DbbE6ooXIOVk4YVLpwftJhS3aiE-/view?usp=sharing)
* [Source Code](https://github.com/mondus/com4521/archive/Lab06_src.zip)
* [Solution](https://github.com/mondus/com4521/archive/Lab06_sln.zip)
* [Solution Explanation](https://drive.google.com/file/d/1Trsmttmng_Bjqdhrz2Hel2VbqOOfyN03/view?usp=sharing)

## Week 07

### Lecture 12 - Warp Level CUDA ([pdf](https://drive.google.com/file/d/1wQm3qegPIp7I5XG0eH_z_HwhLXkAdU4E/view?usp=sharing))

* Warp Scheduling and Divergence
* Atomics
* Warp Operations
* [Excel sheet for SM conflicts](https://drive.google.com/file/d/1DAnIEcW7vixm7zZMIevaIMW7Hf2UGiA9/view?usp=sharing)

### Lecture 13 - Parallel Patterns ([pdf](https://drive.google.com/file/d/1AeJCT0cvIPC5fPXsBxHoheoXHDMlzhRm/view?usp=sharing))

* Parallel Patterns Overview
* Reduction
* Scan

### Lab 07 - Atomics and Primitives

* Lab Sheet
* Source Code
* Solution

## EASTER VACTION

## Week 8

### Lecture 14 and 15 - Performance Optimisation ([pdf](https://drive.google.com/file/d/1fCY4IYtgEu1JszlvkL7u_n-K9Nda-Dzq/view?usp=sharing))

* Profiling Introduction
* The Problem
* Visual Profiler Guided Analysis
* Profiling in the lab ([available as a separate download](https://drive.google.com/file/d/13yUe3-1bk-umAT84LJxnOaD0DwSni8Q3/view?usp=sharing))

### Lab 08 - ShARC Lab

* [Online Lab Guide](./sharc)
* [Profile Lecture Example Code](https://github.com/mondus/com4521/archive/lab08_src.zip)

## Week 09

### Lecture 16 - Sorting and Libraries ([pdf](https://drive.google.com/file/d/1gZRro8vBrcpFdRTZ6vQwU3PGY8bKK6-1/view?usp=sharing))

* Sorting Networks
* Merge and Bitonic Sort
* Thrust Parallel Primitives Library
* Applications of Sorting (binning)

### Lecture 17 - CUDA Streams ([pdf](https://drive.google.com/file/d/13IodcFY0rrZ6iWgmA_IYaJ0Ihpdb9-oL/view?usp=sharing))

* Synchronous and Asynchronous execution 
* CUDA Streams
* Synchronisation
* Multi GPU Programming

### Lab 09 - Libraries and Streams

* [Lab Sheet](https://drive.google.com/file/d/1X6TiotIwEIyxjmi87dmmgm3ENpSHlyE7/view?usp=sharing)
* [Source Code](https://github.com/mondus/com4521/archive/Lab08_src.zip)
* [Solution](https://github.com/mondus/com4521/archive/Lab08_sln.zip)

## Week 10

### Lecture 18 - Invited Talk

### 1st May 2018 (09:00) - MOLE QUIZ (Diamond high spec compute room, DIA-002, Computer room 2)

### Lab 10 - Assignment Help

## Week 11: BANK HOLIDAY

### Lab 11 - OpenGL and Assignment Help

* [Lab Sheet](https://drive.google.com/file/d/19MZ-oVYj2hOB9ZkW3havOOZMQeaJm_w3/view?usp=sharing)
* [Source Code](https://github.com/mondus/com4521/archive/Lab10_src.zip)
* [Solution](https://github.com/mondus/com4521/archive/lab10_sln.zip)

## Week 12: No lectures or labs

# Calendar

You can add this calendar to your University of Sheffield Google Calendar by searching for COM4521 and COM6521

<iframe src="https://calendar.google.com/calendar/embed?src=sheffield.ac.uk_4gq0ug3uf8dlts9d21gp4l1des%40group.calendar.google.com&ctz=Europe/London" style="border: 0" width="800" height="600" frameborder="0" scrolling="no"></iframe>

# Recommended Reading

* Edward Kandrot, Jason Sanders, "CUDA by Example: An Introduction to General-Purpose GPU Programming", Addison Wesley 2010.
* Brian Kernighan, Dennis Ritchie, “The C Programming Language (2nd Edition)”, Prentice Hall 1988.
* NVIDIA, [CUDA C Programming Guide](http://docs.nvidia.com/cuda/cuda-c-programming-guide/)
