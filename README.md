# oreilly_math_fundamentals_data_science
Repo for code examples of book Essential Math For Data Science

## Chapter 2 - Probability
The most popular way to express probability is as a percentage, as in _There is a 70% chance my flight will be late._ We will call this probability $P(X)$ , where $X$ is the event of interest.

$$
\begin{align*}
P(X) & = 0.70 \\
P(\text{not } X) &= 1 - 0.70 = 0.30
\end{align*}
$$

* **Probability** is about quantifying predictions of events yet to happen.
    * Probabilities of all possible mutually exclusive outcomes for an event (meaning only one outcome can occur, not multiple) must sum to 1.0 or 100%.
    * probability can be expressed as an odds $O(X)$ such as 7:3, 7/3, or 2.33

$$
\begin{align*}
P(X) & = \frac{O(X)}{1 + O(X)} \\
O(X) & = \frac{P(X)}{1 - P(X)}
\end{align*}
$$

* **Likelihood** is measuring the frequency of events that already occurred.

### Probability vs Statistics
* **Probability** is purely theoretical of how likely an event is to happen and does not require data.
* **Statistics**, on the other hand, cannot exist without data and uses it to discover probability and provides tools to describe data.

### Probability Math
#### Joint Probabilities
The probability that both events will occur together. This is known as a _joint probability_.

$$
\begin{align*}
\text{If } A \text{ and } B \text{ are independent events, Then:} \\
P(A \cap B) = P(A) \times P(B)
\end{align*}
$$
#### Union Probabilities
When we deal with **OR** operations with probabilities, this is known as a _union probability_.
##### Mutually exclusive events
* _Mutually exclusive_ events are events that cannot occur simulta‐ neously.
* To get the union probability for _mutually exclusive_ events, simply add them together.

$$
P(A \cup B) = P(A) + P(B)
$$

##### Nonmutually exclusive events
* _Nonmutually exclusive_ events are events that can occur simultaneously.
* To calculate probability in this case, we use the _sum rule of probability_ and ensures every joint event is counted only once:

$$
\begin{align*}
P(A \cup B) & = P(A) + P(B) - P(A \cap B) \\
& = P(A) + P(B) - \left( P(A) \times P(B) \right)
\end{align*}
$$

* **Note** that this formula will work also with [_mutually exclusive_ events](#mutually-exclusive-events) as the joint probability $P(A \cap B)$ is going to be $0$.