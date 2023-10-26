# Interferometric Neural Networks (INNs)

All the results from these Notebooks are reported in the paper: <br>
__Arun Sehrawat, Interferometric Neural Networks, [arXiv:2310.16742](https://arxiv.org/abs/2310.16742) [quant-ph] (2023).__

In this paper, we introduce INNs given below in hierarchical order. The top INN is made of the middle one, which is composed of the bottom INN.

<img src="https://github.com/ArunSehrawat/Interferometric-Neural-Networks/assets/99533657/37f68450-fa8b-4896-9d4a-d3b71e24b347" width="400" height="250">

${}$

<img src="https://github.com/ArunSehrawat/Interferometric-Neural-Networks/assets/99533657/19d2f69b-8ea9-4cb1-aa5e-c7b7f333ed89" width="1000" height="400">

![Int_Blk](https://github.com/ArunSehrawat/Interferometric-Neural-Networks/assets/99533657/19d2f69b-8ea9-4cb1-aa5e-c7b7f333ed89)

${}$

![Int (copy)](https://github.com/ArunSehrawat/Interferometric-Neural-Networks/assets/99533657/7eb82607-150b-48be-a5b7-50f4d9155b14)


-----

**(1)** A Quadratic Unconstrained Binary Optimization (QUBO) problem is a combinatorial optimization problem specified by a real square matrix Q. 
In the attached Jupyter notebook __QUBO_with_INN__, we have generated two sets of QUBO instances, where the Q matrix sampled from a discrete uniform and the standard normal distributions.
Each set containing one thousand instances for 17  binary variables (qubits). 
For each problem instance, we obtained two solutions: (1) a global optimum solution through an exhaustive search over $2^{17}=131072$ possibilities and (2) a solution using our INN.
And, we obtained the gap between the two solutions. The INN consistently yields the global optimum, achieving a success rate of 95% and 89% for the uniform and normal distributions, respec-
tively. In both cases, the optimality gaps remain under 2%.

![opt_gap](https://github.com/ArunSehrawat/Interferometric-Neural-Networks/assets/99533657/3d1240e7-0281-4639-adbf-5cfca0a8f6f9)

-----


**(2)** 
