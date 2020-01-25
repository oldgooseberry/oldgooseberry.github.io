---
layout:       page
title:        "Soln 2020-01 #9a"
author:       Beelzebub
category:     [Questions Jan2020]
use_math:     true
nav_order:    2
parent:       Jan 2020
grand_parent: Solutions To Questions
---

# Question

What is the smallest positive solution to

$$(2x + 1)(x -3) \equiv 7 \: \text{mod} \: 23$$

# Solution

To solve this problem, we need to be careful. We can not just solve the equation as if we were in $\mathbb{R}$. We need to plot this looking for intersections of the curve $f(x) = (2x + 1)(x-3)$ and curves of the form $g_{i}(x) = 7 + (23 * i)$ where $i \in \mathbb{Z}$. Doing this for $i = 0$ we get

{% raw %}{::nomarkdown}<div>
$\begin{align*}
(2x+1)(x-3) &= 7 \\
2x^{2} - 6x + x - 3 &= 7\\
2x^{2} - 5x -3 &= 7 \\
2x^{2} - 5x - 10 &= 0 \\
\end{align*}$
</div>{:/}{% endraw %}


Looking at the factors of $10$ and $2$ we see there is no integer solutions possible. We will need to continue this with $i \in \mathbb{Z} \: i > 0$. As this is just an exercise in algebra, I wrote a julia program to search the first $21$ values.  

```julia
julia> for i in 1:21
       k(x) = 2x^2 - 5x - 3 - (7 + i*23)
       @show factor(k(x))
       end
factor(k(x)) = (x + 3)*(2*x - 11)
factor(k(x)) = 2*x^2 - 5*x - 56
factor(k(x)) = 2*x^2 - 5*x - 79
factor(k(x)) = (x + 6)*(2*x - 17)
factor(k(x)) = 2*x^2 - 5*x - 125
factor(k(x)) = 2*x^2 - 5*x - 148
factor(k(x)) = 2*x^2 - 5*x - 171
factor(k(x)) = 2*x^2 - 5*x - 194
factor(k(x)) = 2*x^2 - 5*x - 217
factor(k(x)) = 2*x^2 - 5*x - 240
factor(k(x)) = 2*x^2 - 5*x - 263
factor(k(x)) = 2*x^2 - 5*x - 286
factor(k(x)) = 2*x^2 - 5*x - 309
factor(k(x)) = 2*x^2 - 5*x - 332
factor(k(x)) = 2*x^2 - 5*x - 355
factor(k(x)) = 2*x^2 - 5*x - 378
factor(k(x)) = 2*x^2 - 5*x - 401
factor(k(x)) = 2*x^2 - 5*x - 424
factor(k(x)) = 2*x^2 - 5*x - 447
factor(k(x)) = 2*x^2 - 5*x - 470
factor(k(x)) = (x - 17)*(2*x + 29)
```

As we can see, $i = 1$ factored but does not have integer solutions. The same is true for $i = 4$. However, for $i = 21$ we do get a solution which is a positive integer <br/> 

{% raw %}{::nomarkdown}<div>
$\begin{align*}
(x - 17) &= 0 \\ 
x &= 17
\end{align*}$
</div>{:/}{% endraw %}

This is the smallest positive solution.
