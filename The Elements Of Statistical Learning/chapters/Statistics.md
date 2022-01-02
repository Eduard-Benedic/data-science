# Measures of Location

## Measures of Location

### Mean (sample mean or arithmetic average.)
*Def* -  middle point.

$ \bar{x} - average \space value \space of \space observation $
$$ \bar{x} = \frac{\sum_{i=1}^n x_i}{n}  $$

Mean is sensitive to outliers.

### Median (middle)
Middle value when $x_i$ is ordered.

$ \tilde{x} $ - median

The middle number if $x_i$ odd else the average between the n and n+1.

### Quartiles

Divides the data set into 4 equal parts.

Percentiles divide data into finer segments

## Measures of Variability

### Range

*Range*  = Max - Min (difference between the largest and smalles number)

*Deviation from the mean* - difference between each point and the mean $\bar{x}$

$$ Sum-of-deviation = \sum_{i=1}^n(x_i - \bar{x}) = 0$$

So, we can't use this to assess the distribution. Instead we can square the differences and we will get a positive number.

The formula above is proven below.

$$ \sum{\bar{x}} = n \bar{x} $$
$$ \sum(x_i - \bar{x} ) = \sum{x_i} - \sum{\bar{x}} =  \sum{x_i} - n (\frac{1}{n} \sum{\bar{x_i}})  $$

### Sample Variance

Sample variance formula:
$$ s^2 = \frac{ \sum{(x_i - \bar{x})^2} }{n - 1} = \frac{S_{xx}}{n - 1}
$$

The **Sample Standard Deviation**

$$ s = \sqrt{s^2} $$

The population variance is

$$ \sigma^2 = \frac{\sum_{i = 1}^N (x_i - \mu)^2}{N} $$ 
$ \mu - population \space mean  $

Note the N and not n - 1.

**Note!**

It is customary to $s^2 - sample \space variance$ as being based on **n -1** *degrees of freedom* (df).

That is because specifying the values for every *n - 1* data points we can obtain the sample variance.

The reason being the sum of the deviations will always equal 0.

### Boxplots

Summarizes important features such as
* center
* spread
* extent and nature of any departure from symmetry
* outliers

# Discrete Random Vrialbes and Probability Distributions

## Random Variables

A random variable associates an outcome with a code.

In math a random variable is any rule that associates a number with each outcome.

Bernoulli Random Variable - Any random variable whose output is 0 and 1

Types of Random variables
* Discrete - rv (random var) whose possible outcomes constitute a finite set or can be listed in an infinite sequence in which tere are elements in sequence (first, second, etc)
* Continous - if
  * The set of possible values consists of all numbers in a single interval on the number line
  * No possible value of the variable has positive probability, that is $P(X=c) = 0 $ for any c

### Probability Distributions for Discrete Random Variables

Probability distribution or probability mass function (pmf) of a rv (random variable) is defined for every number

$$ x \space by \space p(x) = P(X=x) = P(all  \space s \space \epsilon )   $$

### A parameter of Probability Distribution

For Bernoully rv (random variable) we can generally describe the probability mass distribution as:

$$
  \begin{equation*}
    p(x;\alpha) = \left\{
      \begin{array}{l}
      1 - \alpha  & \text{if } x = 0,\\
      \alpha & \text{if } x = 1
      \end{array} \right.
  \end{equation*}
$$

### The Cumulative Distribution Function

The cumulative distribution function (cdf) $F(x)$ of a discrete rv X with pmf(probability mass function) $p(x)$ is defined for every number x by.

$$ F(x) = P(X \le x ) = \sum_{y:y \le x }p(y)  $$

### Expected values of Discrete Random Variables

Expected Value of $X$

$$ E(X) = \mu_X = \sum_{x \epsilon D }{x \cdot p(x)} $$


The expected value is the equivalent of the mean for random variables. Thus, Expected Value can also be represented with $ \mu $, population mean.

From here we have the variance.

### The Variance of X

$$ V(X) = \sum_{D}(x-y)^2 \cdot p(x) = E(X-\mu)^2 $$

**Standard Deviation** is:

$$ \sigma_X = \sqrt{\sigma^2}_X $$

Shortcut formula for computing variance($ \sigma $). Computationally less expensive.

$$ V(X) = \sigma^2 = [\sum_D x^2 \cdot p(x)] - \mu^2 = E(X^2) - [E(X)]^2 $$

For a variance of a function we have

$$ V[h(X)] =  \sigma^2_{h(X)} = \sum_{D}{\{h(x) - E[h(x)]\}}^2 \cdot p(x) $$

### Moments and Moment Generating Function

Sometimes the expected values of integer powers of $X \space and \space X - \mu $ are called **moments**.

Expected values of powers of $X$ are called **moments about 0** and powers of $ X - \mu $ are called **moments about the mean**.

E.g. Second moment about 0
$$E(X^2)$$

Fourth moment about mean
$$ E[(X-\mu)^4] $$

The **first moment about 0** is the mean

The second moment about the mean is the variance.

And the third moment about the mean is also important.

$$ 
  E[(X - \mu)^3] = \sum_{x \epsilon D}(x - \mu)^3 \cdot p(x)
$$

This measure can be used for a lack of assymetry. However we want scale independence results. Divide everything by:

$$
  \frac{E[(X - \mu)^3]}{\sigma^3} = E[(\frac{X - \mu}{\sigma})^3]
$$

Departure from symmetry - skewness.

### Moment generating function

When we consider the expected value as a function of $t$, the result is called the moment generatig function (mgf).

$$ M_X(t) = E(e^{t X}) = \sum_{x \epsilon D}  e^{t \cdot x}p(x)$$
Where D is the set of all possible values for $X$.