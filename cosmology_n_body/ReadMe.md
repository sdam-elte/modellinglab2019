# N-body simulations in cosmology

In this project you will experiment with a professional n-body simulator, frequently used in cosmology.

The [Gadget 2](http://www.mpa-garching.mpg.de/gadget/) simulator will help you understanding the 
[theory](http://www.mpa-garching.mpg.de/gadget/gadget2-paper.pdf) behind the simulation algorithms.
([local copy with notes](http://csabai.web.elte.hu/http/simulationLab/gadget2-paper.pdf)).

__Note:__ From October 2020, there is a new version: [GADGET4](https://wwwmpa.mpa-garching.mpg.de/gadget4/)

## Steps:

1. [Install](http://www.mpa-garching.mpg.de/gadget/users-guide.pdf) a local version of the software with the accomaining libraries.
   ([compile](http://obswww.unige.ch/lastro/misc/TP4/doc/rst/Exercices/Ex05.html) the source code and run it on a single processor)

2. Compile the parallel version (the [MPI](http://csabai.web.elte.hu/http/simulationLab/Szammodlab_ParallelComputing.pdf) is a good parallel library)

3. Experiment with the demo problems, povided with the GADGET code:
   * [collision of galaxies](http://www.mpa-garching.mpg.de/mpa/research/current_research/hl2005-2b/hl2005-2b-en.html)
   * [large scale evolution of the Universe](http://www.mpa-garching.mpg.de/galform/millennium/)

4. For each problem above evaluate the simulation results, create a section in your report and a brief presentation

5. Select a similar new problem, e.g. by reading a research paper from the last 3 years, and reproduce the results
at a scale, which fits into the computers you have access to. A good starting point for finding an appropriate article
is to search in the google scholar or in any other scientific citation database, and looking into the papers that 
refers to the above simulator or papers in documentation of the simulator.
A possible interesting project: Compare standard dynamics and [non-Newtonian gravitation](http://en.wikipedia.org/wiki/Modified_Newtonian_dynamics). There is a description of a [modified gravity GADGET code](https://academic.oup.com/mnras/article/436/1/348/972921).

## Further reading

[Gadget File Viewer](http://astro.dur.ac.uk/~jch/gadgetviewer/index.html)

[predictor-corrector in n-body simulations](https://pdfs.semanticscholar.org/96aa/9d4c0c867364aff6b8549e67b93f198bf56d.pdf)

[Introduction](http://www.artcompsci.org/msa/web/index.html) to N-body simulation by P. Hut and J. Makino (local [copy](http://csabai.web.elte.hu/http/simulationLab/hutMakinoTutorial.pdf) and [code](http://csabai.web.elte.hu/http/simulationLab/hutMakinoStarterCode.tar))
 
Generating initial conditions:
* [Starscream](https://github.com/jayjaybillings/starscream): for collisions of galaxies 
* [2LPTic](http://cosmo.nyu.edu/roman/2LPT/): general cosmology simulations

