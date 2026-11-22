# Practical 11 – Sunspot Data Analysis Using Gamma Distribution and MCMC

## Aim
To analyse monthly mean total sunspot numbers from January 1749 to November 2018 using Python. The practical includes data visualisation, Gamma distribution modelling, and parameter estimation using the Markov Chain Monte Carlo (MCMC) method.

## Dataset
The dataset used is **Monthly Mean Total Sunspot Number**, collected from the SILSO World Data Center.

- Time period: January 1749 to November 2018
- Total observations: 3,239
- Main variable: Monthly mean sunspot number

## Libraries Used
- Python
- Pandas
- NumPy
- Matplotlib
- SciPy
- Google Colab

## Practical Steps

### Step 1: Plot the Data Over the Years
A line graph was created to visualise monthly sunspot numbers from 1749 to 2018.

**Conclusion:** The graph shows that sunspot activity increases and decreases over time. These repeated variations represent the solar cycle.

### Step 2: Model the Phenomenon Using Gamma Distribution
The data was divided into cycles of 12 years, equivalent to 144 months. A Gamma distribution was fitted to positive sunspot observations using Maximum Likelihood Estimation.

**Fitted Gamma Parameters:**
- Shape parameter (a): 1.1743
- Scale parameter (b): 71.6402

**Conclusion:** The Gamma distribution provides a probability model for positive sunspot counts and helps describe their right-skewed distribution.

### Step 3: Histogram of Sunspot Counts
A histogram was plotted to understand the frequency distribution of monthly sunspot counts.

**Conclusion:** Most observations occur at lower or moderate values, while some months have much higher sunspot activity.

### Step 4: MCMC Using a = 4 and b = 10
The Metropolis-Hastings algorithm was used to generate samples for the Gamma distribution parameters.

Initial values:
- a = 4
- b = 10
- Total MCMC samples = 30,000

**Acceptance Rate:** 0.04697 (approximately 4.70%)

Three groups of samples were compared:
- First 50 samples
- All samples
- Last 50 samples

**Conclusion:** The three groups help compare how the Gamma distribution changes across MCMC samples and show how the parameter estimates evolve.

### Step 5: Trace Plots and Histograms
Trace plots were created for parameters `a` and `b`. The first 5,000 samples were removed as burn-in samples.

Histograms were then plotted using the remaining samples to understand the posterior distributions.

**Conclusion:** Trace plots show parameter changes across MCMC iterations, while histograms show the posterior distributions of the parameters. Removing burn-in samples reduces the influence of initial values.

### Step 6: Prediction of Parameters a and b
The posterior mean and 95% credible intervals were calculated after removing burn-in samples.

**Results:**

| Parameter | Estimated Mean | 95% Credible Interval |
|---|---:|---|
| a | 1.1733 | 1.1209 – 1.2238 |
| b | 71.7167 | 67.9308 – 75.6814 |

Twelve possible monthly sunspot values were also simulated using the estimated Gamma parameters.

**Conclusion:** The posterior mean values provide estimates of the Gamma parameters. The simulated values represent possible monthly sunspot counts under the fitted model.

## Overall Conclusion
In this practical, we analysed monthly sunspot data from 1749 to 2018 using Python. We visualised the data, fitted a Gamma distribution, and applied the Metropolis-Hastings MCMC algorithm to estimate the shape and scale parameters.

We also compared different groups of MCMC samples, removed burn-in samples, plotted trace graphs and histograms, and calculated posterior estimates with 95% credible intervals.

This practical helped us understand probability distributions, Bayesian parameter estimation, MCMC sampling, and data visualisation.

## Learning Outcomes
- Learned to load and analyse time-series data using Pandas.
- Understood sunspot activity and its cycles.
- Learned to fit a Gamma distribution.
- Understood the Metropolis-Hastings MCMC algorithm.
- Learned the importance of burn-in samples.
- Created trace plots and posterior histograms.
- Estimated parameters using posterior means and credible intervals.
