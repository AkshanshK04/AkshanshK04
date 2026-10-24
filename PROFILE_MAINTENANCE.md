# Project Spinosaurus: Profile maintenance and publishing guide

This document provides instructions for publishing, maintaining, and updating the Project Spinosaurus GitHub profile portfolio for Akshansh (`AkshanshK04`).

---

## How to publish to GitHub

GitHub displays your profile README when it is stored in a repository matching your GitHub username.

### Step 1: Create the profile repository on GitHub
1. Log in to GitHub.
2. Go to https://github.com/new.
3. In the repository name field, enter your username: `AkshanshK04`.
4. Set the repository visibility to Public.
5. Do not initialize with a README, .gitignore, or license.
6. Click Create repository.

### Step 2: Push local files to the repository
Open a terminal in this workspace (`d:\Xenix-Forever-04`) and run:

```bash
# Initialize git in this directory if needed
git init -b main

# Stage the README and assets
git add README.md assets/ PROFILE_MAINTENANCE.md

# Commit
git commit -m "feat: launch Project Spinosaurus engineering portfolio"

# Link to your GitHub profile repository
git remote add origin https://github.com/AkshanshK04/AkshanshK04.git

# Push to GitHub
git push -u origin main
```

---

## Repository structure

```text
.
├── assets/
│   ├── spinosaurus-xenix.jpg      # Main hero image with Spinosaurus and Xenix dialogue
│   ├── spinosaurus-banner.svg     # 900x320 hero banner with blueprint grid and anatomical callouts
│   ├── spinosaurus-mark.svg       # 160x160 species reticle emblem
│   ├── section-divider.svg        # 900x32 geological stratum and clock divider
│   └── architecture-diagram.svg   # 880x370 verified 6-stage pipelined CPU datapath
├── README.md                      # Production GitHub profile README
└── PROFILE_MAINTENANCE.md         # Maintenance guide and evidence ledger
```

---

## Evidence ledger

Every technical claim in README.md was established from audited source files:

| Repository | Verified languages | Key inspected source files | Architectural concepts verified |
| :--- | :--- | :--- | :--- |
| [`Ak-16b-A-16-bit-CPU-`](https://github.com/AkshanshK04/Ak-16b-A-16-bit-CPU-) | Verilog | `cpu_top_pipeline.v`, `hazard_unit.v`, `forwarding_unit.v`, `def_opcode.v` | 6-stage pipeline (IF/ID/EX1/EX2/MEM/WB), RAW forwarding logic, load-use stall insertion, branch resolution in EX2. |
| [`Secure_iot_cpu_system`](https://github.com/AkshanshK04/Secure_iot_cpu_system) | Verilog, C, FreeRTOS, Python | `pipeline_cpu.v`, `hazard_unit.v`, `interrupt_controller.v`, `sensor.c` | Hardware-software co-design: vectored interrupt `0x00F0` with ACK handshake, MMIO registers `0xF0-0xF2`, ADS1115 ADC + MPU6050 IMU FreeRTOS firmware. |
| [`Cache-Simulator`](https://github.com/AkshanshK04/Cache-Simulator) | C99 | `main.c`, `README.md` | Configurable cache hierarchy, bitwise tag/index extraction, true LRU replacement policy, write-back with dirty bit tracking (85% to 95% simulated hit rates). |
| [`rizz`](https://github.com/AkshanshK04/rizz) | Rust | `src/main.rs`, `Cargo.toml`, `examples/*.rz` | Over 45,000 characters of Rust. Full lexer, parser, AST evaluation, scoped environment (`Rc<RefCell<Env>>`), interactive REPL, bubble sort and Fibonacci test suites. |
| [`DSAfromScratch`](https://github.com/AkshanshK04/DSAfromScratch) | C | 260+ `.c` problem solutions | Low-level C programming, pointer manipulation, dynamic programming, linked lists, sliding window algorithms. |
| [`Digital-Signature-Generation-and-Verification`](https://github.com/AkshanshK04/Digital-Signature-Generation-and-Verification) | Python | `code` | RSA cryptosystem from first principles: extended Euclidean algorithm (`extended_gcd`), modular inverse, SHA-256 signing and verification. |

---

## How to add a new project

To add a new project to README.md, follow this format:

```markdown
### [Project title](https://github.com/AkshanshK04/RepoName)
> Primary technologies

* **Core design.** Algorithmic or architectural implementation.
* **Key decision.** Implementation decision or trade-off.
* **Verification.** Distinctive verified metric, test suite, or protocol.
```

---

## Design system reference

Design tokens for SVG assets and color palettes:

* Obsidian: `#101513` and `#0E1311`
* Graphite: `#1B211E` and `#131C18`
* Forest: `#263D32` and `#1E3228`
* Swamp Teal: `#557C73`
* Amber: `#C79A55`
* Sediment: `#A69B85`
* Fossil Ivory: `#E8E1D1`

All SVG files are self-contained vector graphics using standard web fonts, requiring no external network requests or JavaScript execution.
