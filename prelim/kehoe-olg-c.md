---
title: "Part c) Pareto Efficiency" 
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

## Part c) Pareto Efficiency

Define a Pareto efficient allocation.
Either prove that the equilibrium allocation in part a is Pareto efficient or prove that it is not.


<details markdown="block"><summary>Define a Pareto efficient allocation.</summary>

An allocation is *Pareto Efficient* if it is feasible and there is no alternative feasible outcome which makes at least one generation better off and no generations worse off.

### Feasible Allocation

To be Pareto efficient, an allocation $$\{c_t^t, c_{t+1}^t\}_{t=0}^\infty, \{c_1^0\}$$ must be feasible, meaning that for all $t=1,2,...$:

$$c_t^t + c_t^{t-1} = w_t^t + w_t^{t-1}$$

$$c_t^t \geq 0$$

$$c_t^{t-1} \geq 0$$

### No feasible Pareto improvments


</details>





<details markdown="block"><summary>Either prove that the equilibrium allocation in part a is Pareto efficient or prove that it is not.</summary>


</details>
---


Now suppose that $(w_t^t, w_{t+1}^t)=(2,2)$. And that generation $0$ has endowment $w_1^0 = 2$.

With these new endowments, either prove that the Arrow-Debreu equilibrium is Pareto Efficient or prove that it is not. 


<details markdown="block"><summary>Either prove that the AD-equilibrium allocation is Pareto efficient or prove that it is not.</summary>

The Arrow-Debreu equilibrium (which in this economy is autarky) is not Pareto Efficient. 

<details markdown="block"><summary>Proof by counterexample.</summary>

Let $\dot{c}_t^t = 1$ and $\dot{c}_{t+1}^t = 3$ for all $t=1,2,3,...$

Clearly, this alternate allocation is still feasible. 

Generation $0$ is strictly better off with $3$ units instead of their endowment of $2$.

And all other generations are strictly better off as well, because $\ln 1 + 3 > \ln 2 + 2$

</details>
</details>



[Previous](kehoe-olg-b)
{: .float-left }

[Next](kehoe-olg-d)
{: .float-right }
