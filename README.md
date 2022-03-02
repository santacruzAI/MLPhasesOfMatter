# Machine Learning Phases of Matter (Carasquilla, Meiko) - Implementation/Extensions 
Giridhar Vadhul, Pranav Vempati

This Github Repository implements Juan Carasquilla and Roger Melko's 2016 Paper, Machine Learning Phases of Matter (https://arxiv.org/abs/1605.01735).

We implement the Metropolis-Hastings algorithm to simulate 4 Ising Models, namely the Square/Triangular Lattices, Square Ice Lattice and an Ising Gauge Theory-based Lattice. The visualizations of these evolution processes are given below:



Further, we train a Feedforward Neural Network to classify the phases of sample square lattices upto 99.4% test accuracy. This is surprising achievement in itself, given that, as visible in the visualizations, the difference between high and low temperature lattices is very subtle and not humanly-visible. 

We then devise a method to simulate Triangular Lattices. After various experiments with methods of blocking out parts of square lattices to generate a triangular shape, but eventually decided to simulate this through a visualization technique that shifts lattice rows. We further show that this network generalizes with high accuracy to a triangular lattice with a different Hamiltonian. (IN PROGRESS)

The Ising Gauge Theory-based Lattice is a Topological Phase of Matter and naturally it is of great interest how an order parameter of it is inferred. We implement the Hamiltonian ( ), where p is a plaquette, the smallest closed shape within the lattice (in this case a square one), and use the MCMC method Metropolis-Hastings to synthesize such samples. 

We further implement a feedforward neural network and show that it performs near chance on the Topological Phase. As a result, we then show that a Convolutional Neural Network achieves close to 100% test accuracy. (IN PROGRESS)

Finally, we intend to synthesize Square Ice Lattices and demonstrate that a Feedforward Neural Network performs highly here, and then work on further extensions to this approach to generalize well across diverse lattices.

References:

Paper: @article{2017,
   title={Machine learning phases of matter},
   volume={13},
   ISSN={1745-2481},
   url={http://dx.doi.org/10.1038/nphys4035},
   DOI={10.1038/nphys4035},
   number={5},
   journal={Nature Physics},
   publisher={Springer Science and Business Media LLC},
   author={Carrasquilla, Juan and Melko, Roger G.},
   year={2017},
   month={Feb},
   pages={431–434} }

Special Thanks to jsr66's repository: https://github.com/jsr66/Machine-Learning-Phases-of-Matter-with-Discriminative-Localization, which implements part of this paper, and inspired our approach to the Metropolis-Hastings simulation.
