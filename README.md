# Clone-censor-weight

**[Geetha Malika](https://github.com/geethamalika)** · Observational survival analysis · Immortal time bias

---

When people start treatment at different times, a naive comparison (treated vs untreated, with follow-up starting at treatment for the treated) makes treatment look better than it is — partly because everyone who got treatment had to survive until treatment start. That’s immortal time bias. Clone–censor–weight (CCW) is one way to fix it: same time zero for everyone (e.g. diagnosis), clone people into “strategy” groups, censor when they don’t follow that strategy, then weight. This project uses simulated data (no real dataset): everyone has the same time zero (diagnosis), treatment can start anytime in the first 12 months or never, and the outcome is time to death. The true effect is null. The notebook shows the biased result from the naive approach and that CCW brings you back to no effect.

Data are simulated in the notebook (`simulate_cohort()`); no CSV or paths. Open `CCW_Immortal_Time_Bias.ipynb` and run all cells. Requirements: numpy, pandas, matplotlib, seaborn, lifelines (`requirements.txt`).
