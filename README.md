# Probability Models Visualization
This repository contains Python code for simulating and visualizing various probability distributions and their properties, such as the Binomial, Poisson, and Bernoulli distributions, along with visual demonstrations of the Law of Large Numbers and the Central Limit Theorem. The primary goal of this code is to illustrate how these theoretical concepts manifest through random processes and their visual representation.

## Features:
- **Bernoulli Trials Visualization:** Simulates and visualizes the outcome of repeated Bernoulli trials (like coin flips), where each trial has two possible outcomes (heads or tails) with a given probability.
- **Multiple Repetitions:** Simulates several repetitions of Bernoulli trials to showcase how the outcomes vary across different trials.
- **Binomial Distribution:** Simulates a set number of trials (e.g., 20 tosses) and plots the distribution of the total number of heads, demonstrating the binomial probability mass function (PMF).
- **Poisson Distribution Approximation: **Visualizes the Poisson distribution and compares it with the Binomial distribution under certain conditions, showcasing the approximation of the Poisson distribution by the Binomial distribution as the number of trials increases.
- **Conditional Histogram for Selected Outcomes:** Creates histograms of the total number of heads from sequences where the number of heads exceeds a certain threshold, highlighting the impact of filtering based on specific conditions.
- **Simulation of Sum of Poisson Random Variables:** Simulates and visualizes the sum of two Poisson random variables and shows how the distribution of the sum approaches a normal distribution as the number of random variables increases (illustrating the Central Limit Theorem).

## Dependencies:
This code requires the following Python libraries:

- **numpy:** For numerical operations and random number generation.
- **matplotlib:** For creating various types of plots and visualizations.
- **scipy.stats:** For statistical functions such as the binomial and Poisson distributions.
- **seaborn:** For enhanced data visualization and setting plot styles.

To install the required dependencies, run:

```
pip install numpy matplotlib scipy seaborn
```
## Structure:
- **Coin Toss Simulations (Bernoulli Trials):**

  - The first set of plots demonstrates a simple Bernoulli process (coin toss) with a probability of heads set to 0.2. The first graph visualizes the outcome of 20 tosses, showing heads (1) and tails (0) across the trials.
  - The second graph simulates and visualizes the outcomes of 5 repetitions of 20 tosses, using different colors for each repetition to show the randomness of the process.
  - The third graph shows a histogram of the total number of heads after 20 tosses across 100 trials, approximating the Binomial distribution.
- **Poisson Distribution Simulation:**

  - In the Poisson distribution simulation section, random values of alpha are generated, and for each value, both Binomial and Poisson distributions are simulated and compared.
  - The corresponding histograms demonstrate the resemblance of the Binomial distribution to the Poisson distribution when certain parameters are set, validating the theory that the Poisson distribution is a limit of the Binomial distribution for large n and small p.
- **Conditional Histogram for Sequences with Minimum Heads:
**
  - This section simulates 100 sequences of 20 tosses, and only those sequences where the total number of heads is greater than or equal to a specified threshold (k) are selected for further analysis. A histogram is plotted to show the distribution of the total number of heads under this condition.
- **Sum of Poisson Random Variables:**

  - The code simulates the sum of two Poisson random variables, each with randomly chosen lambda values, and visualizes the resulting distribution. As the number of random variables increases, the sum of Poisson variables approaches a normal distribution, which is an illustration of the Central Limit Theorem.
## Key Concepts Illustrated:
- **Law of Large Numbers (LLN):**

  - The LLN states that as the number of trials increases, the average outcome of those trials will converge to the expected value. This is visually demonstrated in the simulations where the average number of heads (successes) gets closer to the theoretical value of np as the number of trials grows.
- **Central Limit Theorem (CLT):**

  - The CLT suggests that the sum (or average) of a large number of independent, identically distributed random variables will approximate a normal distribution, regardless of the original distribution of the variables. This is showcased in the simulation of the sum of Poisson random variables, where the resulting sum tends to a normal distribution as the number of variables increases.
## Conclusion:
This code effectively visualizes various probability distributions and concepts like Bernoulli trials, the Binomial and Poisson distributions, and key statistical theorems. Through graphical representations, it provides insights into the behavior of random processes, helping users understand the underlying statistical principles and how they manifest in real-world data simulations.
