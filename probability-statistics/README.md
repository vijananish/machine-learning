# PROBABILITY AND STATISTICS

## INTRODUCTION

Probability And Statistics are the two important concepts in Maths. Probability is all about chance. Whereas statistics is more about how we handle various data using different techniques. It helps to represent complicated data in a very easy and understandable way.


## RANDOM VARIABLE

A random variable is a numerical description of the outcome of a statistical experiment. A random variable that may assume only a finite number or an infinite sequence of values is said to be discrete; one that may assume any value in some interval on the real number line is said to be continuous.
This is generally represented by 'X'.

Here we can think of and example: Rolling a Die, and Tossing a coin.

Rolling Dice:

X = {1, 2, 3, 4, 5, 6}

Therefore 

P(X=1) = 1/6

P(X=even) = 3/6

Also P(X=x1) = P(x1)

### Discrete Random Variable

A discrete random variable can take only a finite number of distinct values such as 0, 1, 2, 3, 4, … and so on. The probability distribution of a random variable has a list of probabilities compared with each of its possible values known as probability mass function.

Here we used ```Probablitity Mass Function (PMF)```

### Continuous Random Variable

A numerically valued variable is said to be continuous if, in any unit of measurement, whenever it can take on the values a and b. If the random variable X can assume an infinite and uncountable set of values, it is said to be a continuous random variable. When X takes any value in a given interval (a, b), it is said to be a continuous random variable in that interval.

Here we use ```Probablitity Density Function (PDF)```


## POPULATION

In statistics, population is the entire set of items from which you draw data for a statistical study. It can be a group of individuals, a set of items, etc. It makes up the data pool for a study.

There are different types of population. They are:
1. Finite Population
2. Infinite Population
3. Existent Population
4. Hypothetical Population


## SAMPLE

A sample represents the group of interest from the population, which you will use to represent the data. The sample is an unbiased subset of the population that best represents the whole data.
In this we take random variables.
When the sample size becomes large then the sample mean becomes equal to sample mean.
Basically, there are two types of sampling. They are:

### Probability sampling
1. Simple random sampling 
2. Cluster sampling 
3. Stratified Sampling 
4. Disproportionate sampling 
5. Proportionate sampling 
6. Optimum allocation 
7. Stratified sampling 
8. Multi-stage sampling

### Non-probability sampling
1. Quota sampling
2. Judgement sampling
3. Purposive sampling


## DISTRIBUTION USAGE

Probability ---> Data Analysis ---> Answering Question about Data


## CHEBYSHEV'S INEQUALITY

From the Gaussian Distribution one knows about 68-95-99 percent rule.
On the basis of Gaussian Distribution: ```P(nu-2sigma<x<nu+2sigma) = 95%```

What if we don't know the distribution but know the mean and standard deviation. Let x% data lies between nu-sigma and nu+sigma.
Here comes Chebyshev's Inequality comes into play.

According to Chebyshev's let X be random variable and mean be finite and standard deviation be finite and non-zero. We don't know the distribution then

![alt text](https://www.myassignmenthelp.net/statistics-assignment-help/chebyshev-theorem.png)

![alt text](https://allthingsstatistics.com/wp-content/uploads/2021/06/Chebyshevs-Inequality.png)


## UNIFORM DISTRIBUTION

In statistics, uniform distribution refers to a type of probability distribution in which all outcomes are equally likely. A deck of cards has within it uniform distributions because the likelihood of drawing a heart, a club, a diamond, or a spade is equally likely. A coin also has a uniform distribution because the probability of getting either heads or tails in a coin toss is the same.

1. Discrete Uniform Distribution
2. Continuous Uniform Distribution

![alt text](https://miro.medium.com/max/875/0*uswnTdoDOLJrZysc.png)


## BERNOULLI DISTRIBUTION

The Bernoulli distribution is a discrete distribution having two possible outcomes labelled by n=0 and n=1 in which n=1 ("success") occurs with probability p and n=0 ("failure") occurs with probability q=1-p, where 0<p<1. It therefore has probability density function.

![alt text](https://www.probabilisticworld.com/wp-content/uploads/2019/09/bernoulli-distribution-pmf.png)

![alt text](https://www.statisticshowto.com/wp-content/uploads/2016/07/bernoulli-distribution.png)

![alt text](https://miro.medium.com/max/875/1*KvnadxZI-Q-V9D9A4iEhfg.png)
## BINOMIAL DISTRIBUTION 

A binomial distribution can be thought of as simply the probability of a SUCCESS or FAILURE outcome in an experiment or survey that is repeated multiple times. The binomial is a type of distribution that has two possible outcomes (the prefix “bi” means two, or twice). For example, a coin toss has only two possible outcomes: heads or tails and taking a test could have two possible outcomes: pass or fail.

Notation ```X ~ B(n, p)``` where n is number of trials and p is the probability of the event i.e. success.

PMF =  ![alt text](https://andymath.com/wp-content/uploads/2019/03/BinomialProbabilityFunction-e1573148294456.jpg)


## LOG NORMAL DISTRIBUTION

In probability theory, a log-normal (or log-normal) distribution is a continuous probability distribution of a random variable whose logarithm is normally distributed. Thus, if the random variable X is log-normally distributed, then Y = ln(X) has a normal distribution. The log-normal distribution is a right skewed continuous probability distribution, meaning it has a long tail towards the right. It is used for modelling various natural phenomena such as income distributions, the length of chess games or the time to repair a maintainable system and more.
![alt text](https://cdn.wallstreetmojo.com/wp-content/uploads/2019/11/lognormal-distribution.jpg)


## POWER LAW DISTRIBUTION

The power law (also called the scaling law) states that a relative change in one quantity results in a proportional relative change in another. 
It has a long tail
According to Power Law Distribution: It follows ```80-20``` rule means 80% of data in 20% of interval.

![alt text](https://miro.medium.com/max/1168/1*S2SMWfSDGJST3hdgF4yWXw.png)

![alt text](https://www.comscore.com/var/comscore/storage/images/media/images/power_law_distribution/1980661-1-eng-US/Power_Law_Distribution.png)

### Pareto Distribution

There are 2 parameters 

```x(m) is scale i.e. similar to nu in Gaussian Distribution```

```alpha is shape i.e. standard deviation in Gaussian Distribution```

![alt text](https://upload.wikimedia.org/wikipedia/commons/1/11/Probability_density_function_of_Pareto_distribution.svg)

Here as alpha decreases width of tail increases. 

When alpha = infinity then all are 0 but only at x=1 it gives value. This type of distribution is called ```Dirac Delta Function```

We can think of example: traffic of file size, oil reserves fields.

Another way to identify the plot is power law is ```Log-Log``` plot.

![alt text](https://upload.wikimedia.org/wikipedia/commons/1/18/Log-log_plot_example.svg)


## BOX COX TRANSFORM (POWER TRANSFORM)

 Fortunately, we have a way to transform power-law or any non-linear distribution to Normal using a Box-Cox Transformation.
 
![alt text](https://media.geeksforgeeks.org/wp-content/uploads/20200531214708/powerlaw..png)

As per Pareto Distribution let X = [x1, x2, ...., xn]

As per Gaussian Distribution let Y = [y1, y2, ...., yn]

With the help of Box Cox Transform Pareto can be converted to Gaussian.

box cox(X) = λ

![alt text](https://www.statisticshowto.com/wp-content/uploads/2015/07/boxcox-formula-1.png)


## PEARSON CORRELATION COEFFICIENT (RANDOM VARIABLES)

This is used to measure relationship between random variables.
This is defined by:
```
P = cov(X,Y)/(std(X)*std(Y))
```
![alt text](https://upload.wikimedia.org/wikipedia/commons/3/34/Correlation_coefficient.png)

This works well when we have linear relationships. In order to fix this with non-linear we use Spearman Rank Correlation Coefficient.


## SPEARMAN RANK CORRELATION COEFFICIENT

![alt text](https://i.stack.imgur.com/bi0GX.png)
![alt text](https://i.stack.imgur.com/w6Qav.png)

Here rank is calculated by: Sort the column vector and smallest will get the rank 1 and increasing as value increases.

```
here r = PearsonCorrCoeff(rank(X),rank(Y))
```

## CONFIDENCE INTERVAL(CI)

Let X be random variable [x1, x2, x3, ...., xn]

where population mean = μ

where sample mean = x̄

μ ≈ x̄ = 1/n(∑x(i)); 0<i<n

As n increases then μ = x̄

Rather than giving point value we can give range

μ ∈ [interval] with 95% probability will provide much richer information.

This is called confidence interval.


### COMPUTING CONFIDENCE INTERVAL

If we know the underlying distribution then we can easily identify the CI.

Let X have mean ```μ``` and standard deviation be ```σ``` the 95% of data lies between μ-2σ and μ+2σ. Similarly if we want 90% of data we can see the distribution table to find the values.


### COMPUTING CONFIDENCE INTERVAL OF RANDOM VARIABLE

If we know the underlying distribution then we can easily identify the CI.

Let X have mean ```μ``` and standard deviation be ```σ``` the 95% of data lies between μ-2σ and μ+2σ. Similarly if we want 90% of data we can see the distribution table to find the values.

#### Case 1:

where population mean = μ

where sample mean = x̄

As per central limit theorem (CLT)

Then x̄ ≈ N(μ, σ/sqrt(n)) here n is the size of sample.

#### Case 2:

If we don't know population standard deviation and sample of size ```n```. Here as we don't know n and σ then follow t-distribution with n-1 degrees of freedom.

Therefore, x̄ follow t-distribution with n-1 degrees of freedom.

As degree of freedom increases peak increases.

![alt text](https://upload.wikimedia.org/wikipedia/commons/thumb/4/41/Student_t_pdf.svg/1024px-Student_t_pdf.svg.png)


### CONFIDENCE INTERVAL USING BOOTSTRAPPING

To calculate CI we can use programming and simulation tools i.e. using empirical-formula for complex things.

In this we take multiple samples and rearrange the median and then calculate confidence interval.


## HYPOTHESIS TESTING

Hypothesis testing is an act in statistics whereby an analyst tests an assumption regarding a population parameter. The methodology employed by the analyst depends on the nature of the data used and the reason for the analysis.

Hypothesis testing is used to assess the plausibility of a hypothesis by using sample data. Such data may come from a larger population, or from a data-generating process.

e.g. Let μ1 be mean of class 1 and μ2 be mean of class 2. 

Let μ1 = 148 and μ2 = 182 so μ2>μ1
1. Choosing a test statistic.
    We can think of μ2-μ1
2. Null Hypothesis (H0): Follows proof by contradiction.
In this we make assumption. It treats everything in 0 and 1 format.
H0: no-difference in means
H1(alternative hypothesis - opposite of H0): There is difference in means.
3. p-value: what is the probability of observing value of x if my null hypothesis is true.
Let's assume null hypothesis is true i.e. there is no difference. 

In another words it is the probability of null-hypothesis to be true.

p-value defines μ2-μ1=10 cm i.e difference between the heights.

if p=0.9 then null-hypothesis=True

if p=0.05 then null-hypothesis is False.

Calculating p-value: 

Tossing coin 5 times and let's suppose coin is unbiased

Then P(H) = 0.5

H0 = Coin is unbiased

as per p-value p(X=5 | H0) = (1/2)*(1/2)*(1/2)*(1/2)*(1/2) = 1/32 = 3%

```
If P(obs | H0) < 5% then Null-Hypothesis may be incorrect.
```