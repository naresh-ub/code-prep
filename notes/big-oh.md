## Notes from Harvard CS50 course

What makes a program fast or slow? The speed of a computer program is `not measured in seconds or minutes` because computer hardware and software is drastically different.

The speed is measured using Asymptotic Complexity of a program and Big-O Notation.

Formally, a function $f(x)$ runs in the order of $g(x)$ if there exists a value $x_0$ and a constant $C$ such that $f(x) \leq C\cdot g(x) \enspace \forall \enspace x > x_0$.

$$
f(x) \leq C\cdot g(x) \enspace \forall \enspace x > x_0
$$

This is a way to represent how the run-time of the program grows asymptotically i.e., as the size of the input approaches infinity.

- $O(1)$ - Constant time algorithms.
- $O(n)$ - Linear time algorithms. (Counting number of chars in string).
- $O(n^2)$ algos take more time than $O(n)$. Keep in mind that when the input is very small $O(n^2)$ might be good enough.
- $O(log(n))$ are logarithmic time algorithms that are faster than linear time algorithms (example is binary search algorithm to find an element in a sorted array of elements).

To represent the best case and worst case of the asymptotic relation, there are more terms introduced.

For example, the `best case time complexity` to find an element in a list using binary search is $\Omega(1)$. This happens when the element is in the middle of the array and hence no matter how big/small the rest of the array is, the time complexity still will be constant time.

- $\Omega$ represents the best case time complexity.
- $O$ represents the worst case time complexity.
- $\Theta$ can be used when the best case and worst case complexities are the same.

### Summary
In summary these are the ways to reason about a program's efficiency instead of considering the time taken for a program to run on a computer (which is effected by a lot of external factors).

## Notes from Derek Banas's video
$O$ is a way to measure how well a computer algorithm scales as the amount of data increases and approaches infinity.

The time taken to run of an algorithm depends on the highest order of $n$ in its time-complexity.

Example: $O(n^3)+O(n)+100$ can be boiled down to $O(n^3)$.

- $O(1)$ -> appending an element to a list.
- $O(log(n))$ -> binary search.
- $O(n)$ -> linear search.
- $O(n^2)$ -> bubble sort.

## Notes from profbillbyrne

Consider $f(n) = 4n^2 + 16n + 2$ and $g(n) = n^4$. We are trying to find a constant $C$ to check if $f(n) \leq C \cdot g(n)$

if $C$ = 1, the inequality $f(n) \leq C \cdot g(n)$ is true for all values $> 4$. ($n_0 = 4$).

$$ f(n) \text{ is } \Omega(g(n)) \text{ if } C \text{ and } n_0;\\
f(n) \geq C \cdot g(n) \enspace \forall \enspace n > n_0$$


$$ f(n) \text{ is } \Theta(g(n)) \text{ iff }$$

1. $f(n) = O(g(n)) \text{ and }$
2. $f(n) = \Omega(g(n))$









