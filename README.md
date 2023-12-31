# Interferometric Neural Networks (INNs)

All the results from the attached Notebooks are reported in the paper: 

__Arun Sehrawat, Interferometric Neural Networks, [arXiv:2310.16742](https://arxiv.org/abs/2310.16742) [quant-ph] (2023).__

-----

In this paper, we introduce INNs given below in hierarchical order. The top INN is made of INNs shown in the middle, and the middle INN is made of INNs shown at the bottom.

<img src="https://github.com/ArunSehrawat/Interferometric-Neural-Networks/assets/99533657/37f68450-fa8b-4896-9d4a-d3b71e24b347" width="400" height="250">

${}$

<img src="https://github.com/ArunSehrawat/Interferometric-Neural-Networks/assets/99533657/19d2f69b-8ea9-4cb1-aa5e-c7b7f333ed89" width="700" height="200">

${}$

![Int (copy)](https://github.com/ArunSehrawat/Interferometric-Neural-Networks/assets/99533657/7eb82607-150b-48be-a5b7-50f4d9155b14)

-----

**(1)** A Quadratic Unconstrained Binary Optimization (QUBO) problem is a combinatorial optimization problem specified by a real square matrix Q. 
In the Jupyter Notebook __QUBO_with_INN__, we have generated two sets of QUBO instances, where the Q matrix sampled from a discrete uniform and the standard normal distributions.
Each set containing one thousand instances for 17  binary variables (qubits). 
For each problem instance, we obtained two solutions: (1) a global optimum solution through an exhaustive search over $2^{17}=131072$ possibilities and (2) a solution using the the bottom INN.
And, we obtained the gap between the two solutions. The INN consistently yields the global optimum, achieving a success rate of 95% and 89% for the uniform and normal distributions, respectively. In both cases, the optimality gaps remain under 2%.

![opt_gap](https://github.com/ArunSehrawat/Interferometric-Neural-Networks/assets/99533657/3d1240e7-0281-4639-adbf-5cfca0a8f6f9)

-----

**(2)** In the Jupyter Notebook __Binary_Image_classification_with_INN__, we have employed the bottom INN for binary image classifications on the MNIST dataset. To create a 2-class classification problem, we gathered all the images of only two specific digits, denoted as $a$ and $b$, which are respectively labeled as the negative class and the positive class. After the training of the INN, we evaluate its performance by using
accuracy and $\text{f}_1$ scores on the test set. The results are obtained for every $a,b=0,\cdots,9$ provided $a\neq b$.

![acc_mat](https://github.com/ArunSehrawat/Interferometric-Neural-Networks/assets/99533657/7e13bd3e-c535-46e0-a676-b8d485ad66b8)
![f1_mat](https://github.com/ArunSehrawat/Interferometric-Neural-Networks/assets/99533657/9e56aefc-6eda-4b27-b801-e54324b8bee7)

-----

**(3)** In the Jupyter Notebook __Image_classification_with_INN__, we have employed the top INN for image classification on both the MNIST and FashionMNIST datasets, each with $C=10$ classes.
As we increase the number of layers, the performance---measured by the accuracy and average $\text{f}_1$---of the INN improves for both datasets.
In summary, we have attained accuracies and average $\text{f}_1$ scores of 93% and 83% on the MNIST and FashionMNIST datasets, respectively.

![acc_f1](https://github.com/ArunSehrawat/Interferometric-Neural-Networks/assets/99533657/557633ea-27f9-4cb1-b93a-b58057af3651)

-----

**(4)** In the paper, we also introduced IGANs, made of the top INNs, for image generation. 
Separate IGANs were trained on the MNIST dataset and CelebA datasets. 
Their complete implementation is given in the notebook __IGAN__. 
These IGANs have successfully generated images of 0 to 9 digits and human faces.

![faces](https://github.com/ArunSehrawat/Interferometric-Neural-Networks/assets/99533657/4482d8e2-e7b2-45ba-819e-70b4ebb498bc)








