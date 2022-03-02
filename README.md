# Machine Learning Phases of Matter (Carasquilla, Meiko) - Implementation/Extensions 
**Giridhar Vadhul (Advanced Track), Pranav Vempati (SCAI President)**

_This Github Repository implements Juan Carasquilla and Roger Melko's 2016 Paper, Machine Learning Phases of Matter (https://arxiv.org/abs/1605.01735).

**Visualizations: **

We implement the Metropolis-Hastings algorithm to simulate 4 Ising Models, namely the Square/Triangular Lattices, Square Ice Lattice and an Ising Gauge Theory-based Lattice. The visualizations of these evolution processes are given below:

**Square Lattice:**
    **High Temperature Simulation: **
    
    **Low Temperature Simulation: **

**Triangular Lattice:**
  **High Temperature Simulation: **
    
  **Low Temperature Simulation: **

**Topological Phases:**

**Square Ice Lattice:**

Further, we train a Feedforward Neural Network to classify the phases of sample square lattices upto 99.4% test accuracy. This is surprising achievement in itself, given that, as visible in the visualizations, the difference between high and low temperature lattices is very subtle and not humanly-visible. 

We then devise a method to simulate Triangular Lattices. After various experiments with methods of blocking out parts of square lattices to generate a triangular shape, but eventually decided to simulate this through a visualization technique that shifts lattice rows. We further show that this network generalizes with high accuracy to a triangular lattice with a different Hamiltonian. (IN PROGRESS)

The Ising Gauge Theory-based Lattice is a Topological Phase of Matter and naturally it is of great interest how an order parameter of it is inferred. We implement the Hamiltonian ( ), where p is a plaquette, the smallest closed shape within the lattice (in this case a square one), and use the MCMC method Metropolis-Hastings to synthesize such samples. 

We further implement a feedforward neural network and show that it performs near chance on the Topological Phase. As a result, we then show that a Convolutional Neural Network achieves close to 100% test accuracy. (IN PROGRESS)

Finally, we intend to synthesize Square Ice Lattices and demonstrate that a Feedforward Neural Network performs highly here, and then work on further extensions to this approach to generalize well across diverse lattices.

References:

Paper: arXiv:1605.01735 [cond-mat.str-el]

Special Thanks to jsr66's repository: https://github.com/jsr66/Machine-Learning-Phases-of-Matter-with-Discriminative-Localization, which implements part of this paper, and inspired our approach to the Metropolis-Hastings simulation.
