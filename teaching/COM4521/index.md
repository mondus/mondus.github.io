---
title: Dr Paul Richmond - COM4521 & COM 6521 Introduction to Parallel Computing with GPUs
layout: homepage
---


# Course Information

Welcome to the 2021/2022 module page for COM4521/COM6521 Parallel Computing with GPUs.

Accelerator architectures are discrete processing units which supplement a base processor with the objective of providing advanced performance at lower energy cost. Performance is gained by a design which favours a high number of parallel compute cores at the expense of imposing significant software challenges. This module looks at accelerated computing from multi-core CPUs to GPU accelerators with many TFlops of theoretical performance. The module will give insight into how to write high performance code with specific emphasis on GPU programming with NVIDIA CUDA GPUs. A key aspect of the module will be understanding what the implications of program code are on the underlying hardware so that it can be optimised.
 
The modules aims, objectives and assessment details are available on the [modules public teaching page](http://www.dcs.shef.ac.uk/intranet/teaching/public/modules/level4/com4521.html).

## Software for the Module

The module programming exercises are designed to be completed on PCs in the Diamond compute labs. As the modules teaching is online these machines are available via virtual desktop. All Diamond compute lab machines have Visual Studio 2019 and CUDA 11.1 If you intend to use your own machine for programming exercises (on the CUDA part of the module) then you **must** install the latest Community version of Visual Studio 2019 **before** you install the CUDA 11.1 toolkit.

If you want to complete the exercises in Linux then example Makefiles will be provided with the lab starting code and solutions. It is not possible to build Linux CUDA programs on PCs in the Diamond compute labs.

## Computers and Labs Available

As the module requires access to a machine with a GPU the following have been made available to you.

* All diamond Compute Labs (other than High spec lab) - All diamond all in one machines have an NVIDIA GTX1050 (Pascal generation) GPUs. Dedicated labs have been reserved each week to use these. You can find machine availability outside of lab times by using [Find a PC](https://www.sheffield.ac.uk/findapc)
* Diamond High Spec Lab Reservation - These are higher spec machines with NVIDIA Quadro 5200 (Pascal generation) GPUs.
* Your own Windows/Linux machine - Follow the instructions under "software for this module".
* A GPU backed cloud instance (at your own risk and cost)

## Course Attendance Monitoring

Lab attendance is recorded through the use of the [Lab Feedback Form](https://bit.ly/COM4521Form). All attendees on the course are expected to complete this each week. The purpose of the lab feedback from to monitor engagement with the course content and to allow the course instructors to identify areas for group discussion. 

Important Note: **It is not possible to properly understand the course material without completing the labs and reviewing the solutions.** If you do not complete the labs then you will find the assignment difficult. The first lecture will provide some insight into how course engagement affects assessment performance.

## Lectures

With the exception of the first lecture, which will be delivered in person, the course will be run using a flip classroom approach. Lecture content has been pre-recorded into bite sized chunks of ~10-15m each. There is a lecture list for each week which you are expected to listen to **in advance** of the next weeks lab. 

## In Person Lab Classes

The lab classes have been designed to re-enforce the material which you will observe in the on-line lectures by applying the techniques and approaches to specific problems. You should aim to attempt the lab classes exercises **prior** to attending the lab class (i.e. the week before) and use the labs to obtain help in understand and applying the taught content. The lab class solutions are commented to provide insight. The solutions are available in advance of the lab so if you are stuck on a particular exercise then review these to move on and seek help in understanding the problem and solution in the lab class. Within the labs, pair programming or work within small groups is encouraged but left to personal preference. Discussion is encouraged. 

During the lab class there will be an opportunity to discuss and review lecture content, lecture examples and lab solutions. Guided walkthroughs of certain parts of the lab solutions will be provided.

Although the labs are structured around the online lecture material each week you can (and should) ask for help regarding any of the labs during the scheduled lab time. The labs are also used for assignment help. You should start this early.

You should complete the [Lab Feedback Form](https://bit.ly/COM4521Form) each week by editing your response. Please update your responses at the start of each lab.

## Course Assessment

In response to student feedback the number of assignments has been reduced to a single assignment which reflects the reduced number of learning objectives for the module. The assignment will be released Monday the 28th February 2022 (week 4) and is due 17:00 on Wednesday 25th May (week 13). The assignment forms 80% of your mark. You are expected to ask for feedback on your assignment work during the scheduled lab classes.

The remaining 20% of the module mark is from two mole quizes which must be completed under exam conditions. I.e. Within the specified locations with the lock down browser under invigilation from demonstrators.  

* Week 5 - 08/03/2022 13:00 in Diamond Computer Room 3
* Week 10 - 03/05/2022 13:00 in Computer room A04, Alfred Denny Building

Quizes will take 40m (must be completed within the hour) and be multiple choice in a simmilar format to the weekly lab question.

## DDP students and Staff Candidates

PhD students and research/academic staff are not required to undertake assessment but DDP students are expected to attend labs as evidence of participation in the module. You should ensure that you enroll for the course via DDP to ensure that you have access to the Blackboard. If you are a staff member attendee and require access to Blackboard then please contact me.

## Discussion, Announcements and Requests for Help

A [Google group](https://groups.google.com/a/sheffield.ac.uk/d/forum/com4521-group) has been created for announcements, help and discussion. Any important announcements relating to the module will be made via this group. All students enrolled on the module on the 3rd February 2021 have been added to this group already. Likewise and staff or Phd students who expressed an interest in the course via the google form have been added. If you have transferred via Add/Drop then you will need to manually join the group yourself. The group is monitored by the teaching staff (including lab assistants) as well as additional PhD students who can provide help. The purpose of the mailing list is to ask for general support and guidance with the course material (e.g. with concepts and ideas) rather than posting your own code. **You should not post your assignment code on this forum**. If you require personal assistance with your assignment code then you should request this during the lab hours. Any lab class can be used for assignment help in addition to the lab exercises which are set each week.

[https://groups.google.com/a/sheffield.ac.uk/d/forum/com4521-group](https://groups.google.com/a/sheffield.ac.uk/d/forum/com4521-group)


# Course Material Material

Lectures are pre-recorded and are availble on the [COM4521  Parallel Computing with Graphical Processing Units Kaltura Channel](https://digitalmedia.sheffield.ac.uk/channel/COM4521+Parallel+Computing+with+Graphical+Processing+Units/201133333) or as downloadable pdfs on [Google Drive](https://drive.google.com/drive/folders/1XxXJdrzSP6XFwrzzEnNv1BLptfsgZOXu?usp=sharing). Each weeks practical activities (the labs) follow the ideas presented in the lectures so it is important that you follow the lecture and lab timetable below.

## Week 01

### Lecture 01 (In Person) - Course Introduction and Overview

* Course Context ([pdf](https://drive.google.com/open?id=1E0291GtCX_s_5QVHZllq1e6FJaHPorv8), [recording](https://digitalmedia.sheffield.ac.uk/media/Lecture+01+-+Part+01+-+Course+Context/1_4ozidnx3))
* Supercomputing and Software ([pdf](https://drive.google.com/open?id=1E87UUwB1eZAsoCvBfTN00BEcTj9Grq0E), [recording](https://digitalmedia.sheffield.ac.uk/media/Lecture+01+-+Part+02+-+Super+Computing+and+Software/1_3cae6aog))
* Module Details ([pdf](https://drive.google.com/open?id=1E9RccFaT8gKJNMkOOUObDBI8s6VwmDR3), no recording)

### On-line On Demand Lectures - Introduction to C

* Introducing C ([pdf](https://drive.google.com/file/d/1_mL4lhg2sb7Ez4-BzFEele6MXggXBiUK/view?usp=sharing), [recording](https://digitalmedia.sheffield.ac.uk/media/Lecture+02+-+Part+01+-+Introducing+C/1_eakd0424))
* Functions and Scoping ([pdf](https://drive.google.com/file/d/1tM_1D7w0WuVcvzU8QrdaEaZIf7-cgs6R/view?usp=sharing), [recording](https://digitalmedia.sheffield.ac.uk/media/Lecture+02+-+Part+02+-+Functions+and+Scoping/1_cf4tnuln))
* Arrays, Strings and IO ([pdf](https://drive.google.com/file/d/1KqpjzKsc5QjPq-qDKueT1EQBaP8ZCZeJ/view?usp=sharing), [recording](https://digitalmedia.sheffield.ac.uk/media/Lecture+02+-+Part+03+-+Arrays+Strings+and+IO/1_60zchnsf))

## Week 02

### Introduction to Visual Studio and C Programming Lab

* [Getting Started with Visual Studio 2019 Overview](https://drive.google.com/file/d/1BCpXw9Mr04DSkal7P_ARzMis78t3Pveu/view?usp=sharing)
* [Lab Sheet](https://drive.google.com/open?id=1A6efezFVDsIThkoNCfLwXSJvg9sM9Kz6)
* [Source Code](https://github.com/mondus/com4521/archive/Lab01_src.zip)
* [Solution](https://github.com/mondus/com4521/archive/Lab01_sln.zip)

### On-line On Demand Lectures - Memory 

* Pointers ([pdf](https://drive.google.com/file/d/1ek2YjPLMDwdtRJVlUrmPZ31SV6E7UWbV/view?usp=sharing), [recording](https://digitalmedia.sheffield.ac.uk/media/Lecture+03+-+Part+01+-+Pointers/1_2lxp7wyb))
* Advanced use of Pointers ([pdf](https://drive.google.com/file/d/1TuHaiow_oGjXOWvTy05CFY3lw0bwKh2Y/view?usp=sharing), [recording](https://digitalmedia.sheffield.ac.uk/media/Lecture+03+-+Part+02+-+Advanced+Pointers/1_v4x7d5sr))
* Dynamically Managed Memory ([pdf](https://drive.google.com/file/d/1tnGYCG48XOYMhUf78dJT-VT1kT4d6lFp/view?usp=sharing), [recording](https://digitalmedia.sheffield.ac.uk/media/Lecture+03+-+Part+03+-+Manual+Memory+Management/1_4j49qhoj))
* Structures and Binary Files ([pdf](https://drive.google.com/file/d/1Pl_wx-H9dDXfGfKEprxs6jg3RzrTSnVq/view?usp=sharing), [recording](https://digitalmedia.sheffield.ac.uk/media/Lecture+03+-+Part+04+-+Structures+and+Binary+Files/1_38omyxrt))

### On-line On Demand Lectures - Optimisation 

* Optimisation Overview ([pdf](https://drive.google.com/file/d/1wVdzbq9DL0S-qK0K1np084Mc8mF7CWNb/view?usp=sharing), [recording](https://digitalmedia.sheffield.ac.uk/media/Lecture+04+-+Part+01+-+Optmisation+Overview/1_z09qnv7q))
* Compute Bound Code ([pdf](https://drive.google.com/file/d/17xQZlwihTvo2vEEWPpb5k8EWOqXezz3U/view?usp=sharing), [recording](https://digitalmedia.sheffield.ac.uk/media/Lecture+04+-+Part+02+-+Compute+Bound+Code/1_t74gjrqg))
* Memory Bound Code ([pdf](https://drive.google.com/file/d/1pi7FnfWd_0YcMouXTnktV7Pu4BDXoEOh/view?usp=sharing), [recording](https://digitalmedia.sheffield.ac.uk/media/Lecture+04+-+Part+03+-+Memory+Bound+Code/1_eaa6z5dh))

## Week 03

### Memory and Performance Lab

* [Lab Sheet](https://drive.google.com/open?id=1AGK3j4UNxcIhZkZpbXfl7xrGwENcKYvV)
* [Source Code](https://github.com/mondus/com4521/archive/Lab02_src.zip)
* [Solution](https://github.com/mondus/com4521/archive/Lab02_sln.zip)

### On-line On Demand Lectures - OpenMP 

* OpenMP Overview ([pdf](https://drive.google.com/file/d/1Y9EUh835wkh8bwMHyNhu0fzFQGlygGl1/view?usp=sharing), [recording](https://digitalmedia.sheffield.ac.uk/media/Lecture+05+-+Part+01+-+OpenMP+Overview/1_tr35veym))
* Loops and Critical Sections ([pdf](https://drive.google.com/file/d/1adfofgTWGOGqUwOuDgTS9OW_nVDeBS3n/view?usp=sharing), [recording](https://digitalmedia.sheffield.ac.uk/media/Lecture+05+-+Part+02+-+Loops+and+Critical+Sections/1_j4mfsl94))
* Scoping and Tasks ([pdf](https://drive.google.com/file/d/14RxdZl6x2GYiCjbbi_1g1j5B5GhlXfzA/view?usp=sharing), [recording](https://digitalmedia.sheffield.ac.uk/media/Lecture+05+-+Part+03+-+Scoping+and+Tasks/1_tfgpqt3a))

### On-line On Demand Lectures - OpenMP Part II 

* Parallel Reduction ([pdf](https://drive.google.com/file/d/1DhPA-mFid4mFkUkFsRacIjzrPPvqpQs2/view?usp=sharing), [recording](https://digitalmedia.sheffield.ac.uk/media/Lecture+06+-+Part+01+-+Parallel+Reductions/1_0wfcdxdy))
* Scheduling ([pdf](https://drive.google.com/file/d/1n86lfK9u96e6VaqxONkqFg0yTqbIqET-/view?usp=sharing), [recording](https://digitalmedia.sheffield.ac.uk/media/Lecture+06+-+Part+02+-+Scheduling/1_jbiq6pkl))
* Nesting and Summary ([pdf](https://drive.google.com/file/d/1V-ufrzqwAZPvIs6bXl0zt9wE6uJ9KUeT/view?usp=sharing), [recording](https://digitalmedia.sheffield.ac.uk/media/Lecture+06+-+Part+03+-+Nesting+and+Summary/1_m9hddu82))

## Week 04

### OpenMP Lab

* [Lab Sheet](https://drive.google.com/open?id=1ANdghDhzs7ez09sU-Ma4cDFV-TmFR5HL)
* [Source Code](https://github.com/mondus/com4521/archive/Lab03_src.zip)
* [Solution](https://github.com/mondus/com4521/archive/Lab03_sln.zip)

### On-line On Demand Lectures - GPU Architectures 

* Introduction to GPUs ([pdf](https://drive.google.com/file/d/1cGZgGCB27m6zBkqR7-P1Lo0Ce8z7LzYx/view?usp=sharing), [recording](https://digitalmedia.sheffield.ac.uk/media/Lecture+07+-+Part+01+-+Introduction+to+GPUs/1_p7q41uvc))
* Programming GPUs ([pdf](https://drive.google.com/file/d/13G5k7JxXWYkmKdf_f3m34173Z4QQZNNb/view?usp=sharing), [recording](https://digitalmedia.sheffield.ac.uk/media/Lecture+07+-+Part+02+-+Programming+GPUs/1_76m5dhjm))
* GPU Hardware ([pdf](https://drive.google.com/file/d/1Q5YBM8GZqXp4P3FR1yDSPKSN9LP3yFTk/view?usp=sharing), [recording](https://digitalmedia.sheffield.ac.uk/media/Lecture+07+-+Part+03+-+GPU+Hardware/1_t7dweiyp))


### On-line On Demand Lectures - Introduction to CUDA 

* The CUDA Programming Model ([pdf](https://drive.google.com/file/d/1p50MnSqyC-U1lls08GhVX-mW8TEuXqLb/view?usp=sharing), [recording](https://digitalmedia.sheffield.ac.uk/media/Lecture+08+-+Part+01+-+CUDA+Programming+Model/1_kbdt8jns))
* CUDA Device Code ([pdf](https://drive.google.com/file/d/1he_iuEuyo5nONhM9DtkMmVdQ1Zat1s86/view?usp=sharing), [recording](https://digitalmedia.sheffield.ac.uk/media/Lecture+08+-+Part+02+-+CUDA+Device+Code/1_q8zijjv4))
* CUDA Host Code and Memory Management ([pdf](https://drive.google.com/file/d/1-PPKh4g2-Pe8jITUsLbUO0A0SxwIGXtU/view?usp=sharing), [recording](https://digitalmedia.sheffield.ac.uk/media/Lecture+08+-+Part+03+-+CUDA+Host+Code+and+Memory+Management/1_g4zl8te4))

### Assignment Handout 

The assignment will be handed out on the 28th February via Blackboard.

## Week 05

### Introduction to CUDA Lab

* [Lab Sheet](https://drive.google.com/open?id=1AWj5R_4StScIoTFynDreVR61tR_Ry4x5)
* [Source Code](https://github.com/mondus/com4521/archive/Lab04_src.zip)
* [Solution](https://github.com/mondus/com4521/archive/Lab04_sln.zip)
* [CUDA Compilation with Visual Studio 2019 Guide](https://drive.google.com/file/d/1p1WLCG_KfmB54pNxOwAl2fsoh3tFxLy7/view?usp=sharing)


### On-line On Demand Lectures - CUDA Memory

* Memory Overview ([pdf](https://drive.google.com/file/d/1BxiovKdODm1OsRTsLzW0LyOj1CfBYVQX/view?usp=sharing), [recording](https://digitalmedia.sheffield.ac.uk/media/Lecture+09+-+Part+01+-+Memory+Overview/1_0pa748z1))
* Global and Constant Memory ([pdf](https://drive.google.com/file/d/1ZvdLGJJ3D_-DrEFsR6Sai-sA5WN-uuWT/view?usp=sharing), [recording](https://digitalmedia.sheffield.ac.uk/media/Lecture+09+-+Part+02+-+Global+and+Constant+Memory/1_fl15aonq))
* Read Only and Texture Memory ([pdf](https://drive.google.com/file/d/1bSk8km76Y0CXAcBhBypwknl8OGoXb0VT/view?usp=sharing), [recording](https://digitalmedia.sheffield.ac.uk/media/Lecture+09+-+Part+03+-+Read-Only+and+Texture+Memory/1_kiodtb5l))


### On-Demand Lectures - Using GPU Backed Cloud Instances (Optional Content)

*Note/Disclaimer: Any use of cloud is entirely at your own risk and cost. The videos provide a short overview of the use of cloud instances but you are responsible for your own accounts and any cost associated with it. You are encouraged to read up on aspects such as billing notifications and the specific charges for on demand pricing and storage.*

* Creating an EC2 instance using the template AMI ([recording](https://digitalmedia.sheffield.ac.uk/media/CloudComputing-Part1/1_dzaso44d))
* Connecting to your cloud instance ([recording](https://digitalmedia.sheffield.ac.uk/media/CloudComputing-Part2/1_buquvcon))
* Setting restriction on inbound traffic to your instance ([recording](https://digitalmedia.sheffield.ac.uk/media/CloudComputing-Part3.mkv/1_7lf1y6v9))


### Blackboard Quiz

There is an assessed blackboard quiz this week. Date, time and location are in the course google calendar.

## Week 6

### CUDA Memory Lab

* [Lab Sheet](https://drive.google.com/open?id=1AjIdrVgZujFheJ0fkqUcYOWfAaPbNLPb)
* [Source Code](https://github.com/mondus/com4521/archive/Lab05_src.zip)
* [Solution](https://github.com/mondus/com4521/archive/Lab05_sln.zip)


### On-line On Demand Lectures - CUDA Shared Memory

* Introduction to Shared Memory ([pdf](https://drive.google.com/file/d/1EjnE7xi5wo8HEJ3hUA74N9WMUZOudcV5/view?usp=sharing), [recording](https://digitalmedia.sheffield.ac.uk/media/Lecture+10+-+Part+01+-+Introduction+to+Shared+Memory/1_rd20qeup))
* Shared Memory Bank Conflicts ([pdf](https://drive.google.com/file/d/1-VKri93MTBbUMmlIYd-LiK6iMYphg3w9/view?usp=sharing), [recording](https://digitalmedia.sheffield.ac.uk/media/Lecture+10+-+Part+02+-+Shared+Memory+Bank+Conflicts/1_69yoldfs))
* Boundary Conditions ([pdf](https://drive.google.com/file/d/1C4h9_Y0lh2M2k09avtqtqo_1Rw677JUV/view?usp=sharing), [recording](https://digitalmedia.sheffield.ac.uk/media/Lecture+10+-+Part+03+-+Boundary+Conditions/1_5g9cwokq))
* Shared Memory Bank Conflict Calculator ([xlxs file](https://drive.google.com/file/d/1pHTvo-X02_xp8OHCobJ-zFaZ0Vq2mtKK/view?usp=sharing))

### On-line On Demand Lectures - CUDA Performance

* Memory Coalescing ([pdf](https://drive.google.com/file/d/1vDqsfjl_hRbyG1jBkllSIwNLlbycyjlz/view?usp=sharing), [recording](https://digitalmedia.sheffield.ac.uk/media/Lecture+11+-+Part+01+-+Memory+Coalescing/1_o0kfb3ux))
* The L1 Cache ([pdf](https://drive.google.com/file/d/13lSuEalXcMGrX8orbW6HUbXZFj3OqbuH/view?usp=sharing), [recording](https://digitalmedia.sheffield.ac.uk/media/Lecture+11+-+Part+02+-+The+L1+Cache/1_94wtt4kb))
* Occupancy ([pdf](https://drive.google.com/file/d/1ClFMjcO2IDjsCZ7irgSKjaUeKW4yAEev/view?usp=sharing), [recording](https://digitalmedia.sheffield.ac.uk/media/Lecture+11+-+Part+03+-+Occupancy/1_dweyffyn))

## Week 7

### Shared Memory Lab

* [Lab Sheet](https://drive.google.com/open?id=1AqpAd8eseYmlDQo4iTX34HUSrbxw-IIO)
* [Source Code](https://github.com/mondus/com4521/archive/Lab06_src.zip)
* [Solution](https://github.com/mondus/com4521/archive/Lab06_sln.zip)
* [Solution Further Explanation](https://drive.google.com/file/d/1RD06KqubAHJnhRVzoThf-KdTWrG9linc/view?usp=sharing)


### On-line On Demand Lectures - Warp Level CUDA 

* Scheduling and Divergence ([pdf](https://drive.google.com/file/d/1QeI551TNSpKVRZN7tq6N6-VjTp4ch0Wp/view?usp=sharing), [recording](https://digitalmedia.sheffield.ac.uk/media/Lecture+12+-+Part+01+-+Scheduling+and+Divergence/1_z4pi18mz))
* Advanced Divergence ([pdf](https://drive.google.com/file/d/1LAUmDC1WkaauNJahWbdAkVi37xo7sVzd/view?usp=sharing), [recording](https://digitalmedia.sheffield.ac.uk/media/Lecture+12+-+Part+02+-+Advanced+Divergence/1_ddlggmc7))
* Atomic and Warp Operations ([pdf](https://drive.google.com/file/d/17goRBO5osS5mbZHRd48A6TU8BZyT-wse/view?usp=sharing), [recording](https://digitalmedia.sheffield.ac.uk/media/Lecture+12+-+Part+03+-+Atomics+and+Warp+Operations/1_ais622f9))

### On-line On Demand Lectures - Parallel Patterns 

* Parallel Patterns Overview ([pdf](https://drive.google.com/file/d/1gJfnZjQzlB1GzV4BgnaQNXU4aAWyfFIX/view?usp=sharing), [recording](https://digitalmedia.sheffield.ac.uk/media/Lecture+13+-+Part+01+-+Parallel+Patterns+Overview/1_a0nt7yyq))
* Reduction ([pdf](https://drive.google.com/file/d/1mbFSXVTUKmvNZTPmBlLMRIfNjQbpuFDr/view?usp=sharing), [recording](https://digitalmedia.sheffield.ac.uk/media/Lecture+13+-+Part+02+-+Reduction/1_c12ixy0e))
* Scan ([pdf](https://drive.google.com/file/d/1IUDNWjkWDOHtIgg5emo-UgnbyU1xboED/view?usp=sharing), [recording](https://digitalmedia.sheffield.ac.uk/media/Lecture+13+-+Part+03+-+Scan/1_pfrawiuc))

## Week 8

### Atomics and Primitives Lab

* [Lab Sheet](https://drive.google.com/open?id=1B8tAAQsfVbWVaQtKB_GOyQtDkeBJKVJN)
* [Source Code](https://github.com/mondus/com4521/archive/Lab07_src.zip)
* [Solution](https://github.com/mondus/com4521/archive/Lab07_sln.zip)

### On-line On Demand Lectures - Performance Optimisation 

* Performance Profiling - Guest Lecture by Dr Robert Chisholm ([pdf](https://drive.google.com/file/d/1fwo_kuB2hVBPTcJg7FViPt67MrKHS6H0/view?usp=sharing), [recording](https://digitalmedia.sheffield.ac.uk/media/Lecture+14+%26+15+Profiling/1_dn7xvs3k))

## EASTER VACATION

## Week 9

### Profiling Lab

* [Profile Lecture Example Code](https://github.com/mondus/com4521/archive/lab09_sln.zip)
There is no lab sheet for this lab. Examine the source code and try changing the `STEP` macro to compile different iterations of the code to run through the profiler.

### On-line On Demand Lectures - Sorting and Libraries 

* Sorting (Networks) ([pdf](https://drive.google.com/file/d/1P-ove2cxmDTb4J6eqCNE6T5zSKnEwpaG/view?usp=sharing), [recording](https://digitalmedia.sheffield.ac.uk/media/Lecture+16+-+Part+01+-+Sorting/1_xre37phi))
* Libraries and Thrust ([pdf](https://drive.google.com/file/d/1HI19ikicGWw3_2zNlK-pZixWcH6qNryM/view?usp=sharing), [recording](https://digitalmedia.sheffield.ac.uk/media/Lecture+16+-+Part+02+-+Libraries/1_twyysk9a))
* Applications of GPU Sort ([pdf](https://drive.google.com/file/d/1xkv4Zw6g86W6lzF3bs2ZEQLGci7FvLKd/view?usp=sharing), [recording](https://digitalmedia.sheffield.ac.uk/media/Lecture+16+-+Part+03+-+Applications+of+Sort/1_ur7qxhff))


### On-line On Demand Lectures - CUDA Streams 

* Synchronous and Asynchronous Execution ([pdf](https://drive.google.com/file/d/1grdnZs88EvybgW1vydR7FaVgpglbZiCO/view?usp=sharing), [recording](https://digitalmedia.sheffield.ac.uk/media/Lecture+17+-+Part+01+-+Synchronous+and+Asynchronous+Execution/1_d6b13ebk))
* CUDA Streams ([pdf](https://drive.google.com/file/d/113W7x70o-KcuRZ2gK6drp7QM2XvUWff8/view?usp=sharing), [recording](https://digitalmedia.sheffield.ac.uk/media/Lecture+17+-+Part+02+-+CUDA+Streams/1_4jsxnwiz))
* Synchronisation ([pdf](https://drive.google.com/file/d/1Ejnt2KKrydP8AJRy36ZSwIKauruKiLkj/view?usp=sharing), [recording](https://digitalmedia.sheffield.ac.uk/media/Lecture+17+-+Part+03+-+Synchronisation/1_zftp0xht))
* Multi GPU Programming ([pdf](https://drive.google.com/file/d/1Ejnt2KKrydP8AJRy36ZSwIKauruKiLkj/view?usp=sharing), [recording](https://digitalmedia.sheffield.ac.uk/media/Lecture+17+-+Part+04+-+Multi+GPU+Programming/1_k75fi901))


## Week 10

### Blackboard Quiz

There is an assessed blackboard quiz this week. Date, time and location are in the course google calendar.


### Libraries and Streams Lab (Note: This is on Friday due to bank holiday)

* [Lab Sheet](https://drive.google.com/open?id=1BIZ6pfUXtNHxLrP9iitY4ncAtAJUt5l5)
* [Source Code](https://github.com/mondus/com4521/archive/Lab08_src.zip)
* [Solution](https://github.com/mondus/com4521/archive/Lab08_sln.zip)

### In Person Invited Lecture - TBC

### Previous On Demand Invited Lectures (Optional)

Please Find below a list of previous invited lectures which may be of interest.

* [Accelerating Road Network Simulations using GPUs](https://echo360.org.uk/media/de75ffe6-c839-49de-af50-ddb270dd529f/public)
* [Optimising Pedestrian Simulations](https://echo360.org.uk/media/6f8ed7dd-f3d8-4c25-acf2-03c36e40ea9e/public)

## Week 11:

### Assignment Help Lab

### No Lectures

## Week 12:

### Assignment Help Lab

### No Lectures

# Calendar

You can add this calendar to your University of Sheffield Google Calendar by searching for COM4521 and COM6521

<iframe src="https://calendar.google.com/calendar/embed?src=sheffield.ac.uk_4gq0ug3uf8dlts9d21gp4l1des%40group.calendar.google.com&ctz=Europe/London" style="border: 0" width="800" height="600" frameborder="0" scrolling="no"></iframe>

# Recommended Reading

The following are useful resources but not required reading.

* Edward Kandrot, Jason Sanders, "CUDA by Example: An Introduction to General-Purpose GPU Programming", Addison Wesley 2010.
* Brian Kernighan, Dennis Ritchie, “The C Programming Language (2nd Edition)”, Prentice Hall 1988.
* NVIDIA, [CUDA C Programming Guide](http://docs.nvidia.com/cuda/cuda-c-programming-guide/)
