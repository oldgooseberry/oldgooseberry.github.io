---
layout:       page
title:        "Soln 2020-01 #4a"
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

This solution is the quick path to a solution, and will likely be the one found first from high school geometry. Consider the line added to the figure and the angles which have been added

![](/img/older/angle1_soln_a.png)

[A larger image for printing](/img/older/angle1_soln_a.jpeg)

From $\triangle{YZX}$ we can find $\angle{YZX}$ to be

{% raw %}{::nomarkdown}<div>
$\begin{align*}
180 &= 30 + 50 + \angle{YZX}\\
\angle{YZX} &= 180 - (30 + 50) = 100 \\
\end{align*}$
</div>{:/}{% endraw %}

---

Vertical Angle
:   Given two intersecting lines, the two nonadjacent angles with the same vertex are said to be vertical angles.


Theorem
:   Vertical angles are equal. $\leftarrow$ if you do not see this, ask

---

But, $\angle{CZB}$ is a vertical to $\angle{YZX}$ and so is equal. Further, given $\triangle{CZB}$, we know

{% raw %}{::nomarkdown}<div>
$\begin{align*}
180 &= \alpha + \beta + \angle{CZB} \\
180 &= \alpha + \beta + 100 \\
\alpha + \beta  &= 80 \\
\end{align*}$
</div>{:/}{% endraw %}

Finally, if we consder

$\triangle{A(C+\beta)(\alpha+B) \leftarrow \text{crap notation}}$

we can write

{% raw %}{::nomarkdown}<div>
$\begin{align*}
180 &= \angle{A} + \angle{C} + \angle{\alpha} + \angle{\beta} + \angle{B} \\
180 &= \angle{A} + \angle{C} + (\angle{\alpha} + \angle{\beta}) + \angle{B} \\
180 &= \angle{A} + \angle{C} +  80 + \angle{B} \\
100 &= \angle{A} + \angle{C} + \angle{B} \\
\end{align*}$
</div>{:/}{% endraw %}

