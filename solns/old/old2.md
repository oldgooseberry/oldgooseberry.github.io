---
layout:       page
title:        "Soln 2020-01 #2"
author:       Beelzebub
category:     [Questions Jan2020]
use_math:     true
nav_order:    1
parent:       Problems From the Past
grand_parent: Solutions To Questions
---

# Question

It is possible to write the number $2020$ as the difference of two squares

$2020 = 106^{2} - 96^{2}$

is there any *other way* to write $2020$ as the difference of two squares?

# Solution

If we spend a few minutes thinking about the wording of this problem, we might eventually hit on the phrase *"difference of two squares"*. From *Algebra*, what does this mean exactly. This means we have something like

$A^{2} - B^{2}$

But, we know something about expressions which look like this. That is, we can factor these expressions as

$(A - B)(A + B)$

This means our question is really asking, can we write

$A^{2} - B^{2} = (A - B)(A + B) = 2020$

in some way other than

$2020 = 106^{2} - 96^{2}$

This means we are looking for $A$ and $B$ such that $(A - B)$ and $(A + B)$ are factors of $2020$. To that end, the first thing to do is look at the factors of $2020$. Factoring we get

$2020 = 2^{2} \cdot 5 \cdot 101$

This means we need to solve equations like

{% raw %}{::nomarkdown}<div>
$\begin{align*}
A + B &= (101)(2) = 202 \\
A - B &= (5)(2) = 10 \\
\end{align*}$
</div>{:/}{% endraw %}

We know $A + B$ is bigger than $A - B$ so we know the factor $A + B$ will always use at least the factor $101$. Looking at the number of factors and the previous fact, there are only $5$ different sets of equations to check. Lets work the first set and see if we get any hints that will make checking the $5$ faster. We will solve the first equation for $A$ and substitute this into the second equation and solve for $B$

{% raw %}{::nomarkdown}<div>
$\begin{align*}
A + B &= 202 \rightarrow A = 202 - B \qquad\qquad (1)\\
A - B &= 10 \\
202 - B - B &= 10 \\
-2B &= 10 - 202 \\
-2B &= -192 \qquad\qquad\qquad\qquad\qquad\: (2)\\
B &= 96 \rightarrow A = 202 - 96 = 106 \\
\end{align*}$
</div>{:/}{% endraw %}

First, this is the solution we were given to begin with. Next, it becomes clear that in each subsequent pair of equations, we are going to end up with an expression of the form

$-2B = (\text{first constant}) - (\text{second constant})$

There can not be an integer solution to this set of equations unless the difference is *even*. So we can take a short cut and simply look at all the differences.

{% raw %}{::nomarkdown}<div>
$\begin{align*}
101 - 20 &= 81 \leftarrow \text{Not integer solutions}\\
404 - 5 &= 399 \leftarrow \text{Not integer solutions}\\
505 - 4 &= 501 \leftarrow \text{Not integer solutions}\\
1010 - 2 &= 1008 \leftarrow \textbf{VALID!}\\
\end{align*}$
</div>{:/}{% endraw %}

So there is one more solution to the problem. Looking back at $(1)$ and $(2)$, we can quickly solve to find

{% raw %}{::nomarkdown}<div>
$\begin{align*}
-2B &= -1008 \\
B &= 504 \rightarrow A = 1010 - 504 = 506 \\
\end{align*}$
</div>{:/}{% endraw %}

Therefore there are two different pairs of integers such that the difference of their squares is $2020$


{% raw %}{::nomarkdown}<div>
$\begin{align*}
2020 &= 106^{2} - 96^{2}\\
2020 &= 506^{2} - 504^{2}\\
\end{align*}$
</div>{:/}{% endraw %}

