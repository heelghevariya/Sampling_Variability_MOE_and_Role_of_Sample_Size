📊 Sampling Variability and Margin of Error Analysis
Understanding How Sample Size Affects Uncertainty in Real-World Data
📌 Project Overview

In data analytics, decisions are often based on sample estimates rather than full populations. Understanding how sample size affects uncertainty is critical when interpreting survey results, A/B tests, healthcare metrics, or operational KPIs.

This project uses data from the RAND Health Insurance Experiment, originally conducted by the RAND Corporation, to investigate:

- How sample size affects the precision of a mean estimate

- How the margin of error shrinks as sample size increases

- How sampling variability appears even when sample size is fixed


🗂 Dataset:

The dataset contains 20,190 individuals enrolled in a large-scale health insurance experiment.

Each row represents one individual.

Key variable used in this project:

- mdvis — Number of outpatient doctor visits

We treat mdvis as a numeric outcome and estimate its population mean under different sampling scenarios.

🎯 Business Motivation: 

In real-world analytics work, we frequently ask:

- How reliable is our estimate?

- Is our sample size large enough?

- How much uncertainty surrounds our KPI?

- Would collecting more data meaningfully improve precision?

This project answers those questions using empirical simulation.

🔬 Methodology

The project consists of three components:

1️⃣ Effect of Sample Size on Confidence Intervals

Random samples of varying sizes were drawn:

n = 25, 50, 100, 250, 500, 1000

For each sample:

- Computing sample mean

- Computing standard error

- Construct 95% confidence interval

- Visualising CI width across sample sizes


2️⃣ Margin of Error vs Sample Size

The margin of error (MOE) was computed as:

MOE = upper CI bound − mean

	​

3️⃣ Sampling Variability at Fixed Sample Size

With a fixed sample size (n = 100):

- 40 independent samples were drawn

- Means and 95% confidence intervals were computed

- All intervals were plotted together.

This illustrates that:

- Even with fixed sample size, estimates vary

- Confidence intervals shift due to random sampling

- Estimates are probabilistic, not deterministic


This project highlights practical analytics competencies:

✔ Statistical reasoning beyond point estimates
✔ Interpretation of confidence intervals
✔ Understanding of uncertainty quantification
✔ Simulation-based validation
✔ Data visualization for communicating variability
✔ Translating statistical theory into business implications

🛠 Tools Used

- Python

- pandas

- NumPy

- statsmodels

- Matplotlib

- Jupyter Notebook