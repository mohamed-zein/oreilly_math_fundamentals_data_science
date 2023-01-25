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

[<<Previous](../probability/README.md) | [Next>>]()