---
layout: archive
title: "Curriculum Vitae"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
  - /resume/
---

# Priyanshu Mishra

**CPU / SoC Design Verification Engineer | RISC-V | DSP/ASIP | Processor HW/SW Co-Verification**

Bengaluru, Karnataka, India · +91-9039391582 · [priyanshud141@gmail.com](mailto:priyanshud141@gmail.com)  
[LinkedIn](https://www.linkedin.com/in/priyanshu-mishra-68837511b/) · [GitHub](https://github.com/Priyanshumishra77)

## Professional summary

CPU/SoC design-verification engineer with **nearly five years of hands-on experience** spanning RISC-V CPU verification, custom DSP/ASIP HW/SW co-verification, SoC IP bring-up, and processor architecture/RTL development. Experienced in SystemVerilog/UVM, directed and constrained-random testing, ISA and architectural validation, compiler-driven workloads, ISS-to-RTL functional correlation, regression triage, and waveform-based root-cause analysis.

## Technical skills

**Processor architecture:** RISC-V RV32/RV64, IMAFDC, privileged/unprivileged ISA, CSRs, traps/exceptions, privilege modes, Sv32/Sv39/Sv48/Sv57, CPU pipelines, hazards, LSU, MMU/TLB, caches, ASIP/DSP; Arm Cortex-M55/M33, TrustZone, SAU/MPU.

**Design verification:** SystemVerilog, Verilog, UVM, directed and constrained-random testing, functional coverage, assertion-based verification, vPlans, testbench bring-up, regression automation/triage, waveform debug, RTL root-cause analysis, software-driven verification.

**Processor HW/SW co-verification:** Synopsys ASIP Designer/Programmer, GCC, Clang, Chess compiler, compiler-generated workloads, issue.out-to-HEX flow, ISS-to-RTL functional/architectural correlation, C/C++ and RISC-V assembly.

**SoC and interfaces:** AMBA AXI, AHB 5.0, APB, DMA/eDMA, AHB system control, MMU/TLB, Arteris CodaCache LLC, SRAM lookup tables, arbitration, TrustZone, MCU/DSP/SoC integration.

**Tools and programming:** Cadence Xcelium, SimVision, vManager; Synopsys VCS, Verdi, DVE; QuestaSim; SPIKE, OVPSim, RISC-V GNU toolchain, GDB; Cachegrind, gprof, FlameGraph; C/C++, Python, Perl, Shell/Bash, Makefiles; Git/GitLab, Jira, DesignSync; Linux/Unix.

## Professional experience

### ACL Digital — CPU / SoC Design Verification Engineer
**Jun 2026 – Present | Client project: Renesas | Custom DSP / ASIP verification**

- Perform HW/SW co-verification of a custom DSP/ASIP generated with Synopsys ASIP Designer, correlating compiler/SDK outputs, instruction-set simulator (ISS) behavior, and generated RTL execution.
- Work across approximately 50 processor/DSP functional requirements, including vector operations, saturation, SoftFloat/floating-point behavior, arithmetic corner cases, and application-specific instruction behavior.
- Use Synopsys ASIP Programmer with GCC, Clang, and Chess compiler; integrate compiler-generated issue.out output into the supplied SystemVerilog/UVM framework by converting program images to HEX for Cadence Xcelium RTL simulation.
- Perform ISS-to-RTL functional and architectural correlation, debugging discrepancies across generated instruction streams, reference behavior, simulation traces, and processor state.
- Verify RISC-V AES and SHA-2 functionality on the ASIP Designer-generated TRV32P5X; profile workloads with Cachegrind, gprof, and FlameGraph to inspect execution hotspots.
- Enable RISC-V MCU boot and interrupt flows, automate testcase creation/execution scripts, and contribute to DSP subsystem integration and SoC-level verification.

### SiSoC Semiconductor Technologies — SoC Design Verification Engineer
**May 2025 – May 2026 | Client project: NXP | TrustZone-enabled 16 nm AI SoC**

- Performed pre-silicon functional verification and IP bring-up for a SoC integrating Arm Cortex-M55/M33, GPU, NPU/Arm Ethos, and DSP; adapted UVM infrastructure from an earlier 28 nm platform.
- Owned verification activities for eDMA5, AHBSC, MMU, LLC, and PMUX; authored verification plans for eight IPs and brought up UVM environments for eDMA5, AHBSC, MMU, and LLC, including memory maps, testbench configuration, and register models.
- Developed and executed 70+ AHBSC tests, 25 eDMA5 tests, 13 MMU tests, and 15 LLC tests, spanning 130+ functional scenarios.
- Verified TrustZone secure boot, SAU/MPU setup, VTOR lock-down, MMU translation, TLB/SRAM lookup behavior, multi-port arbitration, and Arteris CodaCache replacement/PLRU behavior.
- Built Perl test-matrix generation, vGen scripts, and VSIF regression configurations; integrated C software-driven SoC tests with UVM and migrated eDMA3 verification infrastructure to eDMA5.
- Identified and debugged eight pre-silicon RTL defects across eDMA5/AHBSC, including interrupt/HRESP gating, reset races, DMA-channel configuration, PBUS arbitration, and AHB protocol violations.
- Triaged waveforms, logs, Tarmac traces, and .lst files, reaching approximately 93% pass rate at the second project milestone.

### SiSoC Semiconductor Technologies — CPU Architecture & Verification Lead
**Feb 2024 – Apr 2025**

- Led a 10-engineer team across architecture, microarchitecture, RTL development, and verification of a high-performance RISC-V CPU from concept through RTL.
- Translated privileged/unprivileged ISA requirements and extensions into implementation and validation tasks.
- Led or supported work across CPU pipelines, hazards, execution units, and memory subsystem integration.
- Supported xv6 OS-based validation and system-level execution/SoC bring-up.
- Contributed to heterogeneous compute/GPGPU activities, architecture labs, verification training, technical knowledge-sharing, and mentoring.

### Chiplogic — RISC-V Processor Verification Engineer
**Feb 2023 – Oct 2023 | Client project: Codasip**

- Verified RV32/RV64 processors across IMAFDC and extensions including Zicclsm, Za64rs, Zifence, and Zicsr.
- Developed assembly tests for pseudo-instructions, hints, traps, misaligned-access faults, illegal instructions, exceptions, and architectural corner cases.
- Validated M/S/U privilege behavior, CSRs, Sv32/Sv39/Sv48/Sv57 virtual-memory modes, and MMU/TLB/cache behavior.
- Investigated RISC-V H-extension behavior and supported simulator bring-up, toolchain internals, linker scripts, Makefiles, and test-build infrastructure.

### Scaledge — DV Engineer, RTL Regression / Front-End DV
**Jun 2022 – Oct 2022 | Client project: Intel via Cyient**

- Ran block-level RTL regressions for Intel RPLS/GNRIO-related IP.
- Debugged assertion and simulation failures through Synopsys Verdi, waveforms, and regression logs.

### Scaledge — Design Verification Engineer, RISC-V CPU
**Sep 2021 – May 2022 | CVA6/Ariane**

- Verified CVA6/Ariane RV32/RV64 IMAFDC implementations with directed/constrained-random tests and RISC-V-DV-generated instruction streams.
- Developed SystemVerilog/UVM tests for LSU, pipeline, and hazard behavior.
- Used SPIKE and OVPSim as architectural reference models to validate instruction behavior and debug processor-level mismatches.

## Education

**B.E., Electronics & Communication Engineering**  
IES College of Technology, Bhopal (RGPV) · 2015–2019 · CGPA: 7.19/10

## Training, workshops and recognition

- CPU Design using Verilog — NIT Trichy workshop.
- Computer Architecture — Saylor Academy certification.
- FPGA Computing Systems — Coursera certification.
- GPU Programming — IIT Madras.
- HPC Synergy: Elevating AI with High-Performance Parallel Computing — IIIT Sri City workshop.
- Machine Learning on Hardware — NIT Trichy workshop.
- Hardware for Deep Learning — Bar-Ilan University workshop.
- Embedded Systems and VLSI Design — IIT Kanpur workshop.
- RISC-V and OpenPOWER in HPC — 2nd workshop, ICS International Conference on Supercomputing, 2021.
- Top 10 Performer — SoC Design using OpenPOWER, VIT & IBM.
- 35th International Conference on VLSI Design — attendee, VLSI Society India.

---

*Updated November 2026. This page is the current web CV; use the dates and role descriptions above as the source of truth for this website.*
