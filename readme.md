## 🚀 Highlights

- **PianoGym CPOMDP environment**  
  Models bimanual piano rhythm training as a **post-action, fatigue-constrained POMDP** with music-specific observables and multi-skill latent states.

- **Structured practice action library**  
  Uses a finite set of **tagged practice actions** (difficulty, skill targets, transfer, time cost, fatigue load) plus an explicit **REST** action.

- **Dual-timescale safety layer**  
  Combines **Lagrangian average-fatigue control** with a **short-horizon predictive guard** to keep both long-run and instant fatigue within limits.

- **PianoMPC controller**  
  A **finite-horizon model predictive controller** that plans over **guard-filtered safe actions** and outperforms bandit and value-based baselines in time to mastery.

---

## 📌 Repository Status

> **Important:**  
> This repository is currently a **placeholder** for the paper submission.  
> - Full source code will be **released after the paper is accepted and officially published**.  
> - The directory layout and this README will reflect the final structure for reproducibility.

Planned release items:
- [x] Environment and method description  
- [x] Figures for interaction protocol, safety, and MPC planning  
- [ ] PianoGym environment implementation  
- [ ] PianoMPC controller implementation  
- [ ] Baseline agents (bandits & RL)  
- [ ] Experiment scripts and evaluation pipeline  
- [ ] Pretrained configurations / example setups  

## 🧠 Method Overview

### 1. Post-Action PianoGym CPOMDP

[Post-action interaction protocol](figures/Post-action%20interaction%20protocol.pdf)

### 2. Dual-Timescale Fatigue Safety

[Dual-timescale safety layer](figures/Dual-timescale%20safety%20layer.pdf)

### 3. PianoMPC Planning over Safe Action Sets

[Model predictive control with receding horizon](figures/Model%20predictive%20control%20with%20receding%20horizon.pdf)
