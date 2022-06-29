## Steps for Hypothesis Testing
<img width="565" alt="Steps for testing" src="https://user-images.githubusercontent.com/105242871/176347577-7be5013e-22f7-435f-8a1f-650519c1e81b.png">

***

## Probability Distrubition
<img width="735" alt="Working with Distribution" src="https://user-images.githubusercontent.com/105242871/176350329-bca4af9f-502a-48be-85a0-3fb65b08a558.png">

#### Uniform
<img width="829" alt="Uniform distribution" src="https://user-images.githubusercontent.com/105242871/176348568-59a3afb7-6270-4346-b4c4-c37b7a1e6ff6.png">

What type of statistical distribution allows us to model events where the outcome is discrete, and each outcome has an equally likely chance of occurring.
For example, the probability that you flip heads or tails on a fair coin.

#### Normal Distribution
This distribution allows us to model a continuous random variable where the further away from the mean you are, the less likely the outcome.
It is defined by a mean and a standard deviation. It is symmetric in shape, and the mean, median, and mode are equal.


#### Binomial Distribution
This distribution allows us to model the number of successes after a fixed number of trials, given a certain probability of success.
This distribution assumes that each trial is independent. (Discrete, fixed # of events.)
For example, the probability of throwing a 1 five times out of thirty-five tries.


#### Poisson Distribution
This distribution allows us to model a situation where a certain number of events happen over a specified time interval.
It is used to predict the amount of variation from a known average rate of occurrence within a given time frame.
There is not a fixed number of events, so there is no ceiling on the number of events we can have.

***

## Hypothesis Testing Errors
<img width="910" alt="type1and2error" src="https://user-images.githubusercontent.com/105242871/176348841-bcbe2daa-2108-4374-b5ed-ba369eccaf1b.png">

#### TYPE I (False Positive) - a false alarm
A type I error is when we reject the null hypothesis, but, in reality, the null hypothesis is true.

When doing hypothesis testing, what type of error do we make if we reject our Null Hypothesis when in reality it is True?
(For example, our test indicates there is a relationship in the population, but in reality there is no relationship.)


#### TYPE II (False Negative) - a miss
A type II error is when we fail to reject the null hypothesis when it is actually false.

When doing hypothesis testing, what type of error do we make if we fail to reject our Null Hypothesis when in reality it is not True and should have been rejected?
(For example, our test indicates there is not a relationship in the population, but in reality there IS a relationship.)

***

## Choosing Tests
<img width="397" alt="Statistical Tests" src="https://user-images.githubusercontent.com/105242871/176350393-9c235ec5-bc79-4e03-8b9d-713ac119e182.png">

## T-Test
#### Common assumptions we make when performing a t-test:
- Random Sample: data collected from representative, randomly selected portion of the total population.
- Independence of the observations: Each subject should belong to only one group. There is no relationship between the observations in each group.
- Normality: normal distribution of data. Little skewness and no outliers.
- Equality of Variance: similarity of variance throughout data. Standard deviations of sample are approximately equal.
- Sample Size: adequate sample size.

#### One-tailed
`scipy.stats.ttest_1samp`
<img width="763" alt="one tailed t-test" src="https://user-images.githubusercontent.com/105242871/176348641-93c92bba-25a7-41be-ab6d-dc53bb0378d9.png">

#### Two-tailed
`stats.ttest_ind`
<img width="809" alt="two tailed t-test" src="https://user-images.githubusercontent.com/105242871/176348105-876bd794-4ccd-4584-aced-2fd958a52a88.png">

## ANOVA
`scipy.stats.f_oneway`

## Correlation
`stats.pearsonr`

## Chi Square
`stats.chi2`
