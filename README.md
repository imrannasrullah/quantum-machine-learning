# quantum-machine-learning
This is a Quantum Machine-Learning project under the UF Medicinal Chemistry Lab, which uses Pennylane's QML framework to optimize molecular geometries + interaction energies.

(With extreme appreciation and gratitude to both Dr. Gustabo Seabra and Dr. Chenglong Li for their co-mentorship and willingness to guide me every step of the way)

For the first stage of this project, there's 4 different small molecules, where we express these molecule's Hamiltonian in "relative coordinates" (AKA z-matrix coordinates) and show
that VQE optimizes on these coordinates quite a bit faster + simplifying Hamiltonian parametrization as opposed to normal parametrization using Euclidean-coordinates [completed].

Then, a water dimer is selected for proof of concept for modeling interaction energies, where we use relative coordinates to optimize the interaction between these 2 molecules, which can be used to model protein-ligand interactions [completed].

Finally, these relative coordinates are used to train a classical neural network on the wavefunction of interacting chemical systems (this code is adapted from a similar Pennylane achieving a similar purpose, but it's outdated and uses full euclidean coordinates). This neural network can plot the potential energy surface of interaction systems [completed]. Finally, we contrast neural network performance on biologically-relevant systems by comparing its ability on z-matrix vs. equivalent euclidean-coordinate parameters.
