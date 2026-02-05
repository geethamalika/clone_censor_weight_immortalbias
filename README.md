# Clone-censor-weight

**[Geetha Malika](https://github.com/geethamalika)** · Observational survival analysis · Immortal time bias

---

Clone–censor–weight (CCW) for addressing immortal time bias in studies where treatment starts at different times. This project uses **simulated data** (no external dataset): time zero = diagnosis, treatment can start in 0–12 months or never, outcome = time to death; true effect is null. The notebook shows how a naive analysis (clock starts at treatment for the treated group) produces a spurious survival benefit, and how CCW (same time zero, clone by strategy, censor at deviation, IPCW) recovers the null.

**Good for portfolio:** Demonstrates understanding of time-related bias and a principled fix with Python (pandas, lifelines, simulated cohort).

- **Dataset:** Simulated in the notebook via `simulate_cohort()` — no CSV files or paths.
- **Run:** Open `CCW_Immortal_Time_Bias.ipynb`, run all cells.
- **Requirements:** numpy, pandas, matplotlib, seaborn, lifelines (`requirements.txt`).

---

**Push to your GitHub:** From the project folder run `git init`, then create a new repo named `Clone-censor-weight` on [GitHub](https://github.com/new), add it as `origin`, and push.
