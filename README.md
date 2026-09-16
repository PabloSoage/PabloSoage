# Hi, I'm Pablo Soage

**Computer Engineer | Systems Architecture | Bare-Metal Problem Solver**

<p align="left">
  <img src="https://img.shields.io/badge/C-00599C?style=flat-square&logo=c&logoColor=white" alt="C">
  <img src="https://img.shields.io/badge/C++-00599C?style=flat-square&logo=cplusplus&logoColor=white" alt="C++">
  <img src="https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white" alt="Rust">
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" alt="Python">
  <img src="https://img.shields.io/badge/Kotlin-7F52FF?style=flat-square&logo=kotlin&logoColor=white" alt="Kotlin">
  <img src="https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white" alt="Java">
  <img src="https://img.shields.io/badge/Verilog-1A1A1A?style=flat-square" alt="Verilog">
  <img src="https://img.shields.io/badge/OCaml-EC6813?style=flat-square&logo=ocaml&logoColor=white" alt="OCaml">
  <img src="https://img.shields.io/badge/Julia-9558B2?style=flat-square&logo=julia&logoColor=white" alt="Julia">
</p>
<p align="left">
  <img src="https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black" alt="Linux">
  <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white" alt="Docker">
  <img src="https://img.shields.io/badge/Kubernetes-326CE5?style=flat-square&logo=kubernetes&logoColor=white" alt="Kubernetes">
  <img src="https://img.shields.io/badge/Kafka-231F20?style=flat-square&logo=apachekafka&logoColor=white" alt="Kafka">
  <img src="https://img.shields.io/badge/Spring%20Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white" alt="Spring Boot">
  <img src="https://img.shields.io/badge/AMD%20Xilinx-ED1C24?style=flat-square&logo=amd&logoColor=white" alt="AMD Xilinx">
  <img src="https://img.shields.io/badge/Ghidra-FF6B00?style=flat-square&logo=ghidra&logoColor=white" alt="Ghidra">
  <img src="https://img.shields.io/badge/KiCad-314CB0?style=flat-square&logo=kicad&logoColor=white" alt="KiCad">
  <img src="https://img.shields.io/badge/NVIDIA%20CUDA-76B900?style=flat-square&logo=nvidia&logoColor=white" alt="CUDA">
</p>

I am a Computer Engineering graduate focused on low-level architecture, systems programming, and high-performance computing. I enjoy bridging the gap between hardware and software, from reverse-engineering automotive ECUs and compiling C parsers, to managing bare-metal hyper-compute clusters and rebuilding internal combustion engines.

Currently working as a **Core Software Developer at Ágata Technology (Emetel Group)**, building smart multisystem integration platforms. Alongside my professional work, I am expanding my focus towards **Embedded Systems, Electronic Warfare, Defense Tech**, and high-performance systems programming (`C/C++`, `Rust`).

## Hardware, Infrastructure & Code

My technical background extends beyond standard software development. I approach engineering as a continuous puzzle across multiple disciplines:

* **Systems Architecture & AI Infrastructure:** Designing and maintaining self-hosted homelab environments. I manage a custom bare-metal Gigabyte T181-G20 server (Dual Xeon Platinum, **4x Nvidia Tesla V100 SXM2 via NVLink**) deploying local LLMs (Open-WebUI, vLLM...) and a Docker swarm (Gitea, Minio...). Alongside it, an **AMD Kria KV260 (K26 SOM, Zynq UltraScale+ ZU5EV)** as the FPGA/SDR bench. Both are driven from the terminal by tools I wrote for the purpose — [redfishctl](https://github.com/PabloSoage/redfishctl), a Rust TUI that controls and monitors the server's BMC over Redfish (sensors, charts, power, event log) without `ipmitool` or the BMC web interface.
  * *Hardware Hacks:* Built a remote PSU trigger bridging `PS_ON` to `GND` using a Raspberry Pi GPIO and a MOSFET via Home Assistant. Modified the MegaRAC SP-X BMC JSON configurations to optimize fan curves for idle/load acoustics without thermal throttling.
* **Low-Level OS Troubleshooting:** Experienced in disaster recovery techniques. Examples include using `sethc.exe` backdoor exploitation for `NT AUTHORITY\SYSTEM` privilege escalation to rebuild a corrupted `WinSxS` directory, and forcing Tesla V100s into **WDDM mode on Windows Server 2025**, which NVIDIA does not expose for these cards at all — `nvidia-smi` offers only TCC — by writing the display driver keys directly in the registry, and hot-swapping back without a reboot. That unlocked the GPUs for WSL2 and for graphical workloads (Blender, games) while compute tooling such as LM Studio still detects them under TCC.
* **Automotive Mechanics & ECU Engineering:** Practical knowledge of engine mechanics (rebuilding engines, timing belt replacements, and resurrecting seized motors). Working knowledge of ECU calibration parameters (WinOLS, GDS2, SOI advanced timing, torque capping for gearbox protection) and of the diagnostic layer beneath them — reverse-engineering an adapter's undocumented protocol down to its CRC, and reading a factory tool's own 89 MB vehicle database by decompiling the loader that reads it. This led to my [Denso-ECU-Toolkit](https://github.com/PabloSoage/Denso-ECU-Toolkit) and [opendash](https://github.com/PabloSoage/opendash).
* **Hardware & Fabrication:** Hands-on experience with 3D printing (Resin/FDM), micro-soldering, PCB assembly, and drone piloting.

> ## 📜 Academic Excellence & Endorsements
> 
> Throughout my degree (**GPA: 8.7/10**), I have achieved a record of excellence, receiving **7 Honors (Matrículas de Honor)** in computer science and engineering subjects:
> 
> * **Core Systems & Logic:** Computer Structure, Programming Paradigms, and Language Processing (Flex/Bison).
> * **Data & Infrastructure:** Databases, Computer Networks, and Information Retrieval.
> * **Research & Development:** My Bachelor's Thesis (*Framework for Data Capture and Synchronization for Brain-Computer Interfaces*).
> 
> I have been endorsed by **6 University Professors and PhDs**, five of them specifically for the **Vulcanus in Japan** international program. These recommendations, along with my official  transcript, highlight my technical rigor, ability to solve low-level architectural puzzles, and dedication to high-complexity projects.
> 
> 🔗 **[View Transcript & Recommendation Letters Here](https://udcgal-my.sharepoint.com/:f:/g/personal/p_soage_udc_es/IgDH3t-POAOITKRpsRSBUN9sAab7tpj4zQSfcMLHWMF9zMA?e=Iqe4yF)**

## Featured Engineering Projects

* **[scanner64](https://github.com/PabloSoage/scanner64):** A 64-channel real-time DDC bank in Verilog for the AMD Kria KV260's programmable logic: one sample per cycle, fixed latency, dropped samples impossible by construction. Verified in hardware and benchmarked bit-exact against C, CUDA and Xeon builds — **11x a Tesla V100 and 40x a dual Xeon per watt**.
* **[C-Flex-Bison-HTML-Parser](https://github.com/PabloSoage/C-Flex-Bison-HTML-Parser):** A custom HTML DOM parser built from scratch. Uses Flex/Bison for lexical/syntactic analysis in C, compiled into a shared library, and bound to Python via FFI (`ctypes`). Valgrind-verified with zero memory leaks.
* **[Denso-ECU-Toolkit](https://github.com/PabloSoage/Denso-ECU-Toolkit):** A modular toolchain for extracting, mapping, and visualizing calibration parameters from Denso ECUs. Uses custom Ghidra (Jython) scripts for heuristic memory scanning.
* **[NeuroSync-Framework](https://github.com/PabloSoage/NeuroSync-Framework):** A synchronized pipeline for real-time EEG neurophysiological signal processing. Implements multiprocessing for isolated CPU-intensive tasks (FastICA) alongside a multi-interface architecture (GUI, CLI, FastAPI).
* **[Rustify](https://github.com/PabloSoage/Rustify):** A high-performance Android music player combining a native **Rust core** with a Kotlin/Jetpack Compose frontend. Utilizes custom JNI bindings for dynamic GraphQL scraping, heuristic track matching, and zero-latency loopback HTTP stream proxying to Media3 ExoPlayer.
* **[opendash](https://github.com/PabloSoage/opendash):** An Android diagnostic app for the Scanmatik SM3, built on an undocumented Wi-Fi protocol recovered from packet captures and **confirmed against a live vehicle**. Identifying the frame signature as a CRC turned replaying captures into constructing messages — real CAN filters, live data at ~100 frames/s, and an ELM327 bridge so any existing OBD app can drive the device.
* **[OCaml-Lambda-Interpreter](https://github.com/PabloSoage/OCaml-Lambda-Interpreter):** An interpreter for a statically typed extended lambda calculus. `ocamllex`/`ocamlyacc` front end feeding a type checker with type aliases and **structural subtyping** over records and functions; recursion via a fixed-point combinator (`letrec`), algebraic structures (lists, tuples, records, tagged variants with `case-of`), and a REPL holding a persistent global context.
* **[ASP-Constraint-Solvers](https://github.com/PabloSoage/ASP-Constraint-Solvers):** Declarative logical models built with Answer Set Programming (`clingo` / `telingo`) to solve NP-Hard multi-agent spatio-temporal planning and graph topology problems.
* **[Fabric2D](https://github.com/PabloSoage/Fabric2D):** A procedural 2D engine built on `pygame` with no commercial framework underneath. Features multithreaded Jump Point Search (JPS) pathfinding, graph-based procedural generation, and the native FMOD audio engine driven through its Python bindings (in collaboration with [roiniti](https://github.com/roiniti) and [Mateo-RR](https://github.com/Mateo-RR)).

## Upstream Contributions

* **[codebase-memory-mcp#1764](https://github.com/DeusData/codebase-memory-mcp/issues/1764):** Diagnosed a regression where every idle MCP client burned around 0.7 of a CPU core from `0.9.1-rc.1` onward, multiplying by the number of concurrent sessions. Bisected against `0.9.0` as a control and reproduced by spawning the binary from a shell without sending a single JSON-RPC message. Fixed upstream in PR #1845; the maintainer's words on closing were that "the diagnosis in this thread did the hard part".
* **[nvidia-pstated#10](https://github.com/sasha0552/nvidia-pstated/pull/10):** A clock-based fallback for datacentre GPUs that expose only one performance state (P100, V100). Where setting a P-state fails, it reads each GPU's lowest supported core and memory clocks and idles there instead. +519/−18 across 4 files; open.

## Tech Stack & Tooling

* **Languages:** `C`, [`Rust`](https://github.com/PabloSoage/Rustify), [`Python`](https://github.com/PabloSoage/NeuroSync-Framework), `Julia`, `Java`, [`OCaml`](https://github.com/PabloSoage/OCaml-Lambda-Interpreter), `SQL`, `Kotlin`, `Clingo/Telingo`, `Bash/PowerShell` *(currently expanding into `C++` & [`Verilog/SystemVerilog`](https://github.com/PabloSoage/scanner64))*.
* **Systems & Low-Level:** Concurrency (threads, mutex/locks, multiprocessing), C-FFI and JNI, asynchronous and socket I/O, fixed-point DSP, binary formats and wire protocols, bare-metal deployment.
* **Reverse Engineering:** Ghidra, Wireshark and packet capture, CFR/JADX decompilation, CAN/ISO-TP and J2534 diagnostics, WinOLS/GDS2.
* **Hardware & FPGA:** Vivado/Vitis, XSim, KiCad, AMD Kria KV260 (Zynq UltraScale+), oscilloscope and logic analyser, micro-soldering.
* **Infrastructure:** Docker & Colima, Kubernetes, Nginx, Wireguard, Prometheus, MinIO, Redfish/BMC, Windows Server 2025, Ubuntu Server.
* **How I Work:** Git and GitHub Actions with CI gates; empirical debugging — measure first, change one thing at a time; and writing down what is *not* verified as carefully as what is.

## 🌲 Beyond Engineering

I tend to approach most challenges as logical puzzles, but I also know when to completely unplug:
* 🎻 **Music:** Violinist (9 years of professional conservatory training).
* 🇯🇵 **Languages & Culture:** Self-taught Japanese (memorized ~2,000 kanjis by visually deconstructing them into radical puzzles) and long-time anime enthusiast. Native Spanish/Galician, C1 English, basic German (A1), and currently exploring Russian.
* 🏹 **Focus:** Traditional archery, mechanical restoration, and spatial puzzles (e.g., Megaminx).
* 🌿 **Outdoors:** Hiking and exploring *fervenzas* (traditional Galician waterfalls) and the deep green natural landscapes of my homeland to disconnect from the grid.

> *"If a system has logic, it can be understood. If it can be understood, it can be optimized."* — **Personal Engineering Motto**<br>
> *"逃げたら一つ、進めば二つ" (If you run, you gain one; if you move forward, you gain two.)* — **Mobile Suit Gundam: The Witch from Mercury**<br>
> *"ちりも積もれば山となる" (Even dust, when piled up, becomes a mountain.)* — **Japanese Proverb**
