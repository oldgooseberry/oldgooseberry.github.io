---
layout:       page
title:        "Soln 2020-01 #6b"
author:       Beelzebub
category:     [Questions Jan2020]
use_math:     true
nav_order:    2
parent:       Jan 2020
grand_parent: Solutions To Questions
---

# Question

Given the unbalanced chemical reaction (Rocket Fuel)

$ \ce{Al + NH4ClO4 \rightarrow Al2O3 + AlCl3 + N2 + H2O} $

If the molar mass of $\ce{Al}$ is $\frac{1}{4}$ the molar mass of $\ce{NH4ClO4}$, what percent of the propellan should be $\ce{Al}$ by mass?

# Solution

We begin by trying to balance this chemical equation first. To do that, we introduce some unknowns and re-write the equation as

$ \ce{\alpha_{1}Al + \alpha_{2}NH4ClO4 \rightarrow \alpha_{3}Al2O3 + \alpha_{4}AlCl3 + \alpha_{5}N2 + \alpha_{6}H2O} $

Then we can express each of the elements as equations to balance in the following way

{% raw %}{::nomarkdown}<div>
$\begin{align*}
\ce{Al}&: \alpha_{1} = 2 \alpha_{3} + \alpha_{4} \\
\ce{N}&:  \alpha_{2} = 2 \alpha_{5} \\
\ce{H}&:  4 \alpha_{2} = 2 \alpha_{6} \\
\ce{Cl}&: \alpha_{2} = 3 \alpha_{4} \\
\ce{O}&: 4 \alpha_{2} = 3 \alpha_{3} + \alpha_{6} \\
\end{align*}$
</div>{:/}{% endraw %}

If we let $\alpha_{2} = 1$ then we can solve for all other variables

 {% raw %}{::nomarkdown}<div>
$\begin{align*}
1 &= 2 \alpha_{5} \rightarrow \alpha_{5} = \frac{1}{2}\\
4 &= 2 \alpha_{6} \rightarrow \alpha_{6} = 2 \\
1 &= 3 \alpha_{4} \rightarrow \alpha_{4} = \frac{1}{3}\\
4 &= 3 \alpha_{3} + \alpha_{6} = 3 \alpha_{3} + 2 \rightarrow \alpha_{3} = \frac{2}{3}\\
\alpha_{1} &= 2  \frac{2}{3} + \frac{1}{3} = \frac{5}{3} \\
\end{align*}$
</div>{:/}{% endraw %}

So our equation now looks like

$ \ce{\frac{5}{3}Al + NH4ClO4 \rightarrow \frac{2}{3}Al2O3 + \frac{1}{3}AlCl3 + \frac{1}{2}N2 + 2H2O} $

But, we want the equation to be in integer amounts of the reactants, therefore we multiple by $6$. This gives us the balanced equation 

$ \ce{10Al + 6NH4ClO4 \rightarrow 4Al2O3 + 2AlCl3 + 3N2 + 12H2O} $ 

So the molecular ratio of $\ce{Al}$ to $\ce{NH4ClO4}$ is $10:6$. However, we are told the mass of $\ce{Al}$ is $\frac{1}{4}$ $\ce{NH4ClO4}$. Therefore, our mass ratio is $10:24$. Given this, the percent of the propellan by mass of $\ce{Al}$ should be 

$\frac{10}{10+24} = \frac{10}{34} \approx 30\%$


