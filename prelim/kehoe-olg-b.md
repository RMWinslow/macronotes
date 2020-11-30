---
title: "Part b) SM-Equilibrium" 
parent: OLG - Pareto Efficiency
grand_parent: Past Prelims
---


$$ x^2 \tag{Do tags even work?}$$

# Pareto efficiency in an overlapping generations economy

## Part b) Sequential Markets Equilibrium

Define a Sequential Markets equilibrium for this economy. 
Calculate the unique Sequential Markets equilibrium.

Click to expand solutions.

<details markdown="block"><summary>Define a Sequential Markets equilibrium for this economy.</summary>

A Sequential Markets Equilibrium consists of:

- a sequence of allocations: $$\{ (\tilde{c}^t_t, \tilde{c}^t_{t+1}, \tilde{s}_{t+1}) \}_{t=1}^\infty$$
- an allocation for generation $0$: $$\{ \tilde{c}_1^0 \}$$
- and a sequence of prices: $$\{ \tilde{r}_{t+1} \}_{t=1}^\infty$$

such that the following conditions are satisfied:

### Gen 0 Consumer Optimization:
Taking prices as given, consumer $0$ chooses $\tilde{c}_1^0$ to solve 

$$\max_{c_1^0} \; \ln c_1^0$$

*subject to the constraints:*

$$c_{1}^{0}\geq0 \mytag{Non-neg}$$

$$c_{1}^{0}\leq w_{1}^{0}  \mytag{Budget}$$


### Gen t Consumer Optimization:
Taking prices as given, each consumer $t,t=1,2,...$ chooses $(\tilde{c}^t_t, \tilde{c}^t_{t+1}, \tilde{s}_{t+1})$ to solve

$$\max_{c^t_t, c^t_{t+1}, s_{t+1}^t} \; \ln (c_t^t) + c_{t+1}^t$$

*subject to the constraints:*

$$c_{t}^{t}\geq0 \;\; c_{t+1}^{t}\geq0 \mytag{Non-neg}$$

$$c_{t}^{t}+s_{t+1}^{t}\leq w_{t}^{t}  \mytag{Budget Young}$$

$$c_{t+1}^{t} \leq w_{t}^{t+1} + (1+\tilde{r}_{t+1}) s_{t+1}^t  \mytag{Budget Old}$$


### Markets Clear: 
For all $t=1,2,...$:

$$\mytag{Goods MC}  \tilde{c}_t^{t-1} + \tilde{c}_t^t = w_t^{t-1} + w_t^t$$

$$\mytag{Credit MC}  \tilde{b}_t = 0$$


</details>








<details open markdown="block"><summary>Calculate the unique Sequential Markets equilibrium.</summary>


The unique Sequential Markets equilibrium has each consumer consume their endowments and save nothing. $$\tilde{c}_0^1 = w_1^0$$. And for all$$t=1,2,3,...$$, $$\tilde{c}_t^t = w_t^t$$, $$\tilde{c}_{t+1}^t = w_{t+1}^t$$, $$s_{t+1}^t = 0$$. 

And $\tilde{r}_{t+1} = \frac{1}{c_t^t} - 1$.

<details  open markdown="block"><summary>Explanation and Proof</summary>

### Equilibrium allocations are Autarky

1. First note that every generation has strictly increasing utility and so every budget constraint will hold with equality.
2. The credit market clearing constraint implies that all savings are zero.
3. With zero savings, each generations budget constraints imply the result.

### Finding the equilibrium prices

Combine budgets into a single intertemporal budget constraint:

$${c}_t^t + \frac{{c}_{t+1}^t}{1+r} = {w}_t^t + \frac{{w}_{t+1}^t}{1+r}$$

Set up the Lagrangian for generation $t$'s problem:

$$\mathcal{L} = \ln(c_t^t) + c_{t+1}^t - \lambda\cdot\left[ {c}_t^t + \frac{{c}_{t+1}^t}{1+r} - {w}_t^t - \frac{{w}_{t+1}^t}{1+r} \right]$$


</details>

</details>





[Previous](kehoe-olg-a)
{: .float-left }

[Next](kehoe-olg-c)
{: .float-right }
