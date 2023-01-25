# Chapter 2: Descriptive and Inferential Statistics
_Statistics_ is the practice of collecting and analyzing data to discover findings that are useful or predict what causes those findings to happen.
## Descriptive Versus Inferential Statistics
* _Descriptive Statistics_ is the branch we use to summarize data; calculating mean, median, mode, charts, bell curves, and other tools to describe data.
* _Inferential Statistics_ is the branch that tries to uncover attributes about a larger population, often based on a sample.
## Populations, Samples, and Bias
* A **Population** is a particular group of interest we want to study, such as _all seniors over the age of 65 in the North America_, _all golden retrievers in Scotland_, or _current high school sophomores at Los Altos High School_.
    * We have boundaries on defining our population.
    * Some of these boundaries are broad and capture a large group over a vast geography or age group.
    * Others are highly specific and small such as the sophomores at Los Altos High School.
    * How you hone in on defining a population depends on what you are interested in studying.
* A **Sample** is a subset of the population that is ideally random and unbiased, which we use to infer attributes about the population.
    * We often have to study samples because polling the entire population is not always possible.
* **Bias** means our findings are skewed by overrepresenting a certain group at the expense of other groups.
    * To infer attributes about a population based on a sample, it’s important the sample be as random as possible so we do not skew our conclusions.
    * There are many types of bias, such as:
        * _Geographic bias_: in which we infer attributes about a population based on a sample from only one or few geographic locations while the population exists in many different locations.
        * _self-selection bias_: This particular type of bias where a specific group is more likely to include themselves in a sample.
        * _Confirmation bias_ is gathering only data that supports your belief, which can even be done unknowingly.
        * _Survival bias_ captures only living and survived subjects, while the deceased ones are never accounted for.

----------

## Descriptive Statistics
### Mean and Weighted Mean
#### Mean
* The _mean_ is the average of a set of values.
    * Sum the values and divide by the number of values.
    * The _mean_ is useful because it shows where the **center of gravity** exists for an observed set of values.
* There are two versions of the mean you will see: the sample mean $\overline{x}$ and the population mean $\mu$ as expressed here:

$$
\begin{align*}
\overline{x} & = \frac{x_{1} + x_{2} + x_{3} + \cdots + x_{n}}{n} = \sum{\frac{x_{i}}{n}} \\
\mu & = \frac{x_{1} + x_{2} + x_{3} + \cdots + x_{n}}{N} = \sum{\frac{x_{i}}{N}} \\
\text{Where: } & \\

& n \text{ represents sample size } \\
& N \text{ represents the population size}
\end{align*}
$$

#### Weighted Mean
_Weighted Mean_ is actually a weighted average in which we give each item a different weight.

$$
\text{weighted mean} = \frac{(x_{1} \cdot w_{1}) + (x_{2} \cdot w_{2}) + (x_{3} \cdot w_{3}) + \cdots + (x_{n} \cdot w_{n})}{w_{1} + w_{2} + w_{3} + \cdots + w_{n}}
$$

### Median
* The _median_ is the middlemost value in a set of ordered values.
* We sequentially order the values, and the _median_ will be the centermost value.
* The _median_ can be a helpful alternative to the mean when data is skewed by _outliers_, or values that are extremely large and small compared to the rest of the values.
* When your _median_ is very different from your _mean_, that means you have a skewed dataset with outliers.

    > **The Median Is a Quantile**  
    > There is a concept of _quantiles_ in descriptive statistics. The concept of quantiles is essentially the same as a median, just cutting the data in other places besides the middle. The median is actually the 50% quantile, or the value where 50% of ordered values are behind it. Then there are the 25%, 50%, and 75% quantiles, which are known as _quartiles_ because they cut data in 25% increments.

### Mode
* The _mode_ is the most frequently occurring set of values.
* It primarily becomes useful when your data is repetitive and you want to find which values occur the most frequently.
    * When no value occurs more than once, there is no mode.
    * When two values occur with an equal amount of frequency, then the dataset is considered _bimodal_.
* In practicality, the _mode_ is not used a lot unless your data is repetitive.
* This is commonly encountered with integers, categories, and other discrete variables.

### Variance and Standard Deviation
There are some calculation differences for the sample versus the population.
#### Population Variance and Standard Deviation
* In describing data, we are often interested in measuring the differences between the _mean_ and every data point. This gives us a sense of how **spread out** the data is.
* The _variance_ is a measure of how spread out our data is.
    * A higher variance means more spread.
$$
\begin{align*}
\text{population variance} & = \frac{(x_{1} - mean)^{2} + (x_{2} - mean)^{2} + \cdots + (x_{n} - mean)^{2}}{N} \\
\sigma^{2} & = \frac{\sum{(x_{i} - \mu)^{2}}}{N}
\end{align*}
$$

* This _population variance_ is larger than any of our observations because we did a lot squaring and summing, putting it on an entirely different metric.
* The _standard deviation_ is the variance scaled into a number expressed in similar scale to our observations which makes it a bit more meaningful:

$$
\sigma = \sqrt{\frac{\sum{(x_{i} - \mu)^{2}}}{N}}
$$

#### Sample Variance and Standard Deviation
There is an important tweak we need to apply to these two formulas when we calculate for a **sample**:

$$
\begin{align*}
s^{2} & = \frac{\sum{(x_{i} - \overline{x})^{2}}}{n-1} \\
s & = \sqrt{\frac{\sum{(x_{i} - \overline{x})^{2}}}{n-1} \\}
\end{align*}
$$

* we divide by $n–1$ rather than the total number of items $n$.
    * We do this to decrease any bias in a sample and not underestimate the variance of the population based on our sample.
    * By counting values short of one item in our divisor, we increase the variance and therefore capture greater uncertainty in our sample.


### The Normal Distribution
The _normal distribution_, also known as the _Gaussian distribution_, is a symmetrical bell-shaped distribution that has most mass around the mean, and its spread is defined as a standard deviation. The "tails" on either side become thinner as you move away from the mean.  
![A normal distribution](./images/normal-distribution-01.jpg)

#### Properties of a Normal Distribution
* It’s symmetrical; both sides are identically mirrored at the mean, which is the center.
* Most mass is at the center around the mean.
* It has a spread (being narrow or wide) that is specified by standard deviation.
* The _tails_ are the least likely outcomes and approach zero infinitely but never touch zero.
* It resembles a lot of phenomena in nature and daily life, and even generalizes non-normal problems because of the central limit theorem.

#### The Probability Density Function (PDF)
* The [standard deviation](#variance-and-standard-deviation) plays an important role in the normal distribution, because it defines how **spread out** it is.
* The **probability density function (PDF)** that creates the normal distribution is as follows:

$$
f(x) = \frac{1}{\sigma} \cdot \sqrt{2 \pi} \cdot e^{- \frac{1}{2} \left(\frac{x-\mu^{2}}{\sigma
} \right)}
$$

#### The Cumulative Distribution Function (CDF)
* With the normal distribution, the vertical axis is not the probability but rather the likelihood for the data.
* To find the probability we need to look at a given range, and then find the area under the curve for that range.  
![A CDF measuring probability between 62 and 66 pounds](./images/normal-distribution-02.jpg)

##### A PDF vs CDF
The CDF, which is an S-shaped curve (called a sigmoid curve), projects the area up to that range in the PDF.

![A PDF alongside its CDF](./images/normal-distribution-03.jpg)

### The Inverse CDF
* **The Inverse CDF** enables us to look up an area on the CDF and then return the corresponding x-value.
* The **Inverse CDF**, also called the _PPF_ or _quantile function_

![The Inverse CDF](./images/inverse-cdf.jpg)


[<<Previous](../probability/README.md) | [Next>>]()