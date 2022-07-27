# Machine Learning Phases of Matter (Carasquilla, Melko) - Implementation/Extensions 
## **Giridhar Vadhul (Advanced Track), Pranav Vempati (SCAI President)**

_This Github Repository implements Juan Carasquilla and Roger Melko's 2016 Paper, 'Machine Learning Phases of Matter' (https://arxiv.org/abs/1605.01735)._

## **Visualizations:** (*Ongoing*)

We implement the Metropolis-Hastings algorithm to simulate 4 Ising Models, namely the Square/Triangular Lattices, Square Ice Lattice and an Ising Gauge Theory-based Lattice. The visualizations of these evolution processes are stored in the videos folder.

## **Implementation:**

Further, we train a Feedforward Neural Network to classify the phases of sample square lattices. This is surprising achievement in itself, given that, as visible in the visualizations, the difference between high and low temperature lattices is very subtle and not humanly-visible. 

We then devise a method to simulate Triangular Lattices. We further show that this network generalizes with high accuracy to this triangular lattice with a different Hamiltonian. (IN PROGRESS)

The Ising Gauge Theory-based Lattice is a Topological Phase of Matter and naturally it is of great interest how an order parameter of it is inferred. We implement the Hamiltonian, involving plaquettes p, the smallest closed shape within the lattice (in this case a square one), and use the MCMC method Metropolis-Hastings to synthesize such samples. 

We further implement a feedforward neural network and show that it performs near chance on the Topological Phase. As a result, we then show that a Convolutional Neural Network achieves high accuracy.

In addition to the above, we implement the Toy Models found in Appendices A and C respectively. In the former case, we validate the paper's premise that a neural network can both effectively encode and learn the magnetization of Ising Model configurations.  

Finally, we intend to synthesize Square Ice Lattices and demonstrate that a Feedforward Neural Network performs highly here, and then work on further extensions to this approach to generalize well across diverse lattices.

## **Understanding the data:**

In the process of implementing Appendix B, the high-dimensional clusters present in Appendix A's training data(and the associate decision boundary) is visualized by means of T-SNE in 2 dimensions. We employ sklearn.manifold's TSNE in conjunction with pyplot.scatter for this task. 



## **References:**

Paper: arXiv:1605.01735 [cond-mat.str-el]

Special Thanks to jsr66's repository: https://github.com/jsr66/Machine-Learning-Phases-of-Matter-with-Discriminative-Localization, which implements part of this paper, and inspired our approach to the Metropolis-Hastings simulation. 

Mr.P Solver's tutorial on simulating the Ising Model in Python: https://www.youtube.com/watch?v=K--1hlv9yv0 which inspired our approach to function formatting in our data generation process.

SCAI Tutorial Notebook on Deep Neural Networks in PyTorch: Basis of constructed NN models.

A particularly helpful resource with respect to the Ising Model was the following: https://stanford.edu/~jeffjar/statmech/intro4.html

The Hamiltonian for the triangular lattices is implemented as formulated herein: https://www.publish.csiro.au/ph/pdf/PH740357


