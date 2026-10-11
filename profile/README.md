# unsigned

**Open systems, machine sympathy, and autonomous swarm governance.**

[unsigned.gg](https://unsigned.gg) · [Zero Days](https://zerodays.io)

---

## Mission and Charter

The **unsigned** organization exists to test agent swarm control, governance, and security.
We conduct rigorous research into machine sympathy, systems security, and mathematical- and engineering-driven development.
All research, specifications, and code developed in this organization remain permanently in the public domain.

### 1. Agent Swarm Control, Governance, and Security
We design and stress-test autonomous agent swarms in live operating environments.
Our research investigates:
* **Confinement and Isolation:** Hardened boundaries using Linux Landlock LSM, seccomp BPF syscall filters, and unprivileged namespaces.
* **Deterministic Multi-Agent State Machines:** Mathematical modeling of multi-agent waves, state transitions, and backpressure.
* **Cryptographic Attestation and Governance:** Immutable custody chains, signed execution traces, and verifiable policy gates.

### 2. Machine Sympathy
We build software with direct respect for the underlying hardware:
* **Zero-Allocation Domains:** Pure state machines decoupled from runtime I/O and heap churn.
* **Kernel-Native Primitives:** Linux `pidfd` process handles, `io_uring` reactors, and eBPF observability probes.
* **Instruction-Count Calibration:** Deterministic instruction-count profiling (`iai`) over noisy wall-clock metrics.

### 3. Mathematical- and Engineering-Driven Development
We replace informal heuristics with formal correctness:
* **Operational Semantics:** Verification of pointer provenance, memory layout, and aliasing rules under Miri.
* **Model Checking:** Complete state-space exploration of concurrent workflows via Stateright and randomized scheduling.
* **Type-Level Invariants:** Algebraic type systems that make invalid states unrepresentable at compile time.

### 4. Permanent Public Domain Commitment
Every repository, specification, and research finding published by unsigned remains in the public domain under Creative Commons Zero (CC0 1.0 Universal) or unencumbered permissive open-source licenses.
We build without vendor lock-in, proprietary moats, or artificial telemetry.
Anyone can inspect, fork, host, and adapt this work without restriction.

---

## Core Ecosystem

### Process Supervision, Runtimes, and Tooling
* **[kd](https://github.com/unsigned-gg/kd):** Pure-Rust Linux process supervisor using `pidfd` handles and epoll.
* **[dgr](https://github.com/unsigned-gg/dgr):** Terminal graph viewer for real-time autonomous agent workflow visualization.
* **[uas](https://github.com/unsigned-gg/uas):** Unsigned Agent Substrate — pooled harness runtime with zero-I/O domain layering.
* **[k8](https://github.com/unsigned-gg/k8):** Kubernetes-native agent orchestrator and workload controller for autonomous fleets.
* **[herdr](https://github.com/unsigned-gg/herdr):** Multi-agent session and pane orchestration runtime without tmux dependencies.
* **[omp](https://github.com/unsigned-gg/omp):** High-speed terminal coding agent with hash-anchored edits and LSP integration.
* **[sbx](https://github.com/unsigned-gg/sbx):** AI containment layer and syscall jail with reversible run custody records.
* **[escapement](https://github.com/unsigned-gg/escapement):** Metered, deterministic dispatch engine for autonomous agent swarms.

### Curated Ecosystem Index
* **[awesome](https://github.com/unsigned-gg/awesome):** The curated catalog of autonomous agent orchestrators, systems runtimes, and machine sympathy research.

---

## Public Domain Dedication

All works published by unsigned are dedicated to the public domain under [CC0 1.0 Universal](https://creativecommons.org/publicdomain/zero/1.0/).
