# Interferometric Neural Networks (INNs)

All the results from these Notebooks are reported in the paper: <br>
__Arun Sehrawat, Interferometric Neural Networks, [arXiv:2310.16742](https://arxiv.org/abs/2310.16742) [quant-ph] (2023).__



**(1)** A Quadratic Unconstrained Binary Optimization (QUBO) problem is a combinatorial optimization problem specified by a real square matrix Q. 
In the attached Jupyter notebook __QUBO_with_INN__, we have generated two sets of (QUBO) instances, where the Q matrix sampled from a discrete uniform and the standard normal distributions.
Each set containing one thousand instances for 17  binary variables (qubits). 
For each problem instance, we obtained two solutions: (1) a global optimum solution through an exhaustive search over $2^{17}=131072$ possibilities and (2) a solution using our INN.
And, we obtained the gap between the two solutions. The INN consistently yields the global optimum, achieving a success rate of 95% and 89% for the uniform and normal distributions, respec-
tively. In both cases, the optimality gaps remain under 2%.

