---
title: "Part (a) AD-Equilibrium" 
parent: OLG - Pareto Efficiency
grand_parent: Past Prelims
---

# Pareto efficiency in an overlapping generations economy

## Part a) Arrow-Debreu Equilibrium

Define an Arrow-Debreu equilibrium for this economy. 
Calculate the unique Arrow-Debreu equilibrium.


<details markdown="block">
<summary>
Define an Arrow-Debreu equilibrium for this economy.
</summary>

An Arrow-Debreu Equilibrium consists of:

- a sequence of allocations: $$\{ (\hat{c^t_t}, \hat{c^t_{t+1}}) \}_{t=1}^\infty$$
- an allocation for generation $0$: $$\{ \hat{c_1^0} \}$$
- and a sequence of prices: $$\{ \hat{p_t} \}_{t=1}^\infty$$

such that the following conditions are satisfied:

### **Consumer Optimization:** 
Taking prices as given, consumer $0$ chooses $\hat{c_1^0}$ to solve 

$$\begin{aligned} & \underset{c_{1}^{0}}{\text{maximize}} &  & \ln c_1^0\\
 & \text{subject to}: &  & c_{1}^{0}\geq0\\
 &  &  & \hat{p}_{1}c_{1}^{0}\leq\hat{p}_{1}w_{1}^{0}
\end{aligned}
$$

$$&\max_{c_{1}^{0}}&&\ln\left(c_{1}^{0}\right)\\&\text{s.t.}&&c_{1}^{0}\geq0\\&&&\hat{p}_{1}c_{1}^{0}\leq\hat{p}_{1}w_{1}^{0}$$

$$\max_{c_{1}^{0}}&&&\ln\left(c_{1}^{0}\right)\\\text{s.t.}&&&c_{1}^{0}\geq0\\&&&\hat{p}_{1}c_{1}^{0}\leq\hat{p}_{1}w_{1}^{0}$$

### **Consumer Optimization:** 
Taking prices as given, consumer $0$ chooses $\hat{c_1^0}$ to solve \\[\max_{c_1^0} \ln (c_1^0) \\] s.t. 

$$\begin{gather}
c_1^0 \geq 0 \tag{non-negativity} \\
x^2\\
\end{gather}$$

$$\begin{aligned} & \underset{c_{1}^{0}}{\text{maximize}} &  & \ln c_1^0\\
 & \text{subject to}: &  & c_{1}^{0}\geq0\\
 &  &  & \hat{p}_{1}c_{1}^{0}\leq\hat{p}_{1}w_{1}^{0}
\end{aligned}
$$

$$&\max_{c_{1}^{0}}&&\ln\left(c_{1}^{0}\right)\\&\text{s.t.}&&c_{1}^{0}\geq0\\&&&\hat{p}_{1}c_{1}^{0}\leq\hat{p}_{1}w_{1}^{0}$$

$$\max_{c_{1}^{0}}&&&\ln\left(c_{1}^{0}\right)\\\text{s.t.}&&&c_{1}^{0}\geq0\\&&&\hat{p}_{1}c_{1}^{0}\leq\hat{p}_{1}w_{1}^{0}$$



### **Consumer Optimization:** 
Taking prices as given, consumer $t,t=1,2,...$ chooses $(\hat{c^t_t}, \hat{c^t_{t+1}})$ to solve

$$\begin{aligned} & \underset{c^t_t, c^t_{t+1}}{\text{maximize}} &  & \ln (c_t^t) + c_{t+1}^t\\
 & \text{subject to}: &  & c_{1}^{0}\geq0\\
 &  &  & \hat{p}_{1}c_{1}^{0}\leq\hat{p}_{1}w_{1}^{0}
\end{aligned}
$$

$$\begin{aligned} & \underset{c^t_t, c^t_{t+1}}{\text{maximize}} &  & \ln (c_t^t) + c_{t+1}^t\\
 & \text{s.t.}: &  & c_{1}^{0}\geq0\\
 &  &  & \hat{p}_{1}c_{1}^{0}\leq\hat{p}_{1}w_{1}^{0}
\end{aligned}
$$



### **Markets Clear:** 
For all $t=1,2,...$:

$$\hat{c}_t^{t-1} + \hat{c}_t^t = w_2 + w_1 $$


</details>








<details markdown="block"><summary>Calculate the unique Arrow-Debreu equilibrium.</summary>

The unique Arrow-Debreu equilibrium has each consumer consume their endowments. $\hat{c}_0^1 = w_1^0$. And for all $t=1,2,3,...$, $\hat{c}_t^t = w_t^t$, $\hat{c}_{t+1}^t = w_{t+1}^t$. 

If we normalize $\hat{p}_1 = 1$, then  $\hat{p}_t = \hat{p}_1 \cdot 2^{t-1}$,

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

$$\mathcal{L} = \ln(c_t^t) + c_{t+1}^t$$

First-order conditions:

$$\begin{align}
    0 &= \frac{1}{c_t^t} - \lambda_t p_t \\
    0 &= 1 - \lambda_t p_{t+1} \\
    p_t c_t^t + p_{t+1} c_{t+1}^t &= w_t^t + w_{t+1}^t\\
\end{align}$$

Combine the first two to get that $\frac{1}{c_t^t} = \frac{p_t}{p_{t+1}}$. Plug in the fact that $c_t^t = w_t^t = 2$ to get the result that $p_{t+1} = 2\cdot p_t$.


</details>
</details>







[Previous](kehoe-olg)
{: .float-left }

[Next](kehoe-olg-b)
{: .float-right }
