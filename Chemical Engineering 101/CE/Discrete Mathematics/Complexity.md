## Computational Compexity
### Asymptotic Computational Complexity
In [computational complexity theory](https://en.wikipedia.org/wiki/Computational_complexity_theory "Computational complexity theory"), **asymptotic computational complexity** is the usage of [asymptotic analysis](https://en.wikipedia.org/wiki/Asymptotic_analysis "Asymptotic analysis") for the estimation of computational complexity of [algorithms](https://en.wikipedia.org/wiki/Algorithm "Algorithm") and [computational problems](https://en.wikipedia.org/wiki/Computational_problem "Computational problem"), commonly associated with the usage of the [big O notation](https://en.wikipedia.org/wiki/Big_O_notation "Big O notation").

### Worst Case Complexity
- For each n, worst case input forces algorithm to take the maximum amount of time required.
- Upper Bound for overall running Time.
- It is a function of Algorithm Itself.
- Maybe Rare: Very Pessimistic .

### Average Case Complexity
- Compute Average time taken over all inputs
- Parameters: Average wrt, Likelihood of all Inputs, Probability Distribution over all inputs.


## Big O Notation

Big O notation describes an upper bound on the growth rate of a function. For functions $f(n)$ and $g(n)$, we say:

$f(n) = O(g(n)) \text{ as } n \to \infty$

if there exist positive constants $M$ and $n_0$ such that:

$|f(n)| \leq M \cdot |g(n)| \quad \text{for all } n \geq n_0.$

### Key Points:
- $g(n)$ must be non-zero for sufficiently large $n$.
- The notation captures the **asymptotic behavior** of $f(n)$, focusing on its growth rate relative to $g(n)$.
- Often used in computer science to classify algorithms based on their worst-case performance.

In simpler terms, $f(n)$ is "Big O of $g(n)$" if $f(n)$ grows no faster than a constant multiple of $g(n)$ for large $n$.


- $n^3$ is not $O(n^2)$ as no matter what $c$ we choose, $cn^2$ will always be dominated by $n^3$ for $n \geq c$ 

- If $f_1(n)$ is $O(g_1(n))$ and $f_2(n)$ is $O(g_2(n))$,
- then $f_1(n)+f_2(n)$ is $O(max(g_1(n),g_2(n)))$

- For Algorithm with many phases the least efficient phase is the Upper Bound for the whole Algorithm.

## Omega Notation: Definition

Omega notation describes a lower bound on the growth rate of a function. For functions $f(n)$ and $g(n)$, we say:

$f(n) = \Omega(g(n)) \text{ as } n \to \infty$

if there exist positive constants $M$ and $n_0$ such that:

$|f(n)| \geq M \cdot |g(n)| \quad \text{for all } n \geq n_0.$

### Key Points:
- $g(n)$ must be non-zero for sufficiently large $n$.
- The notation captures the **asymptotic minimum growth rate** of $f(n)$, ensuring that $f(n)$ grows at least as fast as a constant multiple of $g(n)$ for large $n$.
- Often used in computer science to classify algorithms based on their best-case performance or guaranteed lower bounds.

In simpler terms, $f(n)$ is "Omega of $g(n)$" if $f(n)$ grows at least as fast as $g(n)$ for large $n$.

- Typically we establish lower bound for problem as a whole rather than individual algorithms, eg: Sorting requirest $\Omega (n\log n)$ comparisons, no matter how clever the algorithm is.

## Theta Notation: Definition

Theta notation describes a tight bound on the growth rate of a function. For functions $f(n)$ and $g(n)$, we say:

$f(n) = \Theta(g(n)) \text{ as } n \to \infty$

if there exist positive constants $M_1$, $M_2$, and $n_0$ such that:

$M_1 \cdot |g(n)| \leq |f(n)| \leq M_2 \cdot |g(n)| \quad \text{for all } n \geq n_0.$

### Key Points:
- $g(n)$ must be non-zero for sufficiently large $n$.
- The notation captures the **asymptotic tight bound**, meaning $f(n)$ grows at the same rate as $g(n)$ within constant factors.
- Often used in computer science to classify algorithms when their growth rate is tightly constrained between upper and lower bounds.

In simpler terms, $f(n)$ is "Theta of $g(n)$" if $f(n)$ grows at the same rate as $g(n)$ for large $n$, within a constant factor.

