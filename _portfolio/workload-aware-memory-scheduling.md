---
title: "Workload-Aware Memory Scheduling for a RISC-V CPU and Inference Accelerator"
excerpt: "Independent architecture research proposal on memory arbitration, cache allocation, and mixed-workload fairness."
collection: portfolio
---

## Status

**Research proposal only.** The SoC and accelerator have not been implemented, and no simulation or physical measurement is being claimed.

## Research question

How do memory scheduling and last-level-cache allocation policies change accelerator throughput, CPU request latency, and fairness when one RISC-V application-processor model and one inference accelerator share memory?

The initial concept combined CPU cores, GPU, NPU, TPU, HBM, coherent mesh, AI-guided scheduling, DVFS, and edge and data-center targets. My handwritten first-step notes also explored cache replacement, dynamic core allocation, power gating, YAML-to-RTL workflows, interfaces, verification, and Linux bring-up. These ideas remain useful design history, but the first study needs a narrower, measurable boundary.

## Early design notes

These two photographs preserve my first handwritten architecture sketches. They are early ideas, not finalized specifications or evidence of implementation.

<figure>
  <img src="{{ site.baseurl }}/images/heterogeneous-soc-initial-notes-1.svg" alt="First handwritten page of early heterogeneous SoC architecture notes" loading="lazy">
  <figcaption>Early design notes — page 1.</figcaption>
</figure>

<figure>
  <img src="{{ site.baseurl }}/images/heterogeneous-soc-initial-notes-2.svg" alt="Second handwritten page of early heterogeneous SoC architecture notes" loading="lazy">
  <figcaption>Early design notes — page 2.</figcaption>
</figure>

## First-study scope

The proposed baseline uses one simulator-supported RISC-V CPU model, one abstract inference accelerator, private CPU caches, a shared last-level cache, and a documented memory path. The study will compare the simulator's default arbitration with fixed accelerator weighting, bounded priority, and cache partitioning where supported.

The primary measures are accelerator throughput, CPU request latency, per-client slowdown, fairness, cache misses, accelerator stalls, and external-memory traffic. Energy, area, frequency, and temperature are out of scope unless a credible model or implementation becomes available.

## Method and evidence

The work begins with a simulator feasibility check and deterministic CPU-only and accelerator-only validation. It then compares isolated and mixed workloads while changing one policy dimension at a time. Configurations, workload provenance, scripts, raw measurements, and limitations will accompany any future results.

The study does not assume a speedup or novelty in advance. Any conclusion will be tied to a named model, version, workload, configuration, and measured data.

## Why the original numbers were removed

The earlier drafts included pipeline and cache sizes, bandwidth, IPC, latency, power, benchmark, and efficiency estimates without a reproducible implementation or measurement method; the versions also conflicted on several parameters. These are not treated as results or fixed design requirements. For example, eight cores with an eight-wide issue limit imply a theoretical ceiling of 64 issued instructions per cycle only under ideal assumptions, not a measured throughput result.

RVA23 is an architectural profile and does not define a CPU microarchitecture. The first study will use “inference accelerator” as a generic block rather than treating Google's TPU product family as a generic SoC component. Coherence, shared virtual memory, and CXL support will be stated only if the chosen model and configuration implement them.

## Next milestones

1. Confirm simulator and model support for the selected CPU, cache, interconnect, and accelerator abstraction.
2. Freeze a reproducible baseline and validate traffic accounting.
3. Run controlled scheduling and cache-allocation comparisons.
4. Publish results with scripts, configurations, raw data, and limitations.

## References

- RISC-V International, [RVA23 Profile](https://docs.riscv.org/reference/rva23/index.html) and [V Vector Extension](https://docs.riscv.org/reference/isa/unpriv/v-st-ext).
- gem5, [Ruby memory-system documentation](https://www.gem5.org/documentation/general_docs/ruby/).
- MLCommons, [MLPerf Inference documentation](https://docs.mlcommons.org/inference/index_gh/).
- Compute Express Link Consortium, [CXL 3.0 Specification](https://computeexpresslink.org/wp-content/uploads/2024/02/CXL-3.0-Specification.pdf).

Further technical details and reproducible artifacts will be added as the study progresses.
