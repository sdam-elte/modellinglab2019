# Exploring topological phases with the Pybinding package

![](4-scientistsma.jpg)

[Pybinding](http://docs.pybinding.site/en/stable/) is a python package for tight-binding calculations. 
With the help of this package one can easily create simple tight-binding models describing noninteracting
electron systems, and calculate various physical properties, like density of states and electrical conductivity.
The aim of the project is to install the package and with the help of it first investigate certain properties
of simple systems, finally to reproduce some published results.




# Tasks

 1. Install the package in a jupyter notebook environment, make sure that the appropriate version of matplotlib is installed.
 2. Build the Hamiltonian of a simple square lattice in 1,2 and 3 dimensions with 2-300k lattice sites, and calculate the density of states and the bandstructure along high symmetry points in the Brillouin zone.
 3. Using pybinding build a lattice model for the Kane-Mele Hamiltonian of graphene [1]. Using the lattice model calculate the band structure of a graphene ribbon as the function of spin-orbit coupling parameters $\lambda_R$ and $\lambda_{SO}$ and the onsite staggered sublattice potential $\lamda_v$. Make an interactive plot where the bandstructure is plotted for different walues of model parameters.
 5. Calculate the density of states with the KPM method as the function of the magnetic field for a nodal loop semimetal for different orientation of the magnetic field reproducing some results presented at the end of [2].
 4. Reproduce some results in [3] or [4] using the KPM method for calculating the density of states.

# References

- [1](https://arxiv.org/abs/cond-mat/0506581) Phys. Rev. Lett. 95, 146802 (2005)
- [2](https://arxiv.org/abs/1801.04721) Phys. Rev. B 97, 205107 (2018)
- [3](https://arxiv.org/abs/1711.01678) 2D Materials  5, 015017 (2017)
- [4](https://arxiv.org/abs/1812.07299) Phys. Rev. B 99, 035412 (2019)
