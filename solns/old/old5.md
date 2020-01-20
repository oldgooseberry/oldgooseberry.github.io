---
layout:       page
title:        "Soln 2020-01 #5"
author:       Beelzebub
category:     [Questions Jan2020]
use_math:     true
nav_order:    1
parent:       Problems From the Past
grand_parent: Solutions To Questions
---

# Question

The average Thanksgiving dinner weights about 1 kg and contains 3200 kcal, which is about 1200 kcal above our (average) daily requirement.

If the specific heat of food is about 1 $\frac{\text{kcal}}{\text{kg°C}}$, how cold would we have to make our food in order to completely expend the excess calories in heatin   g the food to body temperature?

# Solution

Clearly this was given as a funny problem, but lets work through it. If we think back, we might remember the governing equation for heat we are looking for, that is

$\text{Q} = \text{m} \text{c} \Delta T$

Where

{% raw %}{::nomarkdown}<div>
$\begin{align*}
\text{Q} &= \text{The heat lost or gained, usually measured in kcal} \\
\text{m} &= \text{The mass which is under going the heat loss or gain, usually in kg} \\
\text{c} &= \text{The sqpcific heat of the mass, in} \frac{\text{kcal}}{\text{kg°C}} \\
\Delta T &= \text{The change in temperature of the mass} \\
\end{align*}$
</div>{:/}{% endraw %}

If we then extract from the problem the key values we are given, we have

{% raw %}{::nomarkdown}<div>
$\begin{align*}
\text{Q} &= 1200 \text{kcal} \\
\text{m} &= 1 \text{kg} \\
\text{c} &= 1  \frac{\text{kcal}}{\text{kg°C}} \\
\Delta T &= \bf{UNKNOWN} \\
\end{align*}$
</div>{:/}{% endraw %}

We want then want to solve for $\Delta T$. Doing this we get

{% raw %}{::nomarkdown}<div>
$\begin{align*}
1200 &= (1)(1)\Delta T \\
\Delta T &= 1200
\end{align*}$
</div>{:/}{% endraw %}

Looking at the units, this is $1200 \text{°C}$. So we need to have the food at a temperature which can raised $1200 \text{°C}$ to body temperature ($36.5 \text{°C}$ for an average human) and thus consume the extra $1200$ cal from us. Therefore, we are asking to solve the equation


{% raw %}{::nomarkdown}<div>
$\begin{align*}
\Delta T &= T_{\text{final}} - T_{\text{initial}} = 1200 \\
1200 &= T_{\text{body}} - T_{\text{initial}} \\
1200 &= 36.5 - T_{\text{initial}} \\
T_{\text{initial}} &= 36.5 - 1200 = -1163.5 \\
\end{align*}$
</div>{:/}{% endraw %}

Not only is this a silly number, but *Absolute Zero* is **only** $-273.15\text{°C}$. Therefore, it is not even physically possible.


