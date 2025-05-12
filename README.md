All documents in this repository are Jupyter notebooks designed to guide you in reproducing the results from our paper published 
in Physical Review B, 111(4):045101, 2025.
In this work, we developed a novel restricted Boltzmann machine incorporating essential non‐local connections, efficiently and 
accurately representing arbitrary toric code ground states, extending its applicability to a wide range of complex quantum systems. 
While our research involved extensive experimentation and repetition, the selected notebooks included here outline the key ideas 
and methods necessary to replicate our main results.


1. This note sketches the idea of the paper we cited (Physical Review X, 7(2):021021, 2017), analytically solving the face terms
   and numerically (via machine learning) searching for solutions to the vertex terms. The FRRBM is set on a 2D plane without
   boundaries, assuming translational invariance but not rotational invariance; all parameters are assumed to be real. In this
   simple example, we initialize the parameters near an expected solution, resulting in rapid convergence. When using broader
   initialization to explore the solution space more extensively, convergence becomes slower but uncovers more solutions.
   
2. To understand the different solutions, we generalize the method to a torus, where a basis of the ground-state manifold can
   be defined. This note sketches the idea using a 3×3 square lattice. Building on prior experience and physical intuition,
   we enforce translational invariance but not rotational invariance. All parameters are assumed to be complex, although
   the simple example uses real values.

3. This note collects several solutions obtained through extensive searches over complex-valued parameters, continuing from
   the previous step. All solutions are initially complex but converge toward real-valued configurations. We analytically
   solve and explain this phenomenon in Physical Review B, 111(4):045101, 2025.

4. Having understood the representational capacity of the FRRBM, we proceed to construct an efficient neural network
   representation for arbitrary ground states of the toric code. By introducing three additional hidden neurons, this
   note sketch the reasoning that demonstrates these three neurons are both necessary and sufficient.

6. The RBM can efficiently find solutions for arbitrary ground states through a search process similar to previous examples.
   This code demonstrates the result for a specific ground state that cannot be represented by the FRRBM.
