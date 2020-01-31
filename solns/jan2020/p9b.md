---
layout:       page
title:        "Soln 2020-01 #9b"
author:       Beelzebub
category:     [Questions Jan2020]
use_math:     true
nav_order:    2
parent:       Jan 2020
grand_parent: Solutions To Questions
---

# Question

You have one more small ornament to hang on the mobile shown below

![mobile](/img/jan2020/balance1.png)

[A larger image for printing](/img/jan2020/balance1.jpeg)

After you place it, the mobile should be perfectly balanced at all levels. How many possible places can you put it?

# Solution

If one works through the mobile using force $\times$ distance, one finds the original mobile is in balance. Therefore, we can not add any weights to the lower left bar, as we have only one slot and it would be out of balance. Similarly, we can not add one to the lower right bar. And by similar arguments, no weights can be added to the middle bars and the top bar. This leaves us with attempts to add weights where the stings attach. We can do this on the top bar, so **one**. If we try this on the middle bars, they will not balance as the torque on the right side would be

$1 \times 4 = 4$

but the torque on the left would be

$1 \times 1 = 1$

so out of balance. If we try this with the lowest bars, the same unbalanced behavior will occur. Thus, we can only place one more and it must be placed under the string which holds the top bar.

 
![mobile](/img/jan2020/balance1_soln.png)

[A larger image for printing](/img/jan2020/balance1_soln.jpeg)

