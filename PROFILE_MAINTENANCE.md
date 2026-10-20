# Project Spinosaurus // Profile Maintenance & Publishing Guide

This document provides instructions for publishing, maintaining, and updating the **Project Spinosaurus** GitHub Profile portfolio for **Akshansh** (`AkshanshK04`).

---

## 🚀 How to Publish to GitHub

GitHub displays your profile README when it is stored in a special repository matching your exact GitHub username.

### Step 1: Create the Profile Repository on GitHub
1. Log in to [GitHub](https://github.com).
2. Go to **[github.com/new](https://github.com/new)**.
3. In the **Repository name** field, type your username: `AkshanshK04`.
4. GitHub will show a banner:  
   > *"You found a secret! `AkshanshK04/AkshanshK04` is a special repository that you can use to add a `README.md` to your GitHub profile."*
5. Set the repository visibility to **Public**.
6. **Do not** initialize with a README, .gitignore, or license (we already have all the production files in this workspace).
7. Click **Create repository**.

### Step 2: Push Local Files to the Repository
Open a terminal in this workspace (`d:\Xenix-Forever-04`) and run:

```bash
# Initialize git in this directory (if not already done)
git init -b main

# Stage the README and all custom SVG assets
git add README.md assets/ PROFILE_MAINTENANCE.md

# Commit
git commit -m "feat: launch Project Spinosaurus engineering portfolio"

# Link to your new GitHub profile repository
git remote add origin https://github.com/AkshanshK04/AkshanshK04.git

# Push to GitHub
git push -u origin main
```

Your profile at `https://github.com/AkshanshK04` will immediately render the custom banner, species mark, architecture diagram, and portfolio sections.

---

## 📁 Repository Structure

```text
.
├── assets/
│   ├── spinosaurus-banner.svg     # 900x320 main hero banner with blueprint grid & anatomical callouts
│   ├── spinosaurus-mark.svg       # 160x160 species reticle emblem
│   ├── section-divider.svg        # 900x32 geological stratum + digital clock pulse divider
│   └── architecture-diagram.svg   # 880x370 verified 6-stage pipelined CPU & IoT co-design datapath
├── README.md                      # Production GitHub profile README
└── PROFILE_MAINTENANCE.md         # This maintenance guide & evidence ledger
```

---

## 📑 Evidence Ledger (Audited Repositories)

Every technical claim in `README.md` was established from actual source files audited during the project audit:

| Repository | Verified Languages | Key Inspected Source Files | Architectural Concepts Verified |
| :--- | :--- | :--- | :--- |
| [`Ak-16b-A-16-bit-CPU-`](https://github.com/AkshanshK04/Ak-16b-A-16-bit-CPU-) | Verilog | `cpu_top_pipeline.v`, `hazard_unit.v`, `forwarding_unit.v`, `def_opcode.v` | 6-stage pipeline (IF/ID/EX1/EX2/MEM/WB), RAW forwarding logic, load-use stall insertion, branch resolution in EX2. |
| [`Secure_iot_cpu_system`](https://github.com/AkshanshK04/Secure_iot_cpu_system) | Verilog, C, FreeRTOS, Python | `pipeline_cpu.v`, `hazard_unit.v`, `interrupt_controller.v`, `sensor.c` | Hardware-software co-design: vectored interrupt `0x00F0` with ACK handshake, MMIO registers `0xF0-0xF2`, ADS1115 ADC + MPU6050 IMU FreeRTOS firmware. |
| [`Cache-Simulator`](https://github.com/AkshanshK04/Cache-Simulator) | C (C99) | `main.c`, `README.md` | Configurable cache hierarchy, bitwise tag/index extraction, true LRU replacement policy, write-back with dirty bit tracking (85-95% simulated hit rates). |
| [`rizz`](https://github.com/AkshanshK04/rizz) | Rust | `src/main.rs`, `Cargo.toml`, `examples/*.rz` | >45,000 characters of Rust. Full lexer, parser, AST evaluation, scoped environment (`Rc<RefCell<Env>>`), interactive REPL, bubble sort and Fibonacci test suites. |
| [`DSAfromScratch`](https://github.com/AkshanshK04/DSAfromScratch) | C | 260+ `.c` problem solutions | Low-level C programming, pointer manipulation, dynamic programming, linked lists, sliding window algorithms. |
| [`Digital-Signature-Generation-and-Verification`](https://github.com/AkshanshK04/Digital-Signature-Generation-and-Verification) | Python | `code` | RSA cryptosystem from first principles: extended Euclidean algorithm (`extended_gcd`), modular inverse, SHA-256 signing/verification. |

---

## 🛠️ How to Add a New Project

To add a new project to `README.md`, follow the **Specimen File** format:

```markdown
### [SPECIMEN FILE 0X] · Project Title

> **Core Focus:** Primary Engineering Disciplines  
> **Source Repository:** [`RepoName`](https://github.com/AkshanshK04/RepoName)  
> **Status:** `Maturity Label (e.g. Functional Implementation // Prototype // Active Development)`  
> **Technologies:** `Technology 1` · `Technology 2` · `Technology 3`

Brief 1-2 sentence description explaining the problem addressed and actual result.

* **Key Engineering Aspects:**
  * Bullet 1: Core algorithmic or architectural design.
  * Bullet 2: Significant implementation decision or trade-off.
* **Implementation Detail:** Distinctive, verified detail (e.g., custom protocol, performance figure, or test suite).
* **Maturity & Next Step:** Current state and defensible next milestone.
```

---

## 🎨 Design System Reference

If you wish to edit the SVG assets or add new graphics:

* **Obsidian (Base canvas / deep slate):** `#101513` / `#0E1311`
* **Graphite (Card surface / container):** `#1B211E` / `#131C18`
* **Forest (Subdued dark foliage / water):** `#263D32` / `#1E3228`
* **Swamp Teal (Aquatic accent / bus wires):** `#557C73`
* **Amber (Specimen highlight / signal pulses):** `#C79A55`
* **Sediment (Annotation lines / strata):** `#A69B85`
* **Fossil Ivory (High-contrast typography):** `#E8E1D1`

All SVG files are self-contained vector graphics using standard web fonts (`ui-monospace`, `-apple-system`, `monospace`), requiring no external network requests or JavaScript execution.
