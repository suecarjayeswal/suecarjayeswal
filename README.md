<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/suecarjayeswal/suecarjayeswal/main/assets/banner-dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/suecarjayeswal/suecarjayeswal/main/assets/banner-light.svg">
  <img alt="Swikar Jaiswal -- network flows over time" src="https://raw.githubusercontent.com/suecarjayeswal/suecarjayeswal/main/assets/banner-light.svg">
</picture>

I started by building things with my hands. Modifying an Android APK in Android Studio so it would log raw WiFi telemetry across campus, synchronized with multi-satellite GPS geotags. Writing a native desktop puzzle game in C++ where the stubborn challenge was coding believable gravity for tubes dropping into columns alongside a custom undo/redo state stack. Spending nine months rebuilding an automated execution engine in Rust from scratch to learn what sub-millisecond throughput demands from OS scheduling, lock-free ring buffers, and CPU cache-line alignment. Designing Bayesian MCMC samplers over heavy-tailed market volume distributions, and evolving non-standard trading indicator parameters via genetic algorithms across an 11-year backtest.

Somewhere after second year, I began looking underneath the code at the mathematical machinery governing what I had been writing. I started producing expositions--pulling theorems, discrete geometries, and algebraic structures apart until I could **modify** the machinery rather than merely cite it. Reading widely mattered immensely here: economics, philosophy, design, physics, and ecology each gave a concrete, spatial intuition to how I read a proof.

The computational foundation never left. Being able to think in both abstract mathematics and bare-metal systems is what moves me, and it is why I can sprint at a problem for a year without losing momentum.

Today, my core focus is **Artificial Reasoning and Mathematical Modeling**--whether in trade algorithms, artificial creativity, non-equilibrium economic systems, or autonomous topological memory architectures. I have yet to meet a problem I could not make deeply interesting by looking at it long enough.

**[Multi-facility allocation in network flow models: a case study](https://doi.org/10.70530/kuset.v20i1.721)** · *KUSET* 20(1), 2026 · two further articles under review · writing at **[swikarjaiswal.com.np](https://swikarjaiswal.com.np)**

---

### How the work connects

<div align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/suecarjayeswal/suecarjayeswal/main/assets/trajectory_growth_arc_dark.svg">
    <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/suecarjayeswal/suecarjayeswal/main/assets/trajectory_growth_arc_light.svg">
    <img alt="Swikar Jaiswal -- Intellectual Trajectory &amp; Research Growth Arc" src="https://raw.githubusercontent.com/suecarjayeswal/suecarjayeswal/main/assets/trajectory_growth_arc_dark.svg" width="100%">
  </picture>
</div>

---

### One result, plotted

Traced from the central Kathmandu evacuation network ($25$ nodes, $115$ arcs, $540$ evacuees), the Pareto curve below illustrates how clearance time $T^*$ responds to reversal budget $B$.

<img alt="Budget versus clearance time Pareto frontier, central Kathmandu case study" src="https://raw.githubusercontent.com/suecarjayeswal/suecarjayeswal/main/assets/bqtc_frontier.png" width="100%">

The curve is steep initially and flattens progressively: early budget investments buy sharp evacuation reductions, while subsequent increments yield diminishing returns. Evacuation planning sits at the intersection of operations research and planner judgment--for instance, reaching $T^* = 23$ is available at budget $859$, but saving another time interval to reach $T^* = 22$ demands budget $1190$ ($+38.5\%$ budget for a single time step). The Pareto frontier makes these operational tradeoffs legible.

---

### Selected Systems, Algorithms & Experiments

| Project | Domain / Stack | What was built & discovered |
|---|---|---|
| **[margadarshan](https://github.com/suecarjayeswal/margadarshan)** | `Python` `NetworkX` `Gemma 4` `Ollama` | **Offline road disruption intelligence.** Parses unstructured Nepali police bulletins locally via Gemma 4 (31B) into structured incident JSON. Computes multi-factor edge confidence ($C = \text{Source} \times \text{Corroboration} \times \text{Decay}$) and applies inverse confidence routing penalties. Validated via exact McNemar test ($p = 0.0078$). |
| **[automated-trading-system](https://github.com/suecarjayeswal)** | `Rust` `Lock-Free Ring Buffers` `Async` | **Sub-millisecond execution engine.** 9-month ground-up rebuild. Implements lock-free SPSC order queues, cache-line-aligned hot data structures, and deterministic zero-allocation execution paths to eliminate GC pauses and minimize OS scheduling latency. |
| **[slime-mould-sar](https://github.com/suecarjayeswal)** | `Python` `ESA SNAP GPF` `snappy` `QGIS` | **Bio-inspired disaster routing on satellite telemetry.** Dynamic flood evacuation modeling combining *Physarum polycephalum* adaptive foraging heuristics with an automated ESA Sentinel-1 SAR pipeline (radiometric calibration, terrain correction, Otsu thresholding). Inundation is synced with terrain and transport networks while the slime dynamically adjusts to progressive road closures, providing time-profiles for logistics that evacuate all zones within available clearance windows. |
| **[mcmc-anomaly-detection](https://github.com/suecarjayeswal)** | `Python` `PyMC` `ArviZ` | **Bayesian volume anomaly detection.** Log-normal likelihood model ($V \sim \text{Lognormal}(\mu, \sigma)$) sampled with No-U-Turn Sampler (NUTS) across 4 chains (2,000 draws). Verified convergence with $\hat{R} = 1.00$, $\text{ESS}_\text{bulk} > 7{,}900$, isolating statistically grounded institutional block trades. |
| **[ga-technical-indicators](https://github.com/suecarjayeswal)** | `Python` `NumPy` `LaTeX` | **Meta-heuristic parameter optimization.** Genetic Algorithm optimizing discrete parameter spaces on 11-year NEPSE data (2,522 sessions). Converged to non-standard MACD $(41, 83, 6)$ vs. textbook $(12, 26, 9)$, yielding **+44.1% net profit** while halving execution friction. |
| **[portfolio-risk-graph](https://github.com/suecarjayeswal)** | `Python` `NetworkX` `Dash` `Plotly` | **Topological market geometry.** Maps 130 securities using Mantegna ultrametric distance $d_{ij} = \sqrt{2(1-\rho_{ij})}$. Filters 8,385 correlations down to 129 MST edges; identifies systemic risk nodes and optimal diversification complements via Minimum Weighted Vertex Covers. |
| **[silent-witness](https://github.com/suecarjayeswal/2024-ecothon-ecoequation)** | `Python` `Graph Theory` `YOLO` | **Graph-based behavioral anomaly detection.** Layers spatial interaction graphs over multi-agent object detections to track recurring abusive patterns rather than individual identities. *Special Prize, BioHackathon 2024.* |
| **[filtermyfeed](https://github.com/suecarjayeswal/FiltermyFeed)** | `Python` `distilBERT` `Chrome Extension` | **Context-aware content filtering.** Collaborative project with seniors Mukesh Tiwari ([@mukeshdroid](https://github.com/mukeshdroid)), Bishesh Kafle ([@bses-codes](https://github.com/bses-codes)), and Aayam Basyal. Self-trained NLP classifier distinguishing figurative language from actual threats (*"your eyes kill me"* vs. real harassment). *Hackest 2023.* |
| **[tube-puzzle](https://github.com/suecarjayeswal/Tube_Puzzle)** | `C++` `wxWidgets` `DSA` | **Native desktop puzzle game.** Custom gravity physics simulation for falling tube fluids into discrete columns, featuring a memory-efficient stack-based undo/redo state machine. |
| **[wifi-signal-heatmap](https://github.com/suecarjayeswal)** | `Android Studio` `Python` `Folium` | **Spatial RF telemetry & multi-satellite geotagging.** Modified an Android APK to log raw WiFi RSSI metrics synchronized with multi-constellation satellite GPS, interpolating campus-wide spatial RF heatmaps in Leaflet.js. |

<details>
<summary><b>View first-principles coursework & mathematical implementations</b></summary>

<br/>

- **MATH 402 Cryptography & Quantum Protocols:** AES-128 from scratch with finite field $\text{GF}(2^8)$ multiplication; Weierstrass Elliptic Curve group law visualizer; full Quantum Key Distribution (BB84 protocol) simulation with Bloch sphere state vectors and eavesdropper QBER detection.
- **Operating Systems Architecture:** Multi-policy CPU scheduler (FCFS, SJF, SRTF, Priority, Round Robin) with Gantt telemetry; virtual memory page replacement simulator demonstrating Belady's Anomaly.
- **Galois Field $\text{GF}(2)$ CRC & Error Injection:** Polynomial division bit-level simulator benchmarking syndrome detection rates across multi-bit burst corruption models.
- **Bare-Metal C Systems:** Custom Binary Search Tree pointer benchmarks against CPU clocks; Gaussian elimination linear system solvers from scratch.

</details>

---

### Expositions & How I Think

I write expositions to deconstruct complex machinery until the geometry becomes intuitive:

- **[The Recourse Hyperplane in Submodularity](https://swikarjaiswal.com.np/explorations/submodularity-geometry):** Why submodularity ($f(A \cup B) + f(A \cap B) \le f(A) + f(B)$) is not merely a discrete set inequality, but a question of vector cone projections against the active constraint manifold of dual linear programs.
- **[When Physical Reality Breaks Flow Models](https://swikarjaiswal.com.np/explorations/asan-network-flow):** Simulating how vehicle bans in Kathmandu's historic Asan market cause localized queue collapses, and why dynamic contraflow (BQTC) requires algorithmic lane reversals under tight budgets.
- **[Hallucination as Key to Creativity](https://swikarjaiswal.com.np/explorations/hallucination-creativity):** Viewing creativity as rapid, low-amplitude search across high-dimensional associative spaces--where the bottleneck is not generative capacity, but sharp, topological evaluators and bounded recall criteria.
- **[Dirichlet Bounds in Continued Fraction Compression](https://swikarjaiswal.com.np/explorations):** Probing the information border between rational approximations and data compression limits.

#### Core Research & Engineering Tenets

1. **Find the structural fault first, then rebuild from it.** (I lost weeks of my thesis puzzling over seemingly conflicting dynamic flow representations $[\Gamma]$ vs $[\Gamma]^T$ in the literature, mistaking notation choices for errors. Only after failing an empirical random test case did I realize the underlying theoretical mechanisms operate in a definite amalgam under the right structural conditions. Unlocking that harmony was the breakthrough for the polynomial tractability proof).
2. **Construct the smallest instance that could break the conjecture.** Build the counterexample in code before proving the general case.
3. **Report the baseline beside the result.** State clearly where the model breaks down, where assumptions fail, and what the data cannot cover.

---

<div align="center">
  <sub>Kathmandu University · B.Sc. Computational Mathematics (Graduated 2026)</sub>
  <br/>
  <sub>
    <a href="https://swikarjaiswal.com.np">Portfolio</a> &nbsp;•&nbsp;
    <a href="https://github.com/suecarjayeswal">GitHub</a> &nbsp;•&nbsp;
    <a href="https://www.linkedin.com/in/swikarjaiswal">LinkedIn</a> &nbsp;•&nbsp;
    <a href="mailto:swikarjaiswal@gmail.com">Email</a>
  </sub>
</div>
