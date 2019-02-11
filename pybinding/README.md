# Exploring topological phases with the Pybinding package

![](4-scientistsma.jpg)
## [Topological insulators](https://en.wikipedia.org/wiki/Topological_insulator)
A topological insulator is a material with non-trivial symmetry-protected topological order that behaves as an insulator in its interior but whose surface contains conducting states meaning that electrons can only move along the surface of the material. However, having a conducting surface is not unique to topological insulators, since ordinary band insulators can also support conductive surface states. What is special about topological insulators is that their surface states are symmetry-protected by particle number conservation and time reversal symmetry.

## [Topological semimetals](https://arxiv.org/pdf/1609.05414.pdf)
Topological semimetals (TSM) are defined as systems where the conduction and the valence bands cross each
other in the Brillouin zone (BZ), and the crossing is nonaccidental, i. e., cannot be removed by perturbations on
the Hamiltonian without breaking any of its symmetries.
If there be no symmetry, two bands, when close in energy, will hybridize with each other and maintain a gap
in-between, through a mechanism known as the band repulsion; however, when in the presence of certain symmetries
(e. g. crystalline symmetries and time-reversal symmetry), the two crossing bands may have different quantum numbers
such that they cannot be hybridized. Hence all topological semimetals, can
only be protected by symmetries and hence belong to symmetry protected topological phases of matter.
In three dimensions (3D), two bands can cross each other either at discrete points or along a closed curve. 
In the former case, there are Weyl semimetals1,2 and Dirac semimetals that have been intensively studied
in theory as well as in experiment. In the latter case, the curve where the bands cross is called a nodal line,
which may either take the form of an extended line running across the BZ, whose ends meet the at the BZ boundary,
or wind into a closed loop inside the BZ, or even form a chain consisting of several connected loops (nodal chain).
Topological semimetals with such line band crossings are called topological nodal line semimetals (TNLSM).

## The package
[Pybinding](http://docs.pybinding.site/en/stable/) is a python package for tight-binding calculations. 
With the help of this package one can easily create simple tight-binding models describing noninteracting
electron systems, and calculate various physical properties, like density of states and electrical conductivity.
The aim of the project is to install the package and with the help of it first investigate certain properties
of simple systems, finally to reproduce some published results.




# Tasks

 1. Install the package in a jupyter notebook environment, make sure that the appropriate version of matplotlib is installed.
 2. Build a lattice model (based ont he pybinding examples) of a zig-zag graphene ribbon and calculate the band structure for it. 
 3. Using pybinding build a lattice model for the Kane-Mele Hamiltonian of graphene [1]. Using the lattice model calculate the band structure of a graphene ribbon as the function of spin-orbit coupling parameters $\lambda_R$ and $\lambda_{SO}$ and the onsite staggered sublattice potential $\lamda_v$. Make an interactive plot where the bandstructure is plotted for different walues of model parameters.
 4. Build the Hamiltonian of a simple square lattice in 1,2 and 3 dimensions with 2-300k lattice sites, and calculate the density of states and the bandstructure along high symmetry points in the Brillouin zone.
 5. Calculate the density of states with the KPM method as the function of the magnetic field for a nodal loop semimetal for different orientation of the magnetic field reproducing some results presented at the end of [2].
 6. (extra) Reproduce some results in [3] or [4] using the KPM method for calculating the density of states.

# References

- [1](https://arxiv.org/abs/cond-mat/0506581) Phys. Rev. Lett. 95, 146802 (2005)
- [2](https://arxiv.org/abs/1801.04721) Phys. Rev. B 97, 205107 (2018)
- [3](https://arxiv.org/abs/1711.01678) 2D Materials  5, 015017 (2017)
- [4](https://arxiv.org/abs/1812.07299) Phys. Rev. B 99, 035412 (2019)
