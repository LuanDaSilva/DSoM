# DSoM
Implementation of Dirichlet Sampling on Manifolds. A method created by Luan da Silva

This code is related to a method called Dirichlet Sampling on Manifolds (DSoM) that allows sampling points around a manifold. Some reference data are needed, which can be obtained directly from a physical system, or generated with high fidelity computational models. The probability distribution of the original data is unknown. DSoM generates new data that respect the underlying manifold around which the original data were observed. This can be very helpful, for instance, in neural networks training process, as well as in uncertainty analysis and stochastic optimization. 

Please cite as: L.S. Prado and T.G. Ritto, Data driven Dirichlet sampling on manifolds, Arxiv:2101.00947; https://arxiv.org/abs/2101.00947v1

The steps of DSoM to generate a new sample point from the original data (N) are the following.
(i) K points (K<N) of the original data are randomly selected
(ii) the parameters of the Dirichlet distribution are obtained
(iv) some data points are generated using the Dirichlet distribution
(v) a convex combination is considered to generate one new sample

The details can be found in L.S. Prado and T.G. Ritto (2020), and in the code. 
