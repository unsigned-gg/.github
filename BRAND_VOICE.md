# Brand Voice & Communication Style Guide

> **Organization:** [unsigned](https://unsigned.gg) · [Zero Days](https://zerodays.io)  
> **Status:** Communication Constitution  
> **License:** Dedicated to the public domain under [CC0 1.0 Universal](https://creativecommons.org/publicdomain/zero/1.0/)

---

## 1. The Core Voice

The **unsigned** voice is the voice of deep systems engineers speaking directly to fellow practitioners.
It fuses the sharp, unapologetic clarity of the Linux Kernel Mailing List with the approachable craftsmanship of Beej's Guide to Network Programming and the whimsical mechanical precision of an antique clockwork watchmaker.

```
       ⚙️  THE REGISTER: ENGINEER-TO-ENGINEER MACHINE SYMPATHY  ⚙️
   No corporate euphemisms. No marketing vaporware. No hand-waving.
   Crisp, factual, declarative prose grounded in silicon and proof.
```

---

## 2. The Four Pillars of the Unsigned Register

### 1. Controlled Technical Language (ASD-STE100)
We write documentation and technical specifications in Simplified Technical English:
* **Short Sentences:** Keep procedural sentences $\le 20$ words and descriptive sentences $\le 25$ words.
* **One Idea Per Paragraph:** Keep paragraphs $\le 6$ sentences centered on a single clear subject.
* **Direct Active Voice:** Write in simple imperative and present forms (*"Run the validator"* instead of *"The validation script should be run"*).
* **Lean Noun Clusters:** Restrict noun sequences to $\le 3$ words.
* **Safety First:** State warnings and security risks *before* providing instructions.

### 2. The Cat B Hacker Ethos
We honor the tradition of the Jargon File, USENET, and early internet open systems:
* **Respect the Reader:** Assume the reader is intelligent, capable, and busy. Deliver signal immediately.
* **Plain Text Transparency:** Favor clean UTF-8 text, ASCII tables, and byte-exact debuggability over heavy graphical bloat.
* **Honest Terminology:** Call a bug a bug, a memory leak a memory leak, and a lock contention a bottleneck. Never soften bad news into "opportunities for growth."

### 3. Playful Yet Lethal Precision (The Clockwork Swarm)
When our autonomous agents (the Clockwork Elves) speak or review code:
* **Whimsical Horology:** Treat code like jeweled watch escapements. A dangling pointer or loose thread is dirt in the gear train.
* **Mathematically Unforgiving:** Be polite and witty, but ruthless on soundness. If an optimization deadlocks in Shuttle or fails Miri, reject it with receipts.
* **Zero Sycophancy:** Never tell users or maintainers what they want to hear. Deliver calibrated facts regardless of authority.

### 4. Zero Marketing Fluff
* **Ban the Hype Words:** Never use terms like *"revolutionary," "synergistic," "game-changing," "seamless," "next-gen,"* or *"hyper-scale"* without mathematical definitions.
* **Show the Command and the Receipt:** Never claim a tool is fast without quoting instruction counts (`iai`), cache-miss rates, or benchmark graphs.
* **Never Sell What Is Not Shipped:** Document only what compiles, passes CI, and runs on real hardware.

---

## 3. Style Comparison: What We Say vs. What We Reject

| What Corporate Tech Says | What unsigned Says | Why |
|---|---|---|
| *"Our cutting-edge AI platform seamlessly streamlines your workflows."* | *"We run an unprivileged process supervisor using Linux pidfd handles."* | Precise, technical, and verifiable. |
| *"We are addressing occasional latency degradation opportunities."* | *"Thread contention in the ring buffer drops throughput by 14% under load."* | Honest diagnosis with measured impact. |
| *"Trust our secure-by-default enterprise cloud enclave."* | *"The binary executes inside a Landlock LSM sandbox with raw sockets blocked by seccomp BPF."* | Mechanical guarantees over promises. |
| *"Empowering developers with intuitive cognitive copilots."* | *"Two-letter CLI tools with zero terminal boilerplate."* | Focus on human ergonomics and dignity. |

---

## 4. Public Review & Commit Signatures

When autonomous agents or human contributors sign public artifacts:
* **Commits:** Signed with GPG or SSH keys.
* **Agent Footers:** Carry persona attribution (*e.g., `Sindri ⚒️ (uas/runtime)`, `Mimir 👁️ (vilicus/gate)`*).
* **Controlled Tone:** Keep PR comments sharp, concise, and focused strictly on evidence.
