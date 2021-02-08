## Classical Molecular Dynamics (MD) Simulation with LAMMPS

Simulating the dynamics of atoms, molecules and bulk materials can be done on many length scales with more or less detailed models. In this tutorial we treat the atoms as point particles and describe their interactions classically. There are many software packages for molecular dynamics, such as DLPOLY, GROMACS, AMBER, NAMD, HOOMD etc. A chosen time integrator algorithm will calculate the forces acting on each atom and moves them by a predefined timestep. This way we can observe the dynamics of a couple of thousand of atoms. From these simulations we will be able to calculate statistical averages of physical quantities, potential energy surfaces, diffusion constants, phonon dispersions and so on.

![viz.png](viz.png)

I recommend to use LAMMPS for this project https://lammps.sandia.gov/. It easy to setup and one of the popular options.

In order to run the simulations we will need to use forcefield parameters. Shipped with the LAMMPS source code there is a `potentials` directory, which contains forcefield parameters for various element types for different models. I recommend using the **REAXFF** forcefield parameters or a **Lennard-Jones** type potential with charges.

#### Description of the task:
The following paper by Zhang et al. describes a classical molecular dynamics type of calculation of the $Na^+$ - $F^-$ ion pair distance in aqueos solution. Try to calculate/simulate the quantities which appear in the paper!
[Link to the paper](https://www.sciencedirect.com/science/article/abs/pii/S0378381220301618)

First try to use a simpler model, which runs very fast and allows a crude estimation of these quantities! Once you have the right tools you may move further to a more precise model such as the **ReaxFF**. You may also use the forcefield parameters which appear in the paper.

Try to visualize the movements of atoms/ions as well! You can use VMD[https://www.ks.uiuc.edu/Research/vmd/], (Paraview)[https://www.paraview.org/], (VisIt)[https://wci.llnl.gov/simulation/computer-codes/visit/], (Avogadro)[https://avogadro.cc/] or any other softwares.

#### Forcefield parameters: https://www.scm.com/doc/ReaxFF/Included_Forcefields.html
``` 
    M.V. Fedkin, Y.K. Shin, N. Dasgupta, J. Yeon, W. Zhang, D. van Duin, A.C.T. van Duin, K. Mori, A. Fujiwara, M. Machida, H. Nakamura, and M. Okumura Development of the ReaxFF Methodology for Electrolyte-Water Systems J. Phys. Chem. A, 2019, 123 (10), pp 2125-2141

        Developed for water-electrolyte systems with Li+, Na+, K+, Cs+, F-, Cl-, and I-
        trained against (QM) calculations related to water binding energies, hydration energies and energies of proton transfer

```

#### For validating the water model on the way:
* Spatial distribution of water: https://www.ncbi.nlm.nih.gov/pmc/articles/PMC6175054/
* Assimilating Radial Distribution Functions to Build Water Models with Improved Structural Properties: https://www.researchgate.net/profile/Ashu_Choudhary4/post/Can_anybody_guide_me_to_calculate_Spatial_distribution_function/attachment/59d622726cda7b8083a1c262/AS%3A273533098233860%401442226780198/download/JChemPhys_99_3049.pdf



[] https://www.isis.stfc.ac.uk/Pages/md-lecture-1.pdf
