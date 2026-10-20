<div align="center">

#  XENIX FOREVER

<p align="center">
  <img src="assets/spinosaurus-xenix.jpg" alt="Spinosaurus: I'm a big fan of Xenix" width="680" style="border-radius: 12px;" />
</p>

### **Low-Level Systems · Computer Architecture · Digital Logic · Rust & C**

```text
"Building processors from gate-level logic upward and breaking systems software.
 Big fan of vintage Unix, pipelined architectures, and Spinosaurus aegyptiacus."
```

<p align="center">
  <a href="https://github.com/AkshanshK04"><img src="https://img.shields.io/badge/GitHub-AkshanshK04-181717?style=for-the-badge&logo=github" alt="GitHub" /></a>
  <img src="https://img.shields.io/badge/ARCH-16--Bit%20RISC-557c73?style=for-the-badge" alt="16-Bit RISC" />
  <img src="https://img.shields.io/badge/STACK-Verilog%20%7C%20C%20%7C%20Rust-c79a55?style=for-the-badge" alt="Verilog C Rust" />
  <img src="https://img.shields.io/badge/SPECIES-Spinosaurus-263d32?style=for-the-badge" alt="Spinosaurus" />
</p>

</div>

---

## ⚡ What I Do

I deconstruct computing systems from physical hardware up to the software runtime:

* 🔬 **Computer Architecture & Digital Logic:** Designing 16-bit pipelined CPU datapaths, forwarding multiplexers, and hazard units in **Verilog**.
* ⚙️ **Systems Programming:** Writing memory-conscious software in **C** (cache simulators, data structures) and **Rust** (interpreters, parsers, AST evaluation).
* 🛰️ **Embedded Hardware:** Interfacing **ESP32** microcontrollers with real-time I2C telemetry (ADC, 6-DOF IMUs) and hardware interrupt lines under **FreeRTOS**.
* 🦖 **Paleontology:** Deep curiosity about *Spinosaurus aegyptiacus*—the apex semi-aquatic Cretaceous predator with neurovascular pressure-sensor snout pits and a 1.8m neural spine sail.

---

## 🔥 Featured Builds

### ⚡ [AK-16B: 16-Bit Pipelined CPU](https://github.com/AkshanshK04/Ak-16b-A-16-bit-CPU-)
> **Verilog · Icarus Verilog · GTKWave**
* **6-Stage Pipeline:** `IF` ➔ `ID` ➔ `EX1` ➔ `EX2` ➔ `MEM` ➔ `WB`.
* **Zero-Bubble RAW Forwarding:** Dynamic forwarding unit routes results from `EX2` and `MEM` stages directly into `EX1` ALU operands.
* **Hardware Hazard Detection:** Automatically detects load-use conflicts, stalls the PC, and injects pipeline bubbles.
* **Custom ISA:** Full instruction decoder handling R-type arithmetic, sign-extended I-types, branches (`BEQ`/`BNE`), and jumps.

<details>
<summary><b>📐 View Processor Architecture Schematic</b></summary>
<br />
<div align="center">
  <img src="assets/architecture-diagram.svg" alt="AK-16B Architecture" width="100%" />
</div>
</details>

---

### 🧠 [Cache Simulator](https://github.com/AkshanshK04/Cache-Simulator)
> **C (C99) · Memory Systems**
* Configurable cache simulator supporting **Direct-Mapped** and **N-Way Set-Associative** configurations.
* Bitwise address decomposition into Tag, Index, and Block Offset using logarithmic shifts.
* Implements **True LRU replacement** and **Write-Back with dirty bit tracking**; demonstrated **85–95% hit rates**.

---

### 🦀 [Rizz: Language Runtime & Interpreter](https://github.com/AkshanshK04/rizz)
> **Rust · AST Parser · REPL**
* Complete tree-walking programming language interpreter written in **Rust** (>45k chars).
* Lexer, recursive-descent parser, Abstract Syntax Tree, and environment scoping via `Rc<RefCell<Env>>`.
* Features mutable (`lit`) vs immutable (`rizz`) variable bindings, loops, recursion, and verified algorithms (bubble sort, Fibonacci).

---

### 🛰️ [Secure IoT Edge Co-Design](https://github.com/AkshanshK04/Secure_iot_cpu_system)
> **Verilog · C · ESP32 · FreeRTOS**
* Pipelined CPU core with memory-mapped alert registers (`0xF0–0xF2`) and a **vectored interrupt controller** (vector `0x00F0`).
* Real-time C firmware for ESP32 polling an ADS1115 16-bit ADC and MPU6050 IMU over I2C, streaming normalized telemetry packets to the CPU.

---

### 🗡️ [DSA from Scratch](https://github.com/AkshanshK04/DSAfromScratch)
> **C · 260+ Solutions**
* Core data structures, pointer arithmetic, sliding window, and dynamic programming in raw C without standard library containers.

---

## 🦖 The Mascot: Spinosaurus aegyptiacus

```text
┌────────────────────────────────────────────────────────────────────────┐
│ Cretaceous Delta Predator · 95 Ma · Kem Kem Beds, Morocco              │
│ • Neurovascular snout foramina -> biological hydrophone array          │
│ • Dense pachyosteosclerotic bones -> diving ballast mechanics          │
│ • Massive M-shaped dorsal sail -> thermoregulation & hydrodynamic helm │
│ • Deep caudal fin -> paddle-driven aquatic propulsion                  │
└────────────────────────────────────────────────────────────────────────┘
```

---

## 📊 Activity & Terminal

<div align="center">

<a href="https://github.com/AkshanshK04">
  <img src="https://github-readme-stats.vercel.app/api?username=AkshanshK04&show_icons=true&theme=tokyonight&hide_border=true&bg_color=101412&title_color=c79a55&icon_color=557c73&text_color=e8e1d1" alt="GitHub Stats" />
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=AkshanshK04&layout=compact&theme=tokyonight&hide_border=true&bg_color=101412&title_color=c79a55&text_color=e8e1d1" alt="Top Languages" />
</a>

<br /><br />

```text
>>> CONNECT: akshanshk0406@gmail.com | github.com/AkshanshK04
>>> STATUS : Hacking on custom silicon & low-level runtimes.
```

<sub>Built with 🦖 by <b>Xenix Forever</b></sub>

</div>
