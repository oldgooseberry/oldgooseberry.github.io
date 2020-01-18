---
layout:       page
title:        "Soln 2020-01 #5b"
author:       Beelzebub
category:     [Questions Jan2020]
use_math:     true
nav_order:    2
parent:       Jan 2020
grand_parent: Solutions To Questions
---

# Question

What is $7^{40895} \text{mod} 30$ ?

# Solution

$$7^{40895} \: mod \: 30 = \text{?}$$

## Solution

We are looking for a pattern (cycle) for powers of $7$ mod $30$. Or at least we hope to find one. This would greatly simplify finding the $40895^{\text{th}}$ power of anything. We begin by looking at the first $10$ powers of $7$ mod $30$. Here is some `julia` code to do just that

```julia
julia> for i in 1:10
       println("$(BigInt(7)^i)")
       end
7
49
343
2401
16807
117649
823543
5764801
40353607
282475249

julia> for i in 1:10
       println("$(BigInt(7)^i % 30)")
       end
7
19
13
1
7
19
13
1
7
19
```

As we can see, there is a cycle $\lbrace 7,19,13,1 \rbrace$ of length $4$. We need only figure out the easier problem $$40895 \: mod \: 4 \equiv \text{?}$$ But this is

```julia
julia> 40895 % 4
3
```

Therefore $7^{40895} \: mod \: 30 = 13$ or the third element of the cycle $ \lbrace 7,19,13,1 \rbrace$ 

