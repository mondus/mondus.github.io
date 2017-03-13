---
layout: page
title: Getting Started with the DGX-1 on ShARC
---

# Getting Started with the DGX-1 on ShARC #

*by Dr [Paul Richmond](http://paulrichmond.shef.ac.uk/) (University of Sheffield)*

This document describes how to use the DGX-1 GPU system on Sheffield’s new High Performance computing system (ShARC). ShARC has a number of GPU resources available including two general purpose nodes with 4x Tesla (Kepler) K80 GPUs (8 devices). This is matched by a DGX-1 system owned by computer science with 8x Tesla (Pascal) P100 GPUs. For this undergraduate module course, we will have access to the private P100 GPUs. Details of how to use these will be given in this document.

*Note: Executing code on ShARC requires that we build the code using the NVIDIA compiler `nvcc` in linux without visual studion.*

## Permission to access ShARC ##

To access ShARC you will need a HPC account. Details of gaining one of these is given on the [offical ShARC documentation page](http://docs.hpc.shef.ac.uk/en/latest/hpc/getting-started.html). When emailing the helpdesk to request an account you should copy in p.richmond@sheffield.ac.uk so that permission can be granted.

## Permission to access the DGX-1 ##

To access the DGX-1 you must have a HPC account and be a member of a special project and queue system created for computer science and the research software engineering group. You should ask Paul during a lab session for this permission to be set.

## Accessing ShARC GPUS and Initial Setup ##

The ShARC is accessed through an `ssh` terminal. To login to ShARC from a CICS managed desktop account you can use the PuTTY program (if it is unavailable then you will need to install it via the software centre). Within Putty, set the *“Host Name”* text field to `sharc.shef.ac.uk`. 

If you are connecting from a machine which is your own (i.e. not a CICS managed desktop) then connect to ShARC using the alternative instructions provided on the ShARC documentation site:

[http://docs.hpc.shef.ac.uk/en/latest/hpc/getting-started.html](http://docs.hpc.shef.ac.uk/en/latest/hpc/getting-started.html).

Once you are logged into a ShARC head node then request an interactive session by typing `qrsh`. This creates an interactive session on a CPU worker node which supports command line programs. The worker node **will not** be a GPU accelerated node and **cannot** be used to execute CUDA applications. The worker node can however be used for CUDA compilation, interactive editing of our GPU code and submission of jobs to a GPU accelerated worker. This is a much better solution than running an interactive session on a GPU node as interactive jobs will request GPU resource which will be unused if you are performing tasks like modifying or building your code.

## Configuring the CPU worker node ##

To be able to compile CUDA code within your interactive session on the CPU worker node, we will need to add a couple of modules to the environment. Load the latest version of CUDA using the following command:

	module load libs/CUDA

To compile CUDA programs, you also need a compatible version of the GCC compiler suite. This is the Linux equivalent of the MSVCC compiler within visual studio. Load version 4.9.4 using the following command:

	module load dev/gcc/4.9.4

*Note: Newer versions of GCC are supported on ShARC but may not work correctly with CUDA. Further notes on the modules are available on the ShARC software documentation site.*

Test your CUDA module is correctly loaded by calling:

	nvcc --version

You should get the version information similar to the output below.

	nvcc: NVIDIA (R) Cuda compiler driver
	Copyright (c) 2005-2015 NVIDIA Corporation
	Built on Tue_Aug_11_14:49:10_CDT_2015
	Cuda compilation tools, release 7.5, V7.5.17

## Hello World for GPUs ##

From your interactive session on the CPU worker node get the *"hello world for GPUs"* code from Github by cloning the master branch of the `CUDAHelloWorld` repository from the RSE-Sheffield github account. E.g.

	git clone https://github.com/RSE-Sheffield/CUDAHelloWorld.git

This will check out the hello world example into the folder `CUDAHelloWorld`. Take a look at the contents of this file in the console using `nano` e.g.

	nano helloworld.cu

*Note: If you wish to view/edit this file locally then you can use sftp (e.g. using Filezilla or MoboXTerm).*

Compile the code using nvcc with the following command:

	nvcc helloworld.cu –o helloworld

Assuming there are no errors, your code will be built and you will have a new executable file in the working directory.

## Running a Simple Example as a Job ##

We cannot run our compiled GPU code on the worked node as it has no GPUs or CUDA driver. Instead we must submit the execution of the GPU accelerated CUDA program via the ShARC job submission system (`qsub`). The normal command for doing this on the general GPU pool of K80s would be.

	qsub -l gpu=1 -b y ./helloworld

The `–l` command allow us to request specific resources in this case a GPU (`gpu=1`). The `–b y` command specifies that we are submitting a binary file rather than a batch script. To avoid queuing on the general ShARC GPU nodes we can use the DGX-1 GPUs by using the following call to `qsub`:

	qsub -P rse -q rse.q -l gpu=1 -b y ./helloworld

This will run the jobs on a private job queue (`-q rse.q`) for the DGX-1 which requires that your CICS HPC username is a member of the `rse` project (`-P rse`). If you asked previously for access to the DGX-1 then you will have been added to this project. Please ask on the mailing list or a lab if you have a permission error. You will be notified that your job has been submitted but you will not see the output of the executable in the terminal.

Rather than using this long `qsub` command each time you want to run this example, you can instead place the job submission options in a bash script file and submit this. Examine the file `helloworld.sh` which matches the above configurations and submit the job using the following command instead:

	qsub helloworld.sh

The labs in this training course will provide submission batch scripts for you.

## Monitoring the Progress and Output of Your Job ##

To monitor your job, you can use the `qstat` command. i.e.

	qstat –u <your_cics_username>

This will output a table with your jobs. E.g.

	job-ID  prior   name       user         state submit/start at     queue                          slots ja-task-ID
	-----------------------------------------------------------------------------------------------------------------
	205629 0.00534 bash       co1pr        r     01/18/2017 14:24:55 interactive.q@testnode01.icebe     1
	205650 0.00000 helloworld co1pr        qw    01/18/2017 14:26:45                                    1

The status of your GPU job will initially be `qw` to indicate queued and waiting. It will then change to `r` whilst running and will disappear once complete. The job submission will create an execution log file with a file name batching the binary or bash script and a  file extension of `.e<jobid>` (i.e. `helloworld.e205650`). You can view the contents of this log file using the `cat` command. E.g.

	cat helloworld.e205650

If the execution produced no errors then this file will be empty. Once the job is completed a matching output log will be created with a file extension of `*.o<jobid>` (i.e. `helloworld.sh.o205650`). The contents of which should look like the following:

	Hello World from Thread 0
	Hello World from Thread 1
	Hello World from Thread 2
	Hello World from Thread 3
	Hello World from Thread 4
	Hello World from Thread 5
	Hello World from Thread 6
	Hello World from Thread 7
	Hello World from Thread 8
	Hello World from Thread 9

## Building and Running your own code ##

To build and run your own code you will need to compile it with `nvcc` on a CPU worker node as in the above example. Note that if you rely on third party header files or libraries you will need to use the `-I` (addiitional header file include directory, `-L` (additional library include directory) and `-llibname` (link to `libname` library) options. More details on these is given in the [`nvcc` official documentation](http://docs.nvidia.com/cuda/cuda-compiler-driver-nvcc). 
