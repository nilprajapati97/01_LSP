<div align="center">

<div style="background: linear-gradient(135deg, #20B2AA, #0A2A28); padding: 40px 50px; border-radius: 20px; margin-bottom: 24px; box-shadow: 0 8px 30px rgba(0,0,0,0.4);">

<h1 style="color: white; margin: 0 0 12px 0; font-size: 2.8em; letter-spacing: 2px;">🐧 Linux System Programming Explorer</h1>

<p style="color: rgba(255,255,255,0.9); margin: 0; font-size: 1.2em; line-height: 1.6;">
A comprehensive deep-dive into Linux internals — from system calls to kernel modules,<br>
from process management to 70 days of OS exploration.
</p>

</div>

[![Language](https://img.shields.io/badge/Language-C-1E90FF?style=for-the-badge&logo=c&logoColor=white)](https://en.wikipedia.org/wiki/C_(programming_language))
[![OS](https://img.shields.io/badge/OS-Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)](https://kernel.org)
[![Topics](https://img.shields.io/badge/Topics-LSP%20%7C%20IPC%20%7C%20Threads%20%7C%20Kernel-20B2AA?style=for-the-badge)](.)
[![Days](https://img.shields.io/badge/ExploringOS-70%20Days-6A5ACD?style=for-the-badge)](ExploringOS/)
[![Notes](https://img.shields.io/badge/Notes-10%20Docs-2E8B57?style=for-the-badge)](LSP_Notes/)

</div>

---

## 🗂️ Repository Structure

```
01_LSP_Explore/
├── 📁 Class/               # Hands-on LSP code labs & assignments
│   ├── 01_Library/         # Static & dynamic library creation
│   ├── 02_ProcessManagement/  # fork(), exec(), wait(), pid
│   ├── 03_signalManagement/   # signal(), sigaction()
│   ├── 04_Signal_Management/  # Advanced signal handling
│   ├── 05_IPC/             # Pipe, FIFO, MQ, Shared Memory, Semaphore
│   ├── 06_Thread/          # POSIX threads — create, join, detach
│   └── ...                 # assignments, fm, ipc, library, practice
├── 📁 Compiler/            # GCC internals & compilation stages
│   ├── ExploreCPU.c        # C source
│   ├── ExploreCPU.i        # Pre-processed output
│   └── ExploreCPU.s        # Assembly output
├── 📁 ExploringOS/         # 70-day OS deep-dive course
│   └── src/                # Day-wise Markdown notes + code + diagrams
└── 📁 LSP_Notes/           # Curated study notes for LSP topics
```

---

## 📚 Modules

### 💻 [Class](Class/README.md) — Linux System Programming Labs

Structured, hands-on C programming labs covering the full Linux System Programming curriculum.

| # | Module | Key Concepts |
|:-:|:--|:--|
| 01 | [Library](Class/01_Library/README.md) | `ar`, `ranlib`, `gcc -shared`, static vs dynamic |
| 02 | [Process Management](Class/02_ProcessManagement/README.md) | `fork()`, `exec()`, `wait()`, `getpid()` |
| 03 | [Signal Management](Class/03_signalManagement/README.md) | `signal()`, `sigaction()`, `sigset_t` |
| 04 | [Advanced Signals](Class/04_Signal_Management/README.md) | `sa_flags`, `sa_mask`, real-time signals |
| 05 | [IPC](Class/05_IPC/README.md) | Pipe, FIFO, Message Queue, Shared Memory, Semaphore |
| 06 | [Threads](Class/06_Thread/README.md) | `pthread_create()`, `pthread_join()`, `pthread_detach()` |

> **Prerequisites:** Library functions · Structures · Pointers · Bit-fields · Unions

---

### 🔨 [Compiler](Compiler/README.md) — GCC Internals & Compilation Pipeline

Explores the four-stage GCC compilation process by examining each intermediate output.

```
Source (.c)  →  Pre-process (.i)  →  Compile (.s)  →  Assemble (.o)  →  Link (ELF)
```

| Stage | File | Description |
|:--|:--|:--|
| C Source | `ExploreCPU.c` | Original C code |
| Pre-processed | `ExploreCPU.i` | Macros expanded, headers inlined |
| Assembly | `ExploreCPU.s` | Human-readable x86/ARM assembly |

---

### 🐧 [ExploringOS](ExploringOS/README.md) — 70-Day OS Deep-Dive

A structured 70-day journey through Operating System internals, kernel mechanics, and advanced Linux topics.

<details>
<summary><b>📅 Day-wise Curriculum (click to expand)</b></summary>

#### 🔵 Phase 1 — Process & Thread Fundamentals (Days 1–14)
| Day | Topic |
|:-:|:--|
| 1 | Process Concept |
| 2 | Process States & Transitions |
| 3 | Process Creation |
| 4 | Process Scheduling Basics |
| 5 | Scheduling Algorithms |
| 6 | Context Switching |
| 7 | Thread Concept |
| 8 | Thread Creation & Management |
| 9 | Threads vs Processes |
| 10 | Multithreading Models |
| 11 | Concurrency Fundamentals |
| 12 | Mutex & Semaphores |
| 13 | Deadlock |
| 14 | Deadlock Detection Algorithms |

#### 🟢 Phase 2 — Memory Management (Days 15–24)
| Day | Topic |
|:-:|:--|
| 15 | Memory Management |
| 16 | Logical vs Physical Address Space |
| 17 | Contiguous Memory Allocation |
| 18 | Memory Allocation Algorithms |
| 19 | Paging Mechanism |
| 20 | Page Replacement Algorithms |
| 21 | Memory Segmentation |
| 22 | Virtual Memory |
| 23 | Memory Allocation Internals |
| 24 | Dynamic Memory Management |

#### 🟡 Phase 3 — Filesystem & I/O (Days 25–34)
| Day | Topic |
|:-:|:--|
| 25 | File System |
| 26 | File System Structure |
| 27 | File Allocation Methods |
| 28 | Free Space Management |
| 29 | File Protection Mechanisms |
| 30 | I/O System Management |
| 31 | Disk Scheduling Algorithms |
| 32 | Interrupt Handling |
| 33 | Advanced System Call Implementation |
| 34 | Kernel Module Development |

#### 🟠 Phase 4 — IPC, Scheduling & RTOS (Days 35–50)
| Day | Topic |
|:-:|:--|
| 35 | Inter-Process Communication |
| 36 | Shared Memory |
| 37 | Socket Programming |
| 38 | CPU Scheduling |
| 39 | Real-Time OS Internals |
| 40 | Linux Kernel Memory Management |
| 41 | Process Synchronization |
| 42 | Resource Allocation Graph Theory |
| 43 | Memory Fragmentation |
| 44 | Cache Management Internals |
| 45 | File System Journaling |
| 46 | Device Driver |
| 47 | Security Mechanisms |
| 48 | Process Scheduling Simulator |
| 49 | Network File System Internals |
| 50 | Virtual Memory Management System |

#### 🔴 Phase 5 — Advanced Kernel & Security (Days 51–70)
| Day | Topic |
|:-:|:--|
| 51 | Error Handling Kernel Mechanisms |
| 52 | Advanced Virtual Memory & Hypervisor |
| 53 | Distributed OS Algorithms |
| 54 | Embedded OS Kernel Design |
| 55 | Advanced Microkernel Architecture |
| 56 | OS Performance Profiling & Analysis |
| 57 | Fault Tolerance Mechanisms |
| 58 | Advanced Load Balancing |
| 59 | Containerization Internals |
| 60 | Kernel Synchronization Primitives |
| 61 | Security Vulnerability Analysis |
| 62 | Cryptographic Kernel Mechanisms |
| 63 | Kernel-Level Malware Detection |
| 64 | Kernel Trace Analysis |
| 65 | Memory Allocation Design |
| 66 | Advanced IPC Mechanisms |
| 67 | Kernel Debugging Mechanisms |
| 68 | Dynamic Syscall Handling |
| 69 | Advanced Process Scheduling |
| 70 | Thread Synchronization |

</details>

---

### 📝 [LSP_Notes](LSP_Notes/README.md) — Study Notes

Concise reference notes covering core Linux System Programming concepts.

| # | Document | Topic |
|:-:|:--|:--|
| 000 | [Static Lib vs Dynamic Lib](LSP_Notes/000_StaticLibVsDynamicLib.Md) | Library types, `ar`, `ld`, `dlopen` |
| 001 | [LSP Introduction](LSP_Notes/001_LSP_Intro.md) | Overview of the LSP curriculum |
| 002 | [LSP Basics](LSP_Notes/002_LSP.md) | System calls, POSIX, glibc |
| 003 | [LSP Introduction (Extended)](LSP_Notes/002_LSP_Introduction.md) | Extended intro notes |
| 004 | [Process Time](LSP_Notes/003_LSP_%20ProcessTime.md) | `clock()`, `time()`, process timing |
| 005 | [Random Numbers](LSP_Notes/005_LSP_Random_Number.md) | `rand()`, `srand()`, `/dev/urandom` |
| 006 | [Process Control Block](LSP_Notes/006_LSP_Process_Controll_Block.md) | PCB structure, kernel `task_struct` |
| 007 | [PCB Deep Dive](LSP_Notes/007_LSP_PCB.md) | Fields, context, scheduling |
| 008 | [System Functions](LSP_Notes/008_LSP_System_Function.md) | Key POSIX system call reference |
| 009 | [LSP Advanced](LSP_Notes/009_LSP.md) | Advanced topics |

---

## ⚙️ Getting Started

### Prerequisites

```bash
# Linux (Ubuntu/Debian)
sudo apt update && sudo apt install -y gcc make binutils gdb strace ltrace
```

### Build & Run a Code Example

```bash
# Clone the repository
git clone https://github.com/nilprajapati97/01_LSP_Explore.git
cd 01_LSP_Explore

# Compile a process management example
gcc -o fork_demo Class/02_ProcessManagement/01_fork.c
./fork_demo

# Compile with threading support
gcc -o thread_demo Class/06_Thread/<file>.c -lpthread
./thread_demo
```

### Inspect GCC Compilation Stages

```bash
# Pre-process only
gcc -E Compiler/ExploreCPU.c -o /tmp/out.i

# Compile to assembly
gcc -S Compiler/ExploreCPU.c -o /tmp/out.s

# Full compilation
gcc Compiler/ExploreCPU.c -o /tmp/ExploreCPU
```

---

## 🧰 Technology Stack

| Tool | Purpose |
|:--|:--|
| **GCC** | C compiler — all code examples |
| **GNU Make** | Build automation |
| **POSIX API** | `fork`, `exec`, `signal`, `pthread`, `mmap`, `shmget` |
| **strace / ltrace** | System call & library call tracing |
| **GDB** | Source-level debugger |
| **Valgrind** | Memory leak & error detection |

---

## 🗺️ Learning Roadmap

```
┌─────────────────────────────────────────────────────┐
│              Linux System Programming                │
│                                                     │
│  1. Compiler Internals  →  Understand toolchain     │
│  2. Library Creation    →  Static & Dynamic libs    │
│  3. Process Management  →  fork/exec/wait/signals   │
│  4. IPC                 →  Pipe/FIFO/MQ/SHM/Sem     │
│  5. Thread Management   →  POSIX threads/mutex      │
│  6. OS Deep Dive        →  70-day kernel internals  │
└─────────────────────────────────────────────────────┘
```

---

## 📖 Key Concepts Covered

<table>
<tr>
<td>

**Process Management**
- `fork()` & `exec()` family
- Process groups & sessions
- `wait()` / `waitpid()`
- Zombie & orphan processes

</td>
<td>

**IPC Mechanisms**
- Anonymous & Named Pipes
- POSIX Message Queues
- Shared Memory (`shmget`)
- Semaphores (`sem_open`)

</td>
<td>

**Thread Programming**
- `pthread_create()` / `join()`
- Mutex (`pthread_mutex_t`)
- Condition variables
- Thread-safe programming

</td>
</tr>
<tr>
<td>

**Signal Handling**
- `signal()` vs `sigaction()`
- Signal masks (`sigprocmask`)
- Real-time signals
- `sa_flags` & `sa_mask`

</td>
<td>

**Memory Management**
- Virtual memory & paging
- `mmap()` / `munmap()`
- Stack vs heap internals
- `malloc` internals (`brk`/`sbrk`)

</td>
<td>

**Kernel Internals**
- `task_struct` (PCB)
- Kernel modules (`.ko`)
- System call mechanics
- Device drivers (char driver)

</td>
</tr>
</table>

---

## 🤝 Contributing

Contributions, issues and feature requests are welcome!

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/topic-name`)
3. Commit your changes (`git commit -m 'Add day-XX notes'`)
4. Push to the branch (`git push origin feature/topic-name`)
5. Open a Pull Request

---

<div align="center">

<sub style="color: #666;">
Built with ❤️ for Linux System Programming enthusiasts &nbsp;|&nbsp;
<b style="color: #20B2AA;">nilprajapati97</b>
</sub>

</div>
