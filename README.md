<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/suecarjayeswal/suecarjayeswal/main/assets/banner-dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/suecarjayeswal/suecarjayeswal/main/assets/banner-light.svg">
  <img alt="Swikar Jaiswal — network flows over time" src="https://raw.githubusercontent.com/suecarjayeswal/suecarjayeswal/main/assets/banner-light.svg">
</picture>

I take a problem apart into its actors, the relationships between them, and the processes
running through them, and then look for where the slack is. That habit kept me in network
flow theory for two years. Most of what is here came out of following it.

**[Multi-facility allocation in network flow models: a case study](https://doi.org/10.70530/kuset.v20i1.721)** ·
*KUSET* 20(1), 2026 · two further papers under review ·
writing at **[swikarjaiswal.com.np](https://swikarjaiswal.com.np)**

---

### How the work connects

Two roots, and nearly everything grows off one of them.

```mermaid
%%{init: {'theme':'base','themeVariables':{'primaryColor':'#FBECC4','primaryTextColor':'#1C2B3A','primaryBorderColor':'#B23A2E','lineColor':'#5C5546','secondaryColor':'#EFE9D8','tertiaryColor':'#FFFDF6','fontFamily':'Georgia, serif','fontSize':'14px'}}}%%
flowchart LR
  NF(["flows<br/>over time"])
  PI(["probabilistic<br/>inference"])

  NF --> CT["contraflow<br/>tractability"]
  NF --> FL["facility location<br/>in flow networks"]
  NF --> SM["adaptive networks<br/>slime mould"]

  PI --> MC["MCMC anomaly<br/>detection"]
  PI --> EV["evolutionary<br/>search"]
  PI --> CG["correlation<br/>geometry"]

  CT --> T1{{"where contraflow<br/>gets hard"}}
  FL --> T2{{"KUSET 2026"}}

  NF --> MG["margadarshan"]
  PI --> MG

  style NF fill:#FBECC4,stroke:#B23A2E,stroke-width:2px
  style PI fill:#FBECC4,stroke:#B23A2E,stroke-width:2px
  style T1 fill:#EFE9D8,stroke:#2554A6,stroke-width:2px
  style T2 fill:#EFE9D8,stroke:#2554A6,stroke-width:2px
  style MG fill:#FFFDF6,stroke:#B23A2E,stroke-width:2px
```

`margadarshan` is the one that needed both: claims about the world arrive unreliable and have
to be weighted before they can become edge weights.

---

### One result, plotted

Reversing an inbound lane adds outbound capacity, which is how you empty a city faster. It is
also expensive, so the real question is what a given budget is worth.

<img alt="budget versus clearance time frontier" src="https://raw.githubusercontent.com/suecarjayeswal/suecarjayeswal/main/assets/frontier.svg" width="100%">

The steep part is free money. The flat part is where operations research hands the problem
back to a human being.

---

### Repositories

| | what it is |
|---|---|
| **[margadarshan](https://github.com/suecarjayeswal/margadarshan)** | Routing around road disruptions. A locally-run language model pulls closures out of Nepali police bulletins; each claim is scored by source reliability, corroboration, and age, and those scores become edge weights. `Python` `NetworkX` `Ollama` |
| **[silent-witness](https://github.com/suecarjayeswal/2024-ecothon-ecoequation)** | Behavioural graphs layered over object detection, tracking recurring patterns rather than identities. Most Innovative Project, Watson Code Fest 2024. `Python` |
| **[filtermyfeed](https://github.com/suecarjayeswal/FiltermyFeed)** | Browser extension filtering triggering content with a self-trained classifier. The hard part was figurative language: *your eyes kill me* is not a threat. `Python` `distilBERT` |
| **[nepalensis](https://github.com/suecarjayeswal/nepalensis)** | Visualizing Nepal's entries in the BOLD biodiversity database. Runner-Up, Watson Crack the Code 2022. `CSS` `Python` |

---

### How I work

Find the structural fault first, then rebuild from it. In practice:

- Write the machinery out expositorily until I can **modify** it, not merely cite it.
- Construct the smallest instance that could break the conjecture, then actually build it.
- Keep the counterexamples. Most conjectures die; the survivors become theorems.
- Report the baseline beside the result, and say what the model does not cover.

I lost weeks of the thesis to confusing an incidence matrix with its transpose, because the
standard presentations treat the two interchangeably and the contraflow adaptation does not
permit that. It was the most useful mistake of the project.

---

<sub>Kathmandu University · Computational Mathematics · [swikarjaiswal.com.np](https://swikarjaiswal.com.np) · [LinkedIn](https://www.linkedin.com/in/swikarjaiswal)</sub>
