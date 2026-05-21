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

---

## Research Focus

**Mechanistic Interpretability of Large Language Models**

I work on understanding transformer internals — particularly attention heads — through both theoretical frameworks and empirical experimentation. My current focus is on using optimizer statistics as cheap proxies for head importance.

- 🔬 **HeadRecycle (R&D2):** Validating that Adam's `exp_avg_sq` (a diagonal Fisher proxy — the *"Squisher"*) reliably detects inactive attention heads without a calibration phase. Running ablation studies across **GPT-2 Small/Medium, Pythia, Qwen, and LLaMA** on IIT Bombay's HPC cluster (OpenWebText + WikiText-103).
- 📐 **Baseline hierarchy:** weight magnitude (zero-cost) → Michel et al. 2019 (first-order) → Kwon et al. 2022 (diagonal Fisher) — showing the Squisher matches second-order methods at near-zero cost.
- 🧩 **R&D1:** Studied information over-squashing and representational collapse in decoder-only transformers. Trained models on binary digit counting tasks; found depth strongly influences counting ability, and learned positional embeddings form smooth ribbon-like diagonal patterns convergent across architectures.



<p align="center"><i>"Opening the black box, one attention head at a time."</i></p>
