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

