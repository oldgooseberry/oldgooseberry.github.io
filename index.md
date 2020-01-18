---
layout:   page
title:    "Test math"
author:    Beelzebub
category:  misc
tags:      [test]
use_math:  true
nav_order: 2
---

# Math Test Page

This page was written to explore the process of using Markdown with [GitHub Pages](https://pages.github.com). This page will remain as playground to experiment with different issues which arise while attempting to write mathematics (via $LaTeX$) in Markdown on **GitHub**. Funtimes....

# Stupid simple $LaTeX$ tests

- A simple equation on its own line (centered normally).

   $$
	\begin{equation}
	x = \frac{-b \pm \sqrt{b^{2} - 4ac} }{2a} \label{eq_1}
	\end{equation}
	$$

   I refer you to equation \eqref{eq_1}.

- A series of equations which are aligned on the 

{% raw %}{::nomarkdown}
	<div>
   $$\begin{align}
x^{3} + 1 &= (x+1)(x^{2} - x + 1)\\
x^{5} + 1 &= (x+1)(x^{4} - x^{3} + x^{2} - x + 1)\\
x^{7} + 1 &= (x+1)(x^{6} - x^{5} + x^{4} - x^{3} + x^{2} - x + 1)\\
\vdots \\
x^{101} + 1 &= (x+1)(x^{100} - x^{99} + x^{98} - \ldots + x^{6} - x^{5} + x^{4} - x^{3} + x^{2} - x + 1)
\end{align}$$
	</div>
{:/}{% endraw %}

   **Well that does not work in this system. Suck-o**. <br/>
   If you write

  ```latex
   $$\begin{align*}
x^{3} + 1 &= (x+1)(x^{2} - x + 1)\\
x^{5} + 1 &= (x+1)(x^{4} - x^{3} + x^{2} - x + 1)\\
\end{align*}$$
x
```

   The `&` will break the $LaTeX$ rendering.

   **UPDATE**
   To solve this, wrap the code in

   ```text
\{\% raw %}{::nomarkdown}
    <div>
    $$
    $$
    </div>
{:/}\{\% endraw %}
```

   This is described [here](https://stackoverflow.com/questions/34227995/mathjax-being-parsed-with-jekyll)

- A more complex expression

   $$
\left( \sum_{k=1}^n a_k b_k \right)^2 \leq \left( \sum_{k=1}^n a_k^2 \right) \left( \sum_{k=1}^n b_k^2 \right)
$$

- **Greek**

   $$
\Gamma\ \Delta\ \Theta\ \Lambda\ \Xi\ \Pi\ \Sigma\ \Upsilon\ \Phi\ \Psi\ \Omega \\
\omicron\ \pi\ \rho\ \sigma\ \tau\ \upsilon\ \phi\ \chi\ \psi\ \omega\ \varepsilon\ \vartheta\ \varpi\ \varrho\ \varsigma\ \varphi \\
\alpha\ \beta\ \gamma\ \delta\ \epsilon\ \zeta\ \eta\ \theta\ \iota\ \kappa\ \lambda\ \mu\ \nu\ \xi\
$$

- An integral

   $$
f(x) = \int_{-\infty}^\infty \hat f(\xi)\,e^{2 \pi i \xi x}
$$

- A Vector equation

{% raw %}{::nomarkdown}
   <div>
   $$
\mathbf{V}_1 \times \mathbf{V}_2 =
\begin{vmatrix}
  \mathbf{i} & \mathbf{j} & \mathbf{k} \\
  \frac{\partial X}{\partial u} & \frac{\partial Y}{\partial u} & 0 \\
  \frac{\partial X}{\partial v} & \frac{\partial Y}{\partial v} & 0
\end{vmatrix}
$$
{:/}{% endraw %}

