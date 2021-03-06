---
title: "Part a) AD-Equilibrium" 
parent: OLG - Pareto Efficiency
grand_parent: Past Prelims
---

# Pareto efficiency in an overlapping generations economy

Consider an overlapping generations economy in which there is one good in each period
and each generation, except the initial one, lives for two periods. The representative
consumer in generation $t, t = 1,2,...,$ has the utility function

$$\ln (c_t^t) + c_{t+1}^t$$

and the endowment $(w_t^t, w_{t+1}^t)=(1,2)$.
The representative consumer in generation $0$ lives only in period $1$,
prefers more consumption to less, and has the endowment $w_1^0 = 2$




## Part a) Arrow-Debreu Equilibrium

Define an Arrow-Debreu equilibrium for this economy. 
Calculate the unique Arrow-Debreu equilibrium.


<details markdown="block">
<summary>
Define an Arrow-Debreu equilibrium for this economy.
</summary>

An Arrow-Debreu Equilibrium consists of:

- a sequence of allocations: $$\{ (\hat{c}^t_t, \hat{c}^t_{t+1}) \}_{t=1}^\infty$$
- an allocation for generation $0$: $$\{ \hat{c}_1^0 \}$$
- and a sequence of prices: $$\{ \hat{p}_t \}_{t=1}^\infty$$

such that the following conditions are satisfied:

### Gen 0 Consumer Optimization:
Taking prices as given, consumer $0$ chooses $\hat{c}_1^0$ to solve 

$$\max_{c_1^0} \; \ln c_1^0$$

*subject to the constraints:*

$$c_{1}^{0}\geq0 \mytag{Non-neg}$$

$$\hat{p}_{1}c_{1}^{0}\leq\hat{p}_{1}w_{1}^{0}  \mytag{Budget}$$


### Gen t Consumer Optimization:
Taking prices as given, each consumer $t,t=1,2,...$ chooses $(\hat{c}^t_t, \hat{c}^t_{t+1})$ to solve

$$\max_{c^t_t, c^t_{t+1}} \; \ln (c_t^t) + c_{t+1}^t$$

*subject to the constraints:*

$$c_{t}^{t}\geq0 \;\; c_{t+1}^{t}\geq0 \mytag{Non-neg}$$

$$\hat{p}_{t}c_{t}^{t}+\hat{p}_{t+1}c_{t+1}^{t}\leq\hat{p}_{t}w_{t}^{t}+\hat{p}_{t+1}w_{t}^{t+1}  \mytag{Budget}$$



### Markets Clear: 
For all $t=1,2,...$:

$$\mytag{Goods MC}  \hat{c}_t^{t-1} + \hat{c}_t^t = w_t^{t-1} + w_t^t$$


</details>








<details markdown="block"><summary>Calculate the unique Arrow-Debreu equilibrium.</summary>

The unique Arrow-Debreu equilibrium has each consumer consume their endowments.
$$\hat{c}_0^1 = w_1^0$$. 
And for all$$t=1,2,3,...$$, 
$$\hat{c}_t^t = w_t^t$$, 
$$\hat{c}_{t+1}^t = w_{t+1}^t$$. 

If we normalize $\hat{p}_1 = 1$, then  $\hat{p}_t = \hat{p}_1 \cdot 2^{t-1}$.

<details markdown="block"><summary>Explanation and Proof</summary>

### Equilibrium allocations are Autarky

1. First note that every generation has strictly increasing utility and so every budget constraint will hold with equality.
2. Generation $0$'s budget constraint implies that $\hat{c}_1^0 = w_1^0$
3. Plug this into the period $1$ market clearing condition $\hat{c}_1^{0} + \hat{c}_1^1 = w_1^1 + w_1^0$ to get that $\hat{c}_1^1 = w_1^1$.
4. Plug this into generation $1$'s budget constraint to get that $\hat{c}_2^1 = w_2^1$.
5. Plug this into the period $2$ market clearing condition to get that to get that $\hat{c}_2^2 = w_2^2$.
6. Iterate for all generations.

### Finding the equilibrium prices

Set up the Lagrangian for generation $t$'s problem:

$$\mathcal{L} = \ln(c_t^t) + c_{t+1}^t - \lambda\cdot\left[ p_t c_t^t + p_{t+1} c_{t+1} - p_t w_t^t - p_{t+1} w_{t+1}^t \right]$$

First-order conditions:

$$\begin{aligned}
    0 &= \frac{1}{c_t^t} - \lambda_t p_t \\
    0 &= 1 - \lambda_t p_{t+1} \\
    p_t c_t^t + p_{t+1} c_{t+1}^t &= w_t^t + w_{t+1}^t\\
\end{aligned}$$

Combine the first two to get that $\frac{1}{c_t^t} = \frac{p_t}{p_{t+1}}$. Plug in the fact that $c_t^t = w_t^t = 2$ to get the result that $p_{t+1} = 2\cdot p_t$.

With any other price ratio, the generation $t$ consumer would choose a non-autarky allocation.

So for all the equilibrium conditions to hold, it must be that $\hat{p}_{t+1} = 2\cdot \hat{p}_t$ for all $t=1,2,...$, and so $\hat{p}_t = \hat{p}_1 \cdot 2^{t-1}$


</details>

</details>







[Previous](kehoe-olg)
{: .float-left }

[Next](kehoe-olg-b)
{: .float-right }
