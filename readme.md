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

![Post-action interaction protocol](figures/Post-action interaction protocol.pdf)

> *Figure 1. Post-action interaction loop with music observables and dual fatigue signals in PianoGym.*

---

### 2. Dual-Timescale Fatigue Safety

![Dual-timescale safety](figures/Dual-timescale safety layer.pdf)

> *Figure 2. Slow Lagrangian average-fatigue control combined with a fast predictive guard over the action library.*

---

### 3. PianoMPC Planning over Safe Action Sets

![MPC planning](figures/Model predictive control with receding horizon.pdf)

> *Figure 3. PianoMPC receding-horizon planning using the deterministic model and guard-defined safe action sets.*
