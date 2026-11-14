---
layout: archive
title: "Technical Projects"
permalink: /diyprojects/
author_profile: true
redirect_from:
  - /DIY Projects
---

My independent learning and project interests centre on **computer architecture, processor microarchitecture, RTL design, design verification, memory systems, and AI hardware**.

This page is a curated archive of project topics from my self-directed work. Project maturity varies: some are study topics or planned explorations, while others have involved implementation. I will add repository links, architecture diagrams, verification plans, and measured results as individual projects are ready to publish. A topic listed here should not be interpreted as a claim that a complete implementation or verification result is available.

## Current independent focus

### LLM inference hardware — in progress

I am building my understanding through personal projects focused on LLM inference hardware. The work is ongoing. I plan to publish the architecture, implementation choices, verification approach, and results after the projects reach a reviewable state.

## Processor architecture and microarchitecture

- 32-bit out-of-order Tomasulo execution engine.
- Y86-64 CPU design and formal verification.
- Out-of-order MIPS R10K-style processor based on RISC-V ISA.
- In-order RISC-V CPU design.
- FPGA design of a superscalar out-of-order processor.
- Superscalar pipeline simulator.
- DLX processor design.
- Simulator for the LC-3b ISA.
- Chip multiprocessor with core multithreading.
- Personal architecture research and study involving CVA6, OpenPiton, Mor1kx, and CLARVI.

## Memory systems and interconnect

- Functional verification of an MESI-protocol-based L1 cache-coherent system.
- Cache and memory hierarchy design simulator.
- CAM unit and LRU stack design using Verilog and ModelSim.
- Formal verification of cache-coherence protocols using Murphi.
- AXI interconnect network design and simulation.
- Branch-predictor studies and simulator: global 2-bit, bimodal, and correlated predictors.

## Hardware acceleration and parallel compute

- Binary artificial neural network using Verilog for ASIC/FPGA exploration.
- SMT-based GPGPU design.
- Reed–Solomon error-correction decoder hardware accelerator.
- Exploration of processor and accelerator organization for heterogeneous compute.

## Self-directed coursework

My architecture study has used publicly available course materials and resources from UC Berkeley, CMU, Stanford, Georgia Tech, UC Riverside, and other institutions. These are self-directed learning activities, not claims of enrollment in or completion of a degree programme. See [Learning & Workshops](https://priyanshumishra77.github.io/priyanshu.github.io/mooccourses/) for the course and workshop record.

## Publishing project work

For each project I publish, I aim to include:

1. Problem statement and architectural motivation.
2. Block diagram and microarchitectural decisions.
3. RTL/software implementation and build instructions.
4. Verification strategy, reference model, assertions, and coverage plan.
5. Simulation results, debug observations, limitations, and next steps.
6. Source-code repository or technical report, where publicly shareable.
