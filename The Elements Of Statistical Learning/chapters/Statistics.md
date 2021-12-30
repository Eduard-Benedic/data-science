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
