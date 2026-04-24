# Hi, I'm Pablo Soage

**Computer Engineer | Systems Architecture | Bare-Metal Problem Solver**

I am a Computer Engineering graduate focused on low-level architecture, systems programming, and high-performance computing. I enjoy bridging the gap between hardware and software, from reverse-engineering automotive ECUs and compiling C parsers, to managing bare-metal hyper-compute clusters and rebuilding internal combustion engines.

Currently shifting my focus towards **Embedded Systems, Electronic Warfare, Defense Tech**, and systems programming (`C/C++`, `Rust`).

## Hardware, Infrastructure & Code

My technical background extends beyond standard software development. I approach engineering as a continuous puzzle across multiple disciplines:

* **Systems Architecture & AI Infrastructure:** Designing and maintaining self-hosted homelab environments. I manage a custom bare-metal Gigabyte T181-G20 server (Dual Xeon Platinum, **4x Nvidia Tesla V100 SXM2 via NVLink**) deploying local LLMs (Open-WebUI, vLLM...) and a Docker swarm (Gitea, Minio...).
  * *Hardware Hacks:* Built a remote PSU trigger bridging `PS_ON` to `GND` using a Raspberry Pi GPIO and a MOSFET via Home Assistant. Modified the MegaRAC SP-X BMC JSON configurations to optimize fan curves for idle/load acoustics without thermal throttling.
* **Low-Level OS Troubleshooting:** Experienced in disaster recovery techniques. Examples include using `sethc.exe` backdoor exploitation for `NT AUTHORITY\SYSTEM` privilege escalation to rebuild a corrupted `WinSxS` directory, and writing a Windows Server 2025 script to hot-swap V100 drivers between TCC and WDDM modes without rebooting via direct registry modifications.
* **Automotive Mechanics & ECU Engineering:** Practical knowledge of engine mechanics (rebuilding engines, timing belt replacements, and resurrecting seized motors). Conceptual understanding of ECU calibration parameters (WinOLS, GDS2, SOI advanced timing, torque capping for gearbox protection), which led to the development of my [Denso-ECU-Toolkit](https://github.com/PabloSoage/Denso-ECU-Toolkit).
* **Hardware & Fabrication:** Hands-on experience with 3D printing (Resin/FDM), micro-soldering, PCB assembly, and drone piloting.

> ## 📜 Academic Excellence & Endorsements
> 
> Throughout my degree (**GPA: 8.7/10**), I have achieved a record of excellence, receiving **7 Honors (Matrículas de Honor)** in computer science and engineering subjects:
> 
> * **Core Systems & Logic:** Computer Structure, Programming Paradigms, and Language Processing (Flex/Bison).
> * **Data & Infrastructure:** Databases, Computer Networks, and Information Retrieval.
> * **Research & Development:** My Bachelor's Thesis (*Framework for Data Capture and Synchronization for Brain-Computer Interfaces*).
> 
> I have been endorsed by **5 University Professors and PhDs** for the **Vulcanus in Japan** international program. These recommendations, along with my official  transcript, highlight my technical rigor, ability to solve low-level architectural puzzles, and dedication to high-complexity projects.
> 
> 🔗 **[View Transcript & Recommendation Letters Here](https://udcgal-my.sharepoint.com/:f:/g/personal/p_soage_udc_es/IgDH3t-POAOITKRpsRSBUN9sAab7tpj4zQSfcMLHWMF9zMA?e=Iqe4yF)**

## Featured Engineering Projects

* **[C-Flex-Bison-HTML-Parser](https://github.com/PabloSoage/C-Flex-Bison-HTML-Parser):** A custom HTML DOM parser built from scratch. Uses Flex/Bison for lexical/syntactic analysis in C, compiled into a shared library, and bound to Python via FFI (`ctypes`). Valgrind-verified with zero memory leaks.
* **[Denso-ECU-Toolkit](https://github.com/PabloSoage/Denso-ECU-Toolkit):** A modular toolchain for extracting, mapping, and visualizing calibration parameters from Denso ECUs. Uses custom Ghidra (Jython) scripts for heuristic memory scanning.
* **[NeuroSync-Framework](https://github.com/PabloSoage/NeuroSync-Framework):** A synchronized pipeline for real-time EEG neurophysiological signal processing. Implements multiprocessing for isolated CPU-intensive tasks (FastICA) alongside a multi-interface architecture (GUI, CLI, FastAPI).
* **[ASP-Constraint-Solvers](https://github.com/PabloSoage/ASP-Constraint-Solvers):** Declarative logical models built with Answer Set Programming (`clingo` / `telingo`) to solve NP-Hard multi-agent spatio-temporal planning and graph topology problems.
* **[Fabric2D](https://github.com/PabloSoage/Fabric2D):** A procedural 2D engine built without commercial frameworks. Features multithreaded Jump Point Search (JPS) pathfinding, graph-based procedural generation, and native C/C++ FMOD audio library integration (in collaboration with [roiniti](https://github.com/roiniti) and [Mateo-RR](https://github.com/Mateo-RR)).

## Tech Stack & Tooling

* **Languages:** `C`, `Python`, `Julia`, `OCaml`, `SQL`, `Java`, `Bash/PowerShell` *(Currently expanding into `C++` & `Rust`)*.
* **Infrastructure:** Docker, Nginx, Wireguard, Prometheus, MinIO, Windows Server 2025, Ubuntu Server.
* **Engineering Tools:** Ghidra (Reverse Engineering), WinOLS/GDS2 (Automotive), Clingo/Telingo (Formal Logic), Flex/Bison.
* **Core Concepts:** Concurrency (Multiprocessing, Mutex/Locks), C-FFI, Bare-metal deployment, Asynchronous I/O.

## 🌲 Beyond Engineering

I tend to approach most challenges as logical puzzles, but I also know when to completely unplug:
* 🎻 **Music:** Violinist (9 years of professional conservatory training).
* 🇯🇵 **Languages & Culture:** Self-taught Japanese (memorized ~2,000 kanjis by visually deconstructing them into radical puzzles) and long-time anime enthusiast. Native Spanish/Galician, C1 English, basic German (A1), and currently exploring Russian.
* 🏹 **Focus:** Traditional archery, mechanical restoration, and spatial puzzles (e.g., Megaminx).
* 🌿 **Outdoors:** Hiking and exploring *fervenzas* (traditional Galician waterfalls) and the deep green natural landscapes of my homeland to disconnect from the grid.

> *"If a system has logic, it can be understood. If it can be understood, it can be optimized."* — **Personal Engineering Motto**<br>
> *"逃げたら一つ、進めば二つ" (If you run, you gain one; if you move forward, you gain two.)* — **Mobile Suit Gundam: The Witch from Mercury**<br>
> *"ちりも積もれば山となる" (Even dust, when piled up, becomes a mountain.)* — **Japanese Proverb**
