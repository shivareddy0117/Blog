---
layout: "shiva"
title: "Testing the Salary Claim of a Hiring Company"
date: 2024-04-28 T15:36:57+05:30
categories: statistics hypothesis-testing


---

### 1st Question:
A hiring company claims it finds jobs for its candidates with an annual salary of at least \$260,000. To test the claim, you take a random sample of 100 individuals who used the hiring service and recorded their annual salary. Can we conclude at the 5 percent level of significance that the claim is true?

### Required:

- H0: µ = \$260,000 (The company's claim is true, and the average salary is at least \$260,000.)
- Ha: µ < \$260,000 (The company's claim is not true, and the average salary is less than \$260,000.)

Using the data contained in the tab "Annual Salaries", determine the following:

- Sample Mean
- Sample Standard Deviation
- Sample Size
- t-statistic
- p-value

Do you reject or not reject the null hypothesis at alpha = 0.05, given that the p-value is equal to alpha?
### Answer:
### Hypothesis Test with Python

To perform this hypothesis test, we would follow these statistical steps and use Python to calculate the necessary values.

Here is the Python code that performs the calculations:

{% highlight ruby %}

import numpy as np
from scipy import stats

# Placeholder for sample data - replace this with the actual salary data
sample_data = [260000] * 100  # Example data, replace with actual values
sample_mean = np.mean(sample_data)
sample_std = np.std(sample_data, ddof=1)
sample_size = len(sample_data)

# The hypothesized population mean
mu_0 = 260000

# Calculate the t-statistic
t_statistic = (sample_mean - mu_0) / (sample_std / np.sqrt(sample_size))

# Calculate the p-value for a one-tailed test
p_value = stats.t.cdf(t_statistic, df=(sample_size-1))

# Decide whether to reject the null hypothesis
alpha = 0.05
reject_null = p_value < alpha

(sample_mean, sample_std, sample_size, t_statistic, p_value, reject_null)

{% endhighlight %}
