---
layout:       page
title:        "Soln 2020-01 #3"
author:       Beelzebub
category:     [Questions Jan2020]
use_math:     true
nav_order:    1
parent:       Problems From the Past
grand_parent: Solutions To Questions
---

# Question

The triangle is equilateral, and the upper rectangle is made of two squares. The upper rectangle's area is 12. What is the l   ower square's area?

![](/img/older/square_2.png)

[A larger image for printing](/img/older/square_2.jpeg)

# Solution

To solve this problem, we begin by adding a few things to the diagram. First, since the triangle is equilateral then we know each angle is $60^{\circ}$. We also know that each side has the same lenght, lets call it $\alpha$. To save space, we will also note on the diagram the ration of the sides in a $30^{\circ}, 60^{\circ}, 90^{\circ}$ triangle.

![](/img/older/square_2_soln.png)

[A larger image for printing](/img/older/square_2_soln.jpeg)

With this, the original problem states the area of the upper rectangle is 12; and it is made of two squares. Given this, we know the area of one square is $6$. Therefore the lenght of the side of the square is $x^{2} = 6$ or $x = \sqrt{6}$.

But, the height of the equilateral is then $\sqrt{6}$. With this, and what we know of $30^{\circ}, 60^{\circ}, 90^{\circ}$ triangles; we can write the following ratio

$$ \frac{1}{\frac{\alpha}{2}} = \frac{\sqrt{3}}{\sqrt{6}} $$

> Note: This is the ration of the "unit" $30,60,90$ triangle to the one we have. If you do not see this, ask.

Solving for $\alpha$ ,the lenght of the side of the bottom square, we get

{% raw %}{::nomarkdown}<div>
$\begin{align*}
\frac{2}{\alpha} &= \frac{\sqrt{3}}{\sqrt{6}} \\
2 &= \alpha \cdot \frac{\sqrt{3}}{\sqrt{6}} \\
2\sqrt{6} &= \alpha \sqrt{3} \\
\frac{2\sqrt{6}}{\sqrt{3}} &= \alpha\\
\end{align*}$
</div>{:/}{% endraw %}

Since $\alpha$ is the side of the bottom square, we can find the area of the bottom square as


{% raw %}{::nomarkdown}<div>
$\begin{align*}
\text{Area Bottom Square } &= \left( \alpha \right)^{2} = \left( \frac{2\sqrt{6}}{\sqrt{3}} \right) ^{2} \\
\text{Area Bottom Square } &= \frac{4 \cdot 6}{3} \\
\text{Area Bottom Square } &= 4 \cdot 2 \\
\text{Area Bottom Square } &= 8 \\
\end{align*}$
</div>{:/}{% endraw %}
