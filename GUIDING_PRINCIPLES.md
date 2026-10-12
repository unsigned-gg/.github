# Guiding Principles, Mottos & Northstars

> **Organization:** [unsigned](https://unsigned.gg) - [Zero Days](https://zerodays.io)  
> **Status:** Foundational Doctrine  
> **License:** Dedicated to the public domain under [CC0 1.0 Universal](https://creativecommons.org/publicdomain/zero/1.0/)

---

## 1. Mottos

```
   "A better future through mutual cooperation between man and machine."
   "Priced like plumbing, unencumbered by design."
   "Respect the silicon. Protect the human."
   "Open compute, sovereign custody."
   "Math over marketing. Proof over persuasion."
   "Build what we would rent."
```

---

## 2. Our Northstars

Our engineering decisions orient around four permanent Northstars:

1. **Zero-Overhead Systems Engineering:**
   Every abstraction must justify its existence in cache lines, CPU cycles, and memory footprint. We refuse software bloat that conceals inefficiency behind hardware abundance.
2. **Universal Accessibility Without Proprietary Capture:**
   Every tool, architecture, and finding belongs to humanity. We build software that anyone can inspect, compile, deploy, and fork without licenses, subscriptions, or telemetry traps.
3. **Agent Governance That Elevates Human Agency:**
   Autonomous systems must never become black-box tyrants. Swarms must execute under mechanical gates, formal contracts, and human-sovereign tripwires.
4. **Privacy as a Fundamental Physical Law:**
   Confidentiality and user privacy must not depend on contractual trust. They must be guaranteed through cryptographic mathematics, local-first architectures, and zero-telemetry runtimes.

---

## 3. The Seven Guiding Principles

### I. Machine Sympathy Over Synthetic Fluff
We write software with visceral respect for the metal:
* We favor Linux kernel-native primitives (`pidfd`, `io_uring`, Landlock LSM, eBPF) over synthetic user-space abstraction layers.
* We structure domain logic as zero-allocation, zero-I/O state machines.
* We treat CPU cache lines, memory alignment, and register allocation as primary design concerns.

### II. Soundness Always Trumps Speed
When performance optimizations conflict with mathematical soundness:
* Soundness wins unconditionally.
* We refuse raw pointer tricks, lock-free hacks, or undefined behaviors that fail Miri verification or lack formal inductive safety proofs.
* Speed earned by breaking correctness is not an optimization; it is technical debt disguised as throughput.

### III. Build What We Would Rent
We do not build speculative products or enterprise vanity features:
* We engineer the exact tools, runtimes, and infrastructure we require to run our own autonomous development swarms.
* We dogfood our kernels, supervisors, and CLIs under real production strain every day.

### IV. Mechanical Gates Over Social Consensus
Human review is essential for intent, but safety must be mechanical:
* Invariant checks, linter rules, memory bounds, and escape tests must be enforced by automated juries.
* If a test cannot fail, it proves nothing. If a policy requires human memory to enforce, it is broken.

### V. Deterministic Evidence Over Subjective Claims
A claim is expensive the moment it leaves the terminal:
* We replace wall-clock microbenchmarks with instruction-count profiling (`iai`).
* We replace arbitrary `sleep()` loops with model-checked state-space reachability (`stateright`).
* We calibrate every assertion to reproducible evidence.

### VI. Radical Simplicity and Ergonomics
Keystrokes and mental context are precious natural resources:
* We prefer compact, two-letter command-line ergonomics (`kd`, `od`, `yx`, `rs`) over verbose, multi-word CLI taxonomies.
* We eliminate boilerplate, redundant config flags, and unnecessary dependencies.
* **Registry Discipline:** Every package reservation follows strict anti-squatting discipline: claimed crates publish immediate, substantive code with zero vanity stubs.

### VII. Permanent Public Domain Dedication
We reject proprietary moats, patent hoarding, and vendor lock-in:
* All research, specifications, and code remain in the public domain under CC0 1.0 Universal.
* If an engineer or organization leaves our platform, they take everything: their data, their configurations, their weights, and their freedom.
