<div align="center">

# 🧬 GW HuAI Lab

### Where rigorous statistics meets AI — to make clinical trials *faster, smarter, and more reliable.*

<p align="center">
  <a href="https://sites.google.com/gwmail.gwu.edu/gwhugroup/"><img src="https://img.shields.io/badge/Group_Website-GW_Hu_Group-002147?style=for-the-badge" alt="Group Website"></a>
  <img src="https://img.shields.io/badge/The_George_Washington_University-002147?style=for-the-badge" alt="The George Washington University">
  <img src="https://img.shields.io/badge/Focus-AI_%C3%97_Clinical_Trials-A89968?style=for-the-badge" alt="Focus: AI x Clinical Trials">
</p>

</div>

---

Welcome! We are the research group of **Prof. Feifang Hu** at **The George Washington University**.

We work on two sides of the same problem. On one side, we develop the **statistical foundations of modern clinical trials** — the theory of adaptive randomization and the inference that makes its results trustworthy. On the other, we put those foundations to work by building **AI systems that accelerate clinical-trial development**, from evidence synthesis to data reconstruction to trial design.

The thread that connects everything we do: better trials, reached faster, without giving up statistical rigor.

---

## 🎯 What we do

- **Methodology** — adaptive and covariate-adaptive randomization, causal inference, and valid statistical inference for the designs actually used in practice.
- **AI for clinical trials** — multi-agent systems and machine-learning tools that automate the slow, manual parts of clinical research while keeping a human in the loop where it matters.
- **Translation** — turning both into open, reproducible artifacts that practitioners and methodologists can build on.

---

## 📄 Featured publication

> ### Leveraging AI to Evaluate Minimal Residual Disease Endpoint Surrogacy in Multiple Myeloma
>
> Zexin Ren, Zixuan Zhao, Andrew J. Cowan, Will Ma, En Xie, Qian Shi
> *Cancer Research Communications* (2026) **6(5): 1206–1212**
>
> [![DOI](https://img.shields.io/badge/DOI-10.1158%2F2767--9764.CRC--25--0393-b31b1b?style=flat-square)](https://doi.org/10.1158/2767-9764.CRC-25-0393)

Minimal residual disease (MRD) has been backed by the FDA's Oncology Drugs Advisory Committee as an endpoint for accelerated approval in multiple myeloma — but the evidence base behind that decision predates a wave of recent trials. We introduce an **AI-assisted framework that automatically finds the relevant studies and extracts the numbers they report**, then re-runs the surrogacy analysis on an up-to-date evidence set. The result confirms a **moderate trial-level** and a **strong patient-level** association between MRD-negativity at complete response and survival outcomes.

---

## 🚀 What we're building

### 🔍 PUREvidence — systematic reviews, on autopilot (with a human-in-the-loop)

Systematic literature reviews are the backbone of clinical evidence. **PUREvidence** is a multi-agent system that automates the two most labor-intensive steps, **screening** and **data extraction**, while routing only the genuinely ambiguous cases to a human reviewer. It also turns a one-time review into a *living* one: freeze the eligibility query, re-run it against an up-to-date trial registry, and recover the original evidence plus whatever is new.

- A panel of **heterogeneous screening agents** debates each trial, with an inspector agent driving rounds of self-revision until they converge.
- **Specialized extraction agents** (treatment, subgroup, endpoint) re-read each source to self-correct, and tag every value with a confidence label.
- **Validated at scale** — on a ~2,200-trial NSCLC screening benchmark the agentic pipeline lifts a conservative single model from 0.58 to **0.93 sensitivity** while holding precision near 0.99; extraction reaches **~97% accuracy** with human review of flagged cells.

> 📝 *Manuscript:* "Systematic Literature Review with Two Multi-Agentic Systems and Human-in-the-Loop" — Ren, Zhao, et al. *(in preparation)*

### 🧪 SynthIPD — patient-level data, reconstructed from a published curve

Most statistical analysis needs **individual patient data (IPD)** — but IPD is usually locked away by privacy, ownership, and cost. **SynthIPD** reconstructs realistic patient-level data from *published results alone*. No access to the original IPD, and — unlike GAN/VAE/diffusion approaches — **no training data required at all.**

- Reads a published **Kaplan–Meier curve as vector graphics (SVG)** to recover event and censoring times with high precision.
- Generates **matching covariates** (age group, sex, biomarker status, ...) by constrained optimization, so the synthetic data supports *covariate-adjusted* analyses — something prior reconstruction methods couldn't do.
- Useful for **synthetic control arms**, sample-size planning, and strengthening pooled and subgroup meta-analyses.

> 📝 *Manuscript:* "SynthIPD: Training-free Synthetic Individual Patient Data Generation" — Zhao, Ren, Zhai, Hu, Ma, Xie, Shi — **major revision at *JASA***

---

## 🔬 Research themes

Beyond the AI tooling above, the group maintains a deep methodology portfolio:

- **Covariate-adaptive randomization** — design, discretization, and the effect of unobserved covariates
- **Causal inference & treatment-effect estimation** under adaptive designs
- **A/B testing under network interference** and spillover effects
- **Personalized medicine** and response-adaptive trial design
- **Valid inference for multi-arm trials** (GLMs, mixed-effects models, rerandomization vs. adaptive randomization)

📚 A fuller list lives on our [Research & Publications page](https://sites.google.com/gwmail.gwu.edu/gwhugroup/research-and-publications).

---

## 👥 People

Led by **Prof. Feifang Hu**, the lab brings together PhD students and collaborators across statistics, machine learning, and oncology, working alongside partners in academia and industry.

🎓 Meet the team on our [People page](https://sites.google.com/gwmail.gwu.edu/gwhugroup/people).

---

## 🔗 Connect

- 🌐 **Website:** https://sites.google.com/gwmail.gwu.edu/gwhugroup/
- 📧 **Prof. Feifang Hu:** feifang@gwu.edu
- 🏛️ Department of Statistics, The George Washington University · Washington, DC

<div align="center">

---

*Building the statistics — and the AI — behind better clinical trials.*

</div>
