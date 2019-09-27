# Notes about papers in this folder

## 2019-DAFX: An FPGA-Based Accelerator for Sound Field Rendering

**Important**

Use FPGA to implement FDTD  for sound field rendering. Programmed with high level synthesis in C++ on Intel FPGAs. Significant gain in performance compared to a CPU. Still troubles to run the model in real time.

## 2015-DAFX: Feasability Analysis of Real-Time Physical Modeling Using Wavecore Processor Technology on FPGA

**Important**

Use Wavecore (proprietary) as an intermediate high level language to program FPGAs to implement real-time audio DSP applications. In a way, quite similar to what we're trying to achieve with SyFaLa but since the technology is proprietary, the whole thing is pretty opaque.

## 2015-IEEE: FPGA-Based Sound Synthesis by Digital Waveguide

Title is petty self describing... 

## 2014-DAFX: Declaratively Programmable Ultra Low-Latency Audio Effects Processing on FPGA

Another less recent paper by Math Verstraelen on using WaveCore to program FPGAs at a high level for audio DSP.

## 2014-IEEE: A FPGA Implementation of the Two-Dimensional Digital Huygens’ Model

Basically preliminary version of 2019-DAFX.

## 2012-PARALLEL: Design Space Exploration in Many-Core Processors for Sound Synthesis of Plucked String Instruments

Very interesting paper considering all sorts of multiprocessor hardware for plucked string instruments including FPGAs.

## 2012-DAFX: Real-Time Difference Physical Models of Musical Instruments on a Field Programmable Gate Array (FPGA)

**Important**

Kind of a reference paper. Pure implementation, nothing particular though. Idea here is really to take advantage of the computational power of the FPGA.

## 2011-DAFX: DHM and FDTD Based Hardware Sound Field Simulation Acceleration

Basically, previous version of DAFX-19.

## 2011-IEEE: Multi-Core Platforms for Beamforming and Wave Field Synthesis

**Important** 

Beamforming and WFS on FPGAs and GPUs. Mostly for computational reasons, not for audio latency.

## 2010-ACTA: Labview FPGA Implementation of Digital Reverberators

Title is self describing. 

## 2009-CHAP: Real-Time Physical Modelling of a complete Banjo geometry using FPGA hardware technology

Physical modeling on FPGA, again... Linked to 2012-DAFX.

## 2009-DAFX: A FPGA-Based Adaptive Noise Canceling System

In the context of VR and for headphones.

## 2009-CF: Wave Field Synthesis for 3D Audio: Architectural Prospectives

**Important**

Preliminary version of 2011-IEEE.

Take advantage of FPGA in that context but only for its processing capabilities not for latency, which doesn't really matter in the context of WFS.

## 2008-IEEE: Design Methodology for Real-Time FPGA-Based Sound Synthesis

**Important**

THE reference for finite difference scheme models running on FPGAs. The main advantage here is computational.

## 2007-NIME: Physical models and musical controllers – designing a novel electronic percussion instrument

FPGA used to implement a large physical model using FDTD method. Only possible on FPGA cause very computationally expensive. Highly concurrent algorithm suitable for FPGAs.

## 2006-DAFX: Using Faust for FPGA Programming

Preliminary work on our topic.

## 2005-IEEE: FPGA Implementation of 1D Wave Equation for Real-Time Audio Synthesis

**Important**

One of the earliest paper on the topic. Doing pretty straight forward stuff. 

## 2004-IEEE: An FPGA-based Re-configurable 24-bit 96kHz Sigma-Delta Audio DAC

Implementing a sigma-delta audio dac with an FPGA. Very interesting reference.

## Other Reference

* Dada machine should be mentioned in the proposal
* Guitar pedal based on an FPGA: <https://medium.com/@korora_audio/a-case-study-using-fpga-for-audio-dsp-eab4859bdde2>
* Article on using FPGAs for audio: <https://scialert.net/fulltextmobile/?doi=jas.2014.1972.1977>
* <https://en.antelopeaudio.com/hardware-based-fpga-effects/>

## Thoughts

* Labview/matlab seems to be a common way to program FPGAs at a high level.
* Basically, a large portion of the papers on the topic are related to FDTD acceleration.
