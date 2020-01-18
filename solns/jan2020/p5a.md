---
layout:       page
title:        "Soln 2020-01 #5a"
author:       Beelzebub
category:     [Questions Jan2020]
use_math:     true
nav_order:    2
parent:       Jan 2020
grand_parent: Solutions To Questions
---

# Question

What is the smallest prime factor of $10^{101} + 1$

# Solution

We want to look for a pattern in the factorization of $$10^{n} + 1$$. To this end, we look at the values and factorization for $1 \leq n \leq 10$. A simple `julia` program to do this is

```julia
julia> for i in 1:10
       println("$(BigInt(10)^i + 1) = $( factor(Set, BigInt(10)^i + 1) )")
       end
11 = Set(BigInt[11])
101 = Set(BigInt[101])
1001 = Set(BigInt[7, 13, 11])
10001 = Set(BigInt[137, 73])
100001 = Set(BigInt[11, 9091])
1000001 = Set(BigInt[101, 9901])
10000001 = Set(BigInt[11, 909091])
100000001 = Set(BigInt[17, 5882353])
1000000001 = Set(BigInt[7, 52579, 13, 19, 11])
10000000001 = Set(BigInt[3541, 101, 27961])
```

We see there is a pattern developing. For $n$ odd, the smallest prime factor is $11$. For $n$ even, we can not say anything about the smallest prime factor. Since we were asking about $$10^{101} + 1$$ and $101$ is odd, then $11$ is the smallest prime factor.

A more *Algebraic* (and complete) solution to this problem can be found by noting the following relationships

{% raw %}{::nomarkdown}<div>
$\begin{split} 
x^3 + 1 &= (x+1)(x^{2} - x + 1) \\
x^5 + 1 &= (x+1)(x^{4} - x^{3} + x^{2} - x + 1) \\
x^7 + 1 &= (x+1)(x^{6} - x^{5} + x^{4} - x^{3} + x^{2} - x + 1) \\
\vdots \\
x^{101} + 1 &= (x+1)(x^{100} - x^{99} + x^{98} - \ldots + x^{6} - x^{5} + x^{4} - x^{3} + x^{2} - x + 1) \\
\end{split}$
</div>{:/}{% endraw %}

That is, for $n$ odd, $x^{n} + 1$ can be factored as

$$x^{n} + 1 = (x + 1) \left( \sum_{i = 0}^{n - 1} (-1)^{i} x^{i} \right)$$

Now let $x = 10$ and get the relationship

$$
10^{n} + 1 = 11 \left( \sum_{i = 0}^{n - 1} (-1)^{i} (10)^{i} \right) \\
\text{for odd} \: n
$$

---

> **Note**: Never discount using a tool like a CAS to explore the "shape" of the problem. This can often point you in the direction of a more formal or exact solution/proof. Math actually can be a very [experimental experience](https://en.wikipedia.org/wiki/Experimental_mathematics), though rarely enough is this shown.

Exploring factoing in `julia` can be acomplished by doing the following (this assumes the `SymPy` module has not been built or loaded into your `julia` enviroment if you are using the suggested service skip the first command(s))

```julia
julia> using Pkg; Pkg.add("SymPy"); using SymPy

<LOTS OF STUFF HERE>

julia> @vars x
(x,)

julia> factor(x^3 + 1)
        ⎛ 2        ⎞
(x + 1)⋅⎝x  - x + 1⎠

julia> factor(x^5 + 1)
        ⎛ 4    3    2        ⎞
(x + 1)⋅⎝x  - x  + x  - x + 1⎠

julia> factor(x^7 + 1)
        ⎛ 6    5    4    3    2        ⎞
(x + 1)⋅⎝x  - x  + x  - x  + x  - x + 1⎠

julia> factor(x^4 + 1)
 4
x  + 1

julia> factor(x^6 + 1)
⎛ 2    ⎞ ⎛ 4    2    ⎞
⎝x  + 1⎠⋅⎝x  - x  + 1⎠

julia> factor(x^8 + 1)
 8
x  + 1

julia>
```
