<h1 align="center">Thonangi Vamsikrishna Yadav</h1>
<h3 align="center">MS Researcher · Mechanistic Interpretability · IIT Bombay</h3>

<p align="center">
  <a href="https://github.com/vamsithonangi"><img src="https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github&logoColor=white"/></a>
  <img src="https://img.shields.io/badge/IIT%20Bombay-003087?style=flat-square"/>
  <img src="https://img.shields.io/badge/IISER%20Bhopal-8B0000?style=flat-square"/>
</p>

---

## About

I'm an MS/research student at **IIT Bombay** (ISRDC Lab), advised by **Prof. Virendra Singh**, working at the intersection of **mechanistic interpretability** and **transformer model analysis**. My research asks: *what are neural networks actually doing internally, and can we use that knowledge to prune, steer, and understand them?*

I'm also associated with **IISER Bhopal** in multiple campus roles.

---

## Research Focus

**Mechanistic Interpretability of Large Language Models**

I work on understanding transformer internals — particularly attention heads — through both theoretical frameworks and empirical experimentation. My current focus is on using optimizer statistics as cheap proxies for head importance.

- 🔬 **HeadRecycle (R&D2):** Validating that Adam's `exp_avg_sq` (a diagonal Fisher proxy — the *"Squisher"*) reliably detects inactive attention heads without a calibration phase. Running ablation studies across **GPT-2 Small/Medium, Pythia, Qwen, and LLaMA** on IIT Bombay's HPC cluster (OpenWebText + WikiText-103).
- 📐 **Baseline hierarchy:** weight magnitude (zero-cost) → Michel et al. 2019 (first-order) → Kwon et al. 2022 (diagonal Fisher) — showing the Squisher matches second-order methods at near-zero cost.
- 🧩 **R&D1:** Studied information over-squashing and representational collapse in decoder-only transformers. Trained models on binary digit counting tasks; found depth strongly influences counting ability, and learned positional embeddings form smooth ribbon-like diagonal patterns convergent across architectures.

---

## Current Projects

| Project | Status | Description |
|---|---|---|
| **HeadRecycle P1.6** | 🟡 Active | OWT ablation studies across 5 model families; LLaMA DGX runs pending |
| **Squisher vs. Kwon** | 🔬 Analysis | Comparing diagonal Fisher proxies: empirical vs. standard |
| **CS899 Seminar** | ✅ Done | 5-min talk on mech. interp.: Elhage 2021 → Lindsey 2025 (CLTs, SAEs, Claude biology) |
| **CS728 PA3** | ✅ Done | Retrieval heads, BM25, LLM-based retrieval; best Recall@1 = 0.3494 |

---

## Skills & Stack

**Research**
`Mechanistic Interpretability` `Attention Head Pruning` `Fisher Information` `Transformer Internals` `Ablation Studies`

**ML / Deep Learning**
`PyTorch` `Transformers (HuggingFace)` `GPT-2` `LLaMA` `Pythia` `Qwen`

**Infrastructure**
`SLURM` `HPC Clusters` `CUDA` `conda` `A40 / DGX GPUs`

**Languages & Tools**
`Python` `Bash` `Git` `LaTeX`

---

## Selected Findings

- `geometric_raw_balanced` tops AUC on **OpenWebText** while `combined_raw_balanced` leads on **WikiText** — suggesting scoring method sensitivity to dataset distribution, a potential dataset-generalization argument for the Squisher.
- Positional embeddings in counting-task transformers form **smooth ribbon-like diagonal patterns** that converge across architectures — consistent with over-squashing theory (Barbero et al., NeurIPS 2024).
- Tokenization is **not** the bottleneck for transformer counting failures; depth is.

---

## Reading List / Influences

Elhage et al. 2021 · Michel et al. 2019 · Kwon et al. 2022 · Barbero et al. NeurIPS 2024 · Lindsey et al. 2025 · SAE / Transcoder literature · CLT (Cross-Layer Transcoders)

---

<p align="center"><i>"Opening the black box, one attention head at a time."</i></p>
