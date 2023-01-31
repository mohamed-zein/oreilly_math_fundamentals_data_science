# Chapter 4: Linear Algebra
## What is a Vector?
* A _vector_ is an arrow in space with a specific direction and length, often representing a piece of data.
* In its fundamental form, it has no concept of location so always imagine its tail starts at the origin of a Cartesian plane (0,0).
* The purpose of the vector is to visually represent a piece of data.
* Below figure, shows a vector $\vec{v}$ that moves three steps in the horizontal direction and two steps in the vertical direction.
![A simple vector](./images/vector-01.jpg)  
* We declare a vector mathematically like this:

$$
\vec{v} = \begin{bmatrix}
x \\
y
\end{bmatrix}
$$

### Adding and Combining Vectors
* **Numerically**: simply add the respective $x$-values and then the $y$-values into a new vector

$$
\begin{align*}
\vec{v} & = \begin{bmatrix} 3 \\ 2 \end{bmatrix} \\
\vec{w} & = \begin{bmatrix} 2 \\ -1 \end{bmatrix} \\
\vec{v} + \vec{w} & = \begin{bmatrix} 3+2 \\ 2+ -1 \end{bmatrix} = \begin{bmatrix} 5 \\ 1 \end{bmatrix}
\end{align*}
$$

* **Visually**: connect one vector after the other and walk to the tip of the last vector. The point you end at is a new vector, the result of summing the two vectors.  
![Adding two vectors into a new vector](./images/vector-02.jpg)
* It does not matter whether we add v before w or vice versa, which means it is _commutative_ and order of operation does not matter.
### Scaling Vectors
* _Scaling_ is growing or shrinking a vector’s length by multiplying or scaling it with a single value, known as a _scalar_.
![Scaling a vector](./images/vector-03.jpg)
* Mathematically, you multiply each element of the vector by the scalar value:

$$
\begin{align*}
\vec{v} & = \begin{bmatrix} 3 \\ 1 \end{bmatrix} \\
2\vec{v} & = 2\begin{bmatrix} 3 \\ 1 \end{bmatrix} = \begin{bmatrix} 3 \times 2 \\ 1 \times 2 \end{bmatrix} = \begin{bmatrix} 6 \\ 2 \end{bmatrix}
\end{align*}
$$



[<<Previous](../statistics_hypothesis_testing/README.md) | [Next>>]()