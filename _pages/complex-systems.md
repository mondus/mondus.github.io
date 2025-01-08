---
layout: archive
title: "Complex Systems"
permalink: /complex-systems/
---

Complex systems are systems in which interacting components produce emerging properties or behaviours. Examples include a system of biological cells or molecules through to population dynamics, transportation, economics and crowd behaviours. Such systems can be studied by using an approach called Agent Based Modelling (ABM). The ABM approach is a bottom-up technique where behaviours are described from an individual perspective with system level behaviours allowed to emerge as a feature of embedding individuals within a virtual simulation. Compared with more traditional “top down” modelling this approach is considerably more computationally demanding. 

I am involved in a wide range of collaborative research projects which intersect complex systems simulation with either high-performance (predominantly GPU) computing or research software engineering. For example, appling FLAME GPU to new domains to achieve higher simulation performance, often co-developing new features of the software to extend its applicability. Additionally, developing new software tools or methods around large scale complex systems simulations.

# FLAME GPU and Agent Based Modelling and Simulation

<div style="float:right;padding:20px;" markdown="1">
![FLAME GPU Logo](..\images\fgpu2_icon_256.png)
</div>

I have pioneered the use of inexpensive Graphics Processing Units (GPUs) to vastly accelerate the computational performance and hence scale of such simulations. GPUs are increasingly suited to general purpose computing however the design of appropriate algorithms and software approaches is an active area of my research interests, required to exploit the GPUs massive levels of parallelism. Most notably I am the author of the FLAME GPU software. The FLAME GPU Software originated from my PhD research but has been extended through a number of research projects and individual fellowships. It is also being developed by various RSEs at Sheffield who are looking to improve various aspects of performance or functionality. The primary aim of FLAME GPU is to provide a high level abstraction for complex system simulation through agent based modelling. The details of the GPU architecture are hidden from an user and code is automatically generated. Performance levels of multi agent simulation in FLAME GPU can far exceed those of traditional multi agent simulators. FLAME GPU has attracted a wide range of commercial collaborations from the Department for Transport, SIEMENS and the Rail Standards safety Board (RSSB) and Fujitsu. FLAME GPU also underpins (as the primary experimentation tool) research into; clinical management of Neuroblastoma – PRIMAGE, developing in silico trials to fight tuberculosis – Strituvad and predicting crowd behaviour with respect to social distancing within transportation infrastructure. Over the last 4-5 years the FLAME GPU software has undergone major redevelopment and is now within Beta release stage. The changes to this software make it increasingly accessible, flexible and performant opening up a wider range of potential collaborations.

Links:

 - [NVIDIA Dev Blog Tutorial and Overview for FLAME GPU (a nice approachable introduction)](https://developer.nvidia.com/blog/fast-large-scale-agent-based-simulations-on-nvidia-gpus-with-flame-gpu/)
 - FLAME GPU 2 [Paper](https://onlinelibrary.wiley.com/doi/10.1002/spe.3207), [GitHub](https://github.com/FLAMEGPU/FLAMEGPU2), [Website](https://flamegpu.com/)
 - [FLAME GPU tutorial on Colab](https://colab.research.google.com/github/FLAMEGPU/FLAMEGPU2-tutorial-python/blob/google-colab/FLAME_GPU_2_python_tutorial.ipynb)
 - [My RSE Con 23 talk on FLAME GPU](https://www.youtube.com/watch?v=ZYE0uU264mM) (describing some of the algorithmic and software engineering details)

# Broader Complex Systems Simulation (and Neuroscience)

Beyond FLAME GPU, I have a more general interest in the simulation of complex systems. Neural simulation (computational neuroscience) and neural language design (neuro-informatics) share many of the same problems as agent based simulation (with the advantage that neurons tend not to migrate). First of all large scale simulation requires novelty in the application of parallel hardware architectures, secondly appropriate software tools and languages are required for describing models using high level abstractions which promote automatic parallelisation.

With respect to neural simulation I worked as part of the BIMPA team in developing software for simulation using the SpiNNaker architecture as well as part of the Digital Fruit Fly Brain project to develop a simulator called Neurokernel. The SpiNNaker architecture is inspired by neural biology to be highly scalable and low power. With this comes a number of challenges for mapping models and designing software to facilitate the use of this esoteric infrastructure. With respect to neural language design, the SpineML language was proposed by myself and Alex Cope as part of the BIMPA project but has grown beyond this to become a simulator independent neural language for spiking point neuron models. SpineML has an advanced user interface called Spine Creator which makes it ideal for modellers to engage with, it also has support for a number of parallel simulators including DAMSON, BRAHMS and GeNN. SpineML is inspired by languages such as NeuroML (for compartmental modelling of neurons) and NineML. It is used as the modelling tool within [Opteran](https://opteran.com/) (a University of Sheffield Spin-out).


<div style="float:right;width:300px;padding:20px;" markdown="1">
![FLAME GPU Logo](..\images\spineml.png)
</div>

Links: 

 - SpineML [Paper](https://pubmed.ncbi.nlm.nih.gov/24253973/), [GitHub](https://github.com/SpineML/spineml), [Website](https://spineml.github.io/)
 - [Opteran Technologies Limited](https://opteran.com/)
 - [SpiNNaker Architecture](https://spinnaker.io/docs/reference/architecture/)
