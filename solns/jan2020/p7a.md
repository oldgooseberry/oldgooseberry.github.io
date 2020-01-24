---
layout:       page
title:        "Soln 2020-01 #7a"
author:       Beelzebub
category:     [Questions Jan2020]
use_math:     true
nav_order:    2
parent:       Jan 2020
grand_parent: Solutions To Questions
---

# Question

If Json can fold a crane in $4$ minutes, and Alex can fold $5$ cranes in $12$ minutes, how many minutes would it take for them to fold $10$ working together?

# Solution

To solve this problem, we will begin by finding the rate of crane construction for each person. Then, knowing the production rate we can compute the total number produced in a given time as the rate $\times$ time. But, we are given the number produced and seek the time. So we simply solve the equation for the unknown time.

First, the rates

{% raw %}{::nomarkdown}<div>
$\begin{align*}
R_{Json} &= \frac{\text{number of cranes}}{\text{time}} = \frac{1 \: \text{crane}}{4 \: \text{min}} \\
R_{Alex} &= \frac{\text{number of cranes}}{\text{time}} = \frac{5 \: \text{crane}}{12 \: \text{min}} \\
\end{align*}$
</div>{:/}{% endraw %}

We can then express the total number of cranes produced in a given time by the equation

$C_{total}(t) = R_{Json} \cdot t + R_{Alex} \cdot t$

Now, we want to know how long it will take to create a total of $10$. So we can write

{% raw %}{::nomarkdown}<div>
$\begin{align*}
R_{Json} \cdot t + R_{Alex} \cdot t &= 10 \: \text{crane} \\
\frac{1 \: \text{crane}}{4 \: \text{min}} \cdot t + \frac{5 \: \text{crane}}{12 \: \text{min}} \cdot t &= 10 \: \text{crane} \\
\left( \frac{1 \: \text{crane}}{4 \: \text{min}} + \frac{5 \: \text{crane}}{12 \: \text{min}} \right) \cdot t &= 10 \: \text{crane} \\
\left( \frac{3 \: \text{crane}}{12 \: \text{min}} + \frac{5 \: \text{crane}}{12 \: \text{min}} \right) \cdot t &= 10 \: \text{crane} \\
\left( \frac{8 \: \text{crane}}{12 \: \text{min}} \right) \cdot t &= 10 \: \text{crane} \\
t &= 10 \: \text{crane} \left( \frac{12 \: \text{min}}{8 \: \text{crane}}  \right)\\
t &= 15 \: \text{min} \\
\end{align*}$
</div>{:/}{% endraw %}

So it takes them $15$ minutes to create $10$ cranes working together.


