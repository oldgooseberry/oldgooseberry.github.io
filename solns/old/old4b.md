---
layout:       page
title:        "Soln 2020-01 #4b"
author:       Beelzebub
category:     [Questions Jan2020]
use_math:     true
nav_order:    1
parent:       Problems From the Past
grand_parent: Solutions To Questions
---

# Question

What is the sum of the measures of the three pink angles, $\angle{A} + \angle{B} + \angle{C}$?

![](/img/older/angle1.png)

[A larger image for printing](/img/older/angle1.jpeg)


# Solution

In this solution, we will be working with a few simple facts.

1. Any polygon can be divided in the triangles
2. These triangles have a sum of internal angles of $180°$.
3. If a polygon has $n$ sides, it can be divided into $(n-2)$ triangles

Collectively, these imply the sum of the internal angles of any polygon with $n$ sides is

$ (n - 2) \cdot 180°$

Now consider the labels added to the figure.

![](/img/older/angle1_soln_b.png)

[A larger image for printing](/img/older/angle1_soln_b.jpeg)

We can not list all the triangles in the figure

{% raw %}{::nomarkdown}<div>
$\begin{align*}
\triangle{CaE}\\
\triangle{BbD}\\
\triangle{EdD}\\
\triangle{ABe}\\
\triangle{CcA}\\
\end{align*}$
</div>{:/}{% endraw %}

First, the sum of the internal angles of all these triangles is

$5 \cdot 180 = 900$

Second, if we look carefully at the triangles listes, we notice that the internals angles

$\angle{a}, \angle{b}, \angle{c}, \angle{d}, \angle{e}$

are used one time and form a $5$-sided polygon (a pentagon). The sum of the internal angles of a pentagon is

$(5 -2) \cdot 180 = 540$

Further, the internal angles

$\angle{A}, \angle{B}, \angle{C}, \angle{D}, \angle{E}$

are all used $2$ times, and we know the sizes of $\angle{D}$ and $\angle{E}$. We can then write the equation

{% raw %}{::nomarkdown}<div>
$\begin{align*}
(5 \cdot 180) &= (\text{internal angles of the pentagon}) + 2 (\angle{A} + \angle{B} + \angle{C} + \angle{D} + \angle{E}) \\
900 &= 540 + 2(\angle{A} + \angle{B} + \angle{C} + 50 + 30) \\
900 &= 540 + 2(\angle{A} + \angle{B} + \angle{C}) + 2(80) \\
900 &= 540 + 2(\angle{A} + \angle{B} + \angle{C}) + 160 \\
900 &= 700 + 2(\angle{A} + \angle{B} + \angle{C}) \\
200 &= 2(\angle{A} + \angle{B} + \angle{C}) \\
100 &= \angle{A} + \angle{B} + \angle{C} \\
\end{align*}$
</div>{:/}{% endraw %}


