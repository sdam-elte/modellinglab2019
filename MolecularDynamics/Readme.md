## Classical Molecular Dynamics (MD) Simulation with LAMMPS

Simulating the dynamics of atoms, molecules and bulk materials can be done on many length scales with more or less detailed models. In this tutorial we treat the atoms as point particles and describe their interactions classically. There are many software packages for molecular dynamics, such as DLPOLY, GROMACS, AMBER, NAMD, HOOMD etc. A chosen time integrator algorithm will calculate the forces acting on each atom and moves them by a predefined timestep. This way we can observe the dynamics of a couple of thousand of atoms. From these simulations we will be able to calculate statistical averages of physical quantities, potential energy surfaces, diffusion constants, phonon dispersions and so on.

![viz.png](viz.png)

I recommend to use LAMMPS for this project https://lammps.sandia.gov/. It easy to setup and one of the popular options.

In order to run the simulations we will need to use forcefield parameters. Next to the LAMMPS source code there is a `potentials` directory, which contains forcefield parameters for various element types for different models. We will use the **REAXFF**, **Tersoff** and **COMB3** forcefield parameters and a **Lennard-Jones** type potential with charges.

New task:
try to reproduce the results from the following paper:
https://www.sciencedirect.com/science/article/abs/pii/S0378381220301618


Old task:
2. a, Run the example of `in.comb.Si` in the `examples/comb/combSi` directory  <br>
b, Run the example of `in.spce` in the `examples/rdf-adf` directory. Try to find other values for the water's RDF and ADF in the literature and compare them.  <br>
c, Run the examples of `AuO` and `CHO` in the `examples/reax` directory. Take a look into the papers mentioned in the `README` file for each example. Please explain in few sentences how they obtained the **REAXFF** forcefield parameters and what are their limitations!<br?
d, Try to visualize the movements of atoms for one of the above examples! You can use VMD[https://www.ks.uiuc.edu/Research/vmd/], (Paraview)[https://www.paraview.org/], (VisIt)[https://wci.llnl.gov/simulation/computer-codes/visit/], (Avogadro)[https://avogadro.cc/] or any other softwares.


3. a, Calculate an O_2 molecule's dissociation energy using an MD simulation with the **REAXFF** forcefield<br>
b, Calculate the dissociation energy of a hydrogen atom from methane (CH_4) <br>
c, Compare your results with the literature!

4. Simulate water the **REAX** forcefield and **Lennard-Jones** potential with **Coulomb** interaction (as in exercise 2.b,)<br>
https://www.youtube.com/watch?v=IGEP-u1PNX0 <br>
https://www.youtube.com/watch?v=NQhjAtCKghE&list=PLEdP7cCNp3PpNfrVieARvrXMtCdp1L7yU&t=0s&index=44 <br>
a, Create a box of water <br>
b, Equilibrate the system with the proper thermostat<br>
c, What is the equilibrium density of water at `300K` with the two models ? <br>
d, Is there difference in the radial and angle distribution functions with the two models?
https://www.ncbi.nlm.nih.gov/pmc/articles/PMC6175054/
https://www.researchgate.net/profile/Ashu_Choudhary4/post/Can_anybody_guide_me_to_calculate_Spatial_distribution_function/attachment/59d622726cda7b8083a1c262/AS%3A273533098233860%401442226780198/download/JChemPhys_99_3049.pdf

Choose one of the following:

A. Calculate vibrational modes with the **Tersoff** forcefield<br>
a, Create a periodic single wall carbon nanotube (SWCNT) and calculate the vibrational modes! <br>
b, What parameters limit the accuracy of the calculation? Determine limiting parameters and run simulations for different set of these parameters! <br>
c, Calculate the vibrational modes of a CNT with vacancies!<br>
https://journals.aps.org/prb/pdf/10.1103/PhysRevB.69.235409 <br>
https://www.youtube.com/watch?v=YXQ0gZr0kkI <br>
https://www.youtube.com/watch?v=3NmrxLbBx60 <br>

B. Wave-Drag Enhancement of Friction in Sliding Carbon Nanotubes<br>
Please read this paper, and try to reproduce the simulation (and results) https://journals.aps.org/prl/pdf/10.1103/PhysRevLett.97.195901


Many of the above calculated properties are well documented in the literature, therefore for each section write a brief report of your findings in comparison with the results of others!

[] https://www.isis.stfc.ac.uk/Pages/md-lecture-1.pdf
