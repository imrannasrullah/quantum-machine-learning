# quantum-machine-learning
This code is part of a QML prokect under Dr. Gustavo Seabra to use Pennylane's QML framework to optimize molecular geometries + interaction energies.

Initially, there's 4 different small molecules, where we express these molecule's Hamiltonian in "relative coordinates" (AKA z-matrix coordinates) and show
that VQE optimizes on these coordinates quite a bit faster [completed].

Then, a water dimer is selected for proof of concept for modeling interaction energies, where we use relative coordinates to optimize the interaction between these 2 molecules, which can be used to model protein-ligand interactions [currently in progress].

Finally, these relative coordinates are used to train a classical neural network on the wavefunction of interaction chemical systems. This neural network should then be able to plot out a potential energy surface of interaction systems [currently in progress].
