---
title: Dr Paul Richmond - COM4521 & COM 6521 Introduction to Parallel Computing with GPUs
layout: homepage
---


# Course Information

Welcome to the 2020/2021 module page for COM4521/COM6521 Parallel Computing with GPUs.

Accelerator architectures are discrete processing units which supplement a base processor with the objective of providing advanced performance at lower energy cost. Performance is gained by a design which favours a high number of parallel compute cores at the expense of imposing significant software challenges. This module looks at accelerated computing from multi-core CPUs to GPU accelerators with many TFlops of theoretical performance. The module will give insight into how to write high performance code with specific emphasis on GPU programming with NVIDIA CUDA GPUs. A key aspect of the module will be understanding what the implications of program code are on the underlying hardware so that it can be optimised.
 
The modules aims, objectives and assessment details are available on the [modules public teaching page](http://www.dcs.shef.ac.uk/intranet/teaching/public/modules/level4/com4521.html).

## Software for the Module

The module programming exercises are designed to be completed on PCs in the Diamond compute labs. As the modules teaching is online these machines are available via virtual desktop. All Diamond compute lab machines have Visual Studio 2019 and CUDA 11.1 If you intend to use your own machine for programming exercises (on the CUDA part of the module) then you **must** install the latest Community version of Visual Studio 2019 **before** you install the CUDA 11.1 toolkit.

If you want to complete the exercises in Linux then example Makefiles will be provided with the lab starting code and solutions. It is not possible to build Linux CUDA programs on PCs in the Diamond compute labs.

## Computers and Labs Available

As the module requires access to a machine with a GPU the following have been made available to you.

* Diamond Virtual Computer Lab 1 - This is reserved for exclusive access during the scheduled lab hours. You can access this lab by opening [myTimetable](https://cmisgonext.sheffield.ac.uk/Web/Timetable) and selecting the COM4521/COM6521 lab session which provides a link to the virtual room. The machines in this room are the same as the Diamond all in one machines and have a NVIDIA GTX1050 GPU.
* Diamond High Spec Lab Reservation - This is reserved for exclusive access during the scheduled lab hours. You can access this lab by opening [myTimetable](https://cmisgonext.sheffield.ac.uk/Web/Timetable) and selecting the COM4521/COM6521 lab session which provides a link to the virtual room. The machines in this room are the same as the Diamond High Spec lab and have an NVIDIA Quadro P4000.
* [Diamond High Spec Lab - Computer Room 4](https://www.sheffield.ac.uk/findapc/rdp/room/4/pcs) - This room can not be reserved but machines can be requested. These machines have slightly higher capability GPUs (Quadro P4000) but are limited in availability.
* [Any other Diamond Computer Lab](https://www.sheffield.ac.uk/findapc/now) - These machines can be requested at any time and have GTX 1050s.
* Your own Windows/Linux machine - Follow the instructions under "software for this module".

## Course Attendance Monitoring

Lab attendance is recorded through Blackboard collaborate. You are expected to attend labs to get assistance form the module leader and course demonstrators. It is not possible to properly understand the course material without completing the labs and reviewing the solutions. If you do not complete the labs then you will find the assignment difficult.

## Lab class Guide

Assistance with the course material is provided through online labs. Each week is designed to provide support for a particular set of lectures and lab material. You are however free to ask about any of the lab content or assignment help in any of the lab classes.

[Link to the lab class guide](./lab_guide)


## Course Assessment

In response to student feedback the number of assignments has been reduced to a single assignment this year which reflects the reduced number of learning objectives for the module. The assignment will be released Monday the 1st March 2021 (week 4) and is due 17:00 on Monday 17th May (week 12). The assignment forms 80% of your mark. You are expected to ask for feedback on your assignment work during the scheduled lab classes.

The remaining 20% of the module mark is from two mole quizes which can be taken remotely **only at the specified times**

* Week 5 - During the first half of the lab (11:00-12:00 08/03/2021)
* Week 9 - During the first half of the lab (11:00-12:00 26/04/2021)

## DDP students and Staff Candidates

PhD students and research/academic staff are not required to undertake assessment but DDP students are expected to attend labs as evidence of participation in the module.

## Discussion, Announcements and Requests for Help

A [Google group](https://groups.google.com/a/sheffield.ac.uk/d/forum/com4521-group) has been created for announcements, help and discussion. Any important announcements relating to the module will be made via this group. All students enrolled on the module on the 4th February 2021 have been added to this group already. If you have transferred via Add/Drop then you will need to manually join the group yourself. The group is monitored by the teaching staff (including lab assistants) as well as additional PhD students who can provide help. The purpose of the mailing list is to ask for general support and guidance with the course material (e.g. with concepts and ideas) rather than posting your own code. You should not post your assignment code on this forum. If you require personal assistance with your assignment code then you should request this during the lab hours. Any lab class can be used for assignment help in addition to the lab exercises which are set each week.

[https://groups.google.com/a/sheffield.ac.uk/d/forum/com4521-group](https://groups.google.com/a/sheffield.ac.uk/d/forum/com4521-group)


# Course Material Material

Lectures are pre-recorded and are availble on the [COM4521  Parallel Computing with Graphical Processing Units Kaltura Channel](https://digitalmedia.sheffield.ac.uk/channel/COM4521+Parallel+Computing+with+Graphical+Processing+Units/201133333) or as downloadable pdfs on [Google Drive](https://drive.google.com/drive/folders/1XxXJdrzSP6XFwrzzEnNv1BLptfsgZOXu?usp=sharing). Each weeks practical activities (the labs) follow the ideas presented in the lectures so it is important that you follow the lecture and lab timetable below.

## Week 01

### Lecture 01 - Introduction 

* Course Context ([pdf](https://drive.google.com/file/d/18PDhCWL_TQqntVqPTTHVeWJoZyF54Sf2/view?usp=sharing), [recording](https://digitalmedia.sheffield.ac.uk/media/Lecture+01+-+Part+01+-+Course+Context/1_4ozidnx3))
* Supercomputing and Software ([pdf](https://drive.google.com/file/d/1oMgIPthO-N7EyllFrxol-zkF19J5Kh75/view?usp=sharing), [recording](https://digitalmedia.sheffield.ac.uk/media/Lecture+01+-+Part+02+-+Super+Computing+and+Software/1_3cae6aog))
* Module Details ([pdf](https://drive.google.com/file/d/12g0vTczjQCzQj0Idpjpt3k1Od-z7Uo9W/view?usp=sharing), [recording](https://digitalmedia.sheffield.ac.uk/media/Lecture+01+-+Part+03+-+Module+Details/1_hx158hky))

### Lecture 02 - Introduction to C

* Introducing C ([pdf](https://drive.google.com/file/d/1_mL4lhg2sb7Ez4-BzFEele6MXggXBiUK/view?usp=sharing), [recording](https://digitalmedia.sheffield.ac.uk/media/Lecture+02+-+Part+01+-+Introducing+C/1_eakd0424))
* Functions and Scoping ([pdf](https://drive.google.com/file/d/1tM_1D7w0WuVcvzU8QrdaEaZIf7-cgs6R/view?usp=sharing), [recording](https://digitalmedia.sheffield.ac.uk/media/Lecture+02+-+Part+02+-+Functions+and+Scoping/1_cf4tnuln))
* Arrays, Strings and IO ([pdf](https://drive.google.com/file/d/1KqpjzKsc5QjPq-qDKueT1EQBaP8ZCZeJ/view?usp=sharing), [recording](https://digitalmedia.sheffield.ac.uk/media/Lecture+02+-+Part+03+-+Arrays+Strings+and+IO/1_60zchnsf))


### Lab 01 - Introduction to Visual Studio and C Programming 

* [Getting Started with Visual Studio 2019 Overview](https://drive.google.com/file/d/1BCpXw9Mr04DSkal7P_ARzMis78t3Pveu/view?usp=sharing)
* [Lab Sheet](https://drive.google.com/file/d/1DsU1uOsQqiBwDrNwpVH4yB5GyWBaia_x/view?usp=sharing)
* [Source Code](https://github.com/mondus/com4521/archive/Lab01_src.zip)
* [Solution](https://github.com/mondus/com4521/archive/Lab01_sln.zip)

## Week 02

### Lecture 03 - Memory 

* Pointers ([pdf](https://drive.google.com/file/d/1ek2YjPLMDwdtRJVlUrmPZ31SV6E7UWbV/view?usp=sharing), [recording](https://digitalmedia.sheffield.ac.uk/media/Lecture+03+-+Part+01+-+Pointers/1_2lxp7wyb))
* Advanced use of Pointers ([pdf](https://drive.google.com/file/d/1TuHaiow_oGjXOWvTy05CFY3lw0bwKh2Y/view?usp=sharing), [recording](https://digitalmedia.sheffield.ac.uk/media/Lecture+03+-+Part+02+-+Advanced+Pointers/1_v4x7d5sr))
* Dynamically Managed Memory ([pdf](https://drive.google.com/file/d/1tnGYCG48XOYMhUf78dJT-VT1kT4d6lFp/view?usp=sharing), [recording](https://digitalmedia.sheffield.ac.uk/media/Lecture+03+-+Part+03+-+Manual+Memory+Management/1_4j49qhoj))
* Structures and Binary Files ([pdf](https://drive.google.com/file/d/1Pl_wx-H9dDXfGfKEprxs6jg3RzrTSnVq/view?usp=sharing), [recording](https://digitalmedia.sheffield.ac.uk/media/Lecture+03+-+Part+04+-+Structures+and+Binary+Files/1_38omyxrt))

### Lecture 04 - Optimisation 

* Optimisation Overview ([pdf](https://drive.google.com/file/d/1wVdzbq9DL0S-qK0K1np084Mc8mF7CWNb/view?usp=sharing), [recording](https://digitalmedia.sheffield.ac.uk/media/Lecture+04+-+Part+01+-+Optmisation+Overview/1_z09qnv7q))
* Compute Bound Code ([pdf](https://drive.google.com/file/d/17xQZlwihTvo2vEEWPpb5k8EWOqXezz3U/view?usp=sharing), [recording](https://digitalmedia.sheffield.ac.uk/media/Lecture+04+-+Part+02+-+Compute+Bound+Code/1_t74gjrqg))
* Memory Bound Code ([pdf](https://drive.google.com/file/d/1pi7FnfWd_0YcMouXTnktV7Pu4BDXoEOh/view?usp=sharing), [recording](https://digitalmedia.sheffield.ac.uk/media/Lecture+04+-+Part+03+-+Memory+Bound+Code/1_eaa6z5dh))

### Lab 02 - Memory and Performance

* [Lab Sheet](https://drive.google.com/file/d/1JMqV-a5J2de0mUS961xrNsG1GUn4C8tr/view?usp=sharing)
* [Source Code](https://github.com/mondus/com4521/archive/Lab02_src.zip)
* [Solution](https://github.com/mondus/com4521/archive/Lab02_sln.zip)

## Week 03

### Lecture 05 - OpenMP 

* OpenMP Overview ([pdf](https://drive.google.com/file/d/1Y9EUh835wkh8bwMHyNhu0fzFQGlygGl1/view?usp=sharing), [recording](https://digitalmedia.sheffield.ac.uk/media/Lecture+05+-+Part+01+-+OpenMP+Overview/1_tr35veym))
* Loops and Critical Sections ([pdf](https://drive.google.com/file/d/1adfofgTWGOGqUwOuDgTS9OW_nVDeBS3n/view?usp=sharing), [recording](https://digitalmedia.sheffield.ac.uk/media/Lecture+05+-+Part+02+-+Loops+and+Critical+Sections/1_j4mfsl94))
* Scoping and Tasks ([pdf](https://drive.google.com/file/d/14RxdZl6x2GYiCjbbi_1g1j5B5GhlXfzA/view?usp=sharing), [recording](https://digitalmedia.sheffield.ac.uk/media/Lecture+05+-+Part+03+-+Scoping+and+Tasks/1_tfgpqt3a))

### Lecture 06 - OpenMP Part II 

* Parallel Reduction ([pdf](https://drive.google.com/file/d/1DhPA-mFid4mFkUkFsRacIjzrPPvqpQs2/view?usp=sharing), [recording](https://digitalmedia.sheffield.ac.uk/media/Lecture+06+-+Part+01+-+Parallel+Reductions/1_0wfcdxdy))
* Scheduling ([pdf](https://drive.google.com/file/d/1n86lfK9u96e6VaqxONkqFg0yTqbIqET-/view?usp=sharing), [recording](https://digitalmedia.sheffield.ac.uk/media/Lecture+06+-+Part+02+-+Scheduling/1_jbiq6pkl))
* Nesting and Summary ([pdf](https://drive.google.com/file/d/1V-ufrzqwAZPvIs6bXl0zt9wE6uJ9KUeT/view?usp=sharing), [recording](https://digitalmedia.sheffield.ac.uk/media/Lecture+06+-+Part+03+-+Nesting+and+Summary/1_m9hddu82))

### Lab 03 - OpenMP

* [Lab Sheet](https://drive.google.com/file/d/1ADMZfATvH17S2-XdLXQMcJwqf2I-wcAc/view?usp=sharing)
* [Source Code](https://github.com/mondus/com4521/archive/Lab03_src.zip)
* [Solution](https://github.com/mondus/com4521/archive/Lab03_sln.zip)

## Week 04

### Lecture 07 - GPU Architectures 

* Introduction to GPUs ([pdf](https://drive.google.com/file/d/1cGZgGCB27m6zBkqR7-P1Lo0Ce8z7LzYx/view?usp=sharing), [recording](https://digitalmedia.sheffield.ac.uk/media/Lecture+07+-+Part+01+-+Introduction+to+GPUs/1_p7q41uvc))
* Programming GPUs ([pdf](https://drive.google.com/file/d/13G5k7JxXWYkmKdf_f3m34173Z4QQZNNb/view?usp=sharing), [recording](https://digitalmedia.sheffield.ac.uk/media/Lecture+07+-+Part+02+-+Programming+GPUs/1_76m5dhjm))
* GPU Hardware ([pdf](https://drive.google.com/file/d/1Q5YBM8GZqXp4P3FR1yDSPKSN9LP3yFTk/view?usp=sharing), [recording](https://digitalmedia.sheffield.ac.uk/media/Lecture+07+-+Part+03+-+GPU+Hardware/1_t7dweiyp))


### Lecture 08 - Introduction to CUDA 

* The CUDA Programming Model ([pdf](https://drive.google.com/file/d/1p50MnSqyC-U1lls08GhVX-mW8TEuXqLb/view?usp=sharing), [recording](https://digitalmedia.sheffield.ac.uk/media/Lecture+08+-+Part+01+-+CUDA+Programming+Model/1_kbdt8jns))
* CUDA Device Code ([pdf](https://drive.google.com/file/d/1he_iuEuyo5nONhM9DtkMmVdQ1Zat1s86/view?usp=sharing), [recording](https://digitalmedia.sheffield.ac.uk/media/Lecture+08+-+Part+02+-+CUDA+Device+Code/1_q8zijjv4))
* CUDA Host Code and Memory Management ([pdf](https://drive.google.com/file/d/1-PPKh4g2-Pe8jITUsLbUO0A0SxwIGXtU/view?usp=sharing), [recording](https://digitalmedia.sheffield.ac.uk/media/Lecture+08+-+Part+03+-+CUDA+Host+Code+and+Memory+Management/1_g4zl8te4))

### Lab 04 - Introduction to CUDA

* [Lab Sheet](https://drive.google.com/file/d/1y5GnTyyp0wmBk1RRLep8oYs_HVMvAvxX/view?usp=sharing)
* [Source Code](https://github.com/mondus/com4521/archive/Lab04_src.zip)
* [Solution](https://github.com/mondus/com4521/archive/Lab04_sln.zip)


## Week 05

### Lecture 09 - CUDA Memory

* Memory Overview ([pdf](https://drive.google.com/file/d/1BxiovKdODm1OsRTsLzW0LyOj1CfBYVQX/view?usp=sharing), [recording](https://digitalmedia.sheffield.ac.uk/media/Lecture+09+-+Part+01+-+Memory+Overview/1_0pa748z1))
* Global and Constant Memory ([pdf](https://drive.google.com/file/d/1ZvdLGJJ3D_-DrEFsR6Sai-sA5WN-uuWT/view?usp=sharing), [recording](https://digitalmedia.sheffield.ac.uk/media/Lecture+09+-+Part+02+-+Global+and+Constant+Memory/1_fl15aonq))
* Read Only and Texture Memory ([pdf](https://drive.google.com/file/d/1bSk8km76Y0CXAcBhBypwknl8OGoXb0VT/view?usp=sharing), [recording](https://digitalmedia.sheffield.ac.uk/media/Lecture+09+-+Part+03+-+Read-Only+and+Texture+Memory/1_kiodtb5l))

### Quiz BEFORE Lab 5

### Lab 5 - CUDA Memory

* [Lab Sheet](https://drive.google.com/file/d/1O57IkNHqL9VcNIGa8qtpY-aKWg3D8FWp/view?usp=sharing)
* [Source Code](https://github.com/mondus/com4521/archive/Lab05_src.zip)
* [Solution](https://github.com/mondus/com4521/archive/Lab05_sln.zip)


## Week 6

### Lecture 10 - CUDA Shared Memory

* Introduction to Shared Memory ([pdf](https://drive.google.com/file/d/1EjnE7xi5wo8HEJ3hUA74N9WMUZOudcV5/view?usp=sharing), [recording](https://digitalmedia.sheffield.ac.uk/media/Lecture+10+-+Part+01+-+Introduction+to+Shared+Memory/1_rd20qeup))
* Shared Memory Bank Conflicts ([pdf](https://drive.google.com/file/d/1-VKri93MTBbUMmlIYd-LiK6iMYphg3w9/view?usp=sharing), [recording](https://digitalmedia.sheffield.ac.uk/media/Lecture+10+-+Part+02+-+Shared+Memory+Bank+Conflicts/1_69yoldfs))
* Boundary Conditions ([pdf](https://drive.google.com/file/d/1C4h9_Y0lh2M2k09avtqtqo_1Rw677JUV/view?usp=sharing), [recording](https://digitalmedia.sheffield.ac.uk/media/Lecture+10+-+Part+03+-+Boundary+Conditions/1_5g9cwokq))
* Shared Memory Bank Conflict Calculator ([xlxs file](https://drive.google.com/file/d/1pHTvo-X02_xp8OHCobJ-zFaZ0Vq2mtKK/view?usp=sharing))

### Lecture 11 - CUDA Performance

* Memory Coalescing ([pdf](https://drive.google.com/file/d/1vDqsfjl_hRbyG1jBkllSIwNLlbycyjlz/view?usp=sharing), [recording](https://digitalmedia.sheffield.ac.uk/media/Lecture+11+-+Part+01+-+Memory+Coalescing/1_o0kfb3ux))
* The L1 Cache ([pdf](https://drive.google.com/file/d/13lSuEalXcMGrX8orbW6HUbXZFj3OqbuH/view?usp=sharing), [recording](https://digitalmedia.sheffield.ac.uk/media/Lecture+11+-+Part+02+-+The+L1+Cache/1_94wtt4kb))
* Occupancy ([pdf](https://drive.google.com/file/d/1ClFMjcO2IDjsCZ7irgSKjaUeKW4yAEev/view?usp=sharing), [recording](https://digitalmedia.sheffield.ac.uk/media/Lecture+11+-+Part+03+-+Occupancy/1_dweyffyn))

### Lab 6 - Shared Memory

* [Lab Sheet](https://drive.google.com/file/d/1_G8pSTyfSw04ELjp13Y1FB-AFKn7Sa9Q/view?usp=sharing)
* [Source Code](https://github.com/mondus/com4521/archive/Lab06_src.zip)
* [Solution](https://github.com/mondus/com4521/archive/Lab06_sln.zip)
* [Solution Further Explanation](https://drive.google.com/file/d/1RD06KqubAHJnhRVzoThf-KdTWrG9linc/view?usp=sharing)

## Week 7

### Lecture 12 - Warp Level CUDA 

* Warp Scheduling and Divergence
* Atomics
* Warp Operations
* Excel sheet for SM conflicts

### Lecture 13 - Parallel Patterns 

* Parallel Patterns Overview
* Reduction
* Scan

### Lab 07 - Atomics and Primitives

* [Lab Sheet](https://drive.google.com/file/d/1AhnQeeAn6-Fn4h1SsFiAh1OxqofUrRdA/view?usp=sharing)
* [Source Code](https://github.com/mondus/com4521/archive/Lab07_src.zip)
* [Solution](https://github.com/mondus/com4521/archive/Lab07_sln.zip)


## EASTER VACATION

## Week 8

### Lecture 14 and 15 - Performance Optimisation 

* Profiling Introduction
* The Problem
* Visual Profiler Guided Analysis

### Lab 08 - Profiling Example

* [Profile Lecture Example Code](https://github.com/mondus/com4521/archive/lab09_sln.zip)

## Week 9

### Lecture 16 - Sorting and Libraries 

* Sorting Networks
* Merge and Bitonic Sort
* Thrust Parallel Primitives Library
* Applications of Sorting (binning)

### Lecture 17 - CUDA Streams 

* Synchronous and Asynchronous execution 
* CUDA Streams
* Synchronisation
* Multi GPU Programming

### Lab 09 - Libraries and Streams

* [Lab Sheet](https://drive.google.com/file/d/1nB7uOrb-ZolV5qsuiQEasBl9CDyg2axk/view?usp=sharing)
* [Source Code](https://github.com/mondus/com4521/archive/Lab08_src.zip)
* [Solution](https://github.com/mondus/com4521/archive/Lab08_sln.zip)

## Week 10

### Lecture 18 - Guest Lecture (TBC)

Please Find below a list of previous invited lectures

* [Accelerating Road Network Simulations using GPUs](https://echo360.org.uk/media/de75ffe6-c839-49de-af50-ddb270dd529f/public)
* [Optimising Pedestrian Simulations](https://echo360.org.uk/media/6f8ed7dd-f3d8-4c25-acf2-03c36e40ea9e/public)

### Lab 

No lab due to bank holiday

## Week 11:

### No Lecture

### Assignment Help Lab

## Week 12:

No Lectures or Labs

# Calendar

You can add this calendar to your University of Sheffield Google Calendar by searching for COM4521 and COM6521

<iframe src="https://calendar.google.com/calendar/embed?src=sheffield.ac.uk_4gq0ug3uf8dlts9d21gp4l1des%40group.calendar.google.com&ctz=Europe/London" style="border: 0" width="800" height="600" frameborder="0" scrolling="no"></iframe>

# Recommended Reading

The following are useful resources but not required reading.

* Edward Kandrot, Jason Sanders, "CUDA by Example: An Introduction to General-Purpose GPU Programming", Addison Wesley 2010.
* Brian Kernighan, Dennis Ritchie, “The C Programming Language (2nd Edition)”, Prentice Hall 1988.
* NVIDIA, [CUDA C Programming Guide](http://docs.nvidia.com/cuda/cuda-c-programming-guide/)
