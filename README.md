A/B Testing — Designing the Data-Generating Process

Objective

I used experimental and observational data to study treatment effects, selection bias, statistical significance, confidence intervals, and sample-size planning.

Methodology

Loaded the LaLonde NSW job training experiment with 445 people.

Calculated the experimental average treatment effect on 1978 earnings.

Created a simulated observational comparison group to illustrate selection bias.

Used a permutation test with 9,999 shuffles to test the treatment effect.

Used bootstrap resampling to construct a 95% BCa confidence interval.

Performed power analysis to study required sample sizes for different effect sizes.

Applied the same testing methods to the Cookie Cats A/B test with 90,189 players.

Wrote an n_needed() function to calculate the sample size required for a new experiment.

Key Findings

In the LaLonde experiment, trainees earned $1,794.34 more than the randomized control group. The permutation test gave a p-value of 0.0046, and the 95% bootstrap confidence interval was $575.18 to $3,262.37. In contrast, the simulated observational comparison produced an estimated ATE of about -$14,784.46, showing how selection bias can reverse the conclusion.

For Cookie Cats, Day-1 retention was about 0.59 percentage points higher for gate 30 than gate 40, with a permutation p-value of 0.0790. Based on the observed effect, a new experiment would require about 111,192 players per group to achieve 80% power.
