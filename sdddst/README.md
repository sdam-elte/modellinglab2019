# SDDDST - Simple Discrete Dislocation Dynamics Toolkit
Plastic deformation on the microscopic level in crystalic materials can be described by the motion of dislocations. In this project you will experiment with a simple discrete dislocation dynamics simulator. During the project you are going to get to know how to work with already existing tools and how to modify them. You will have a better understanding about dislocations and how different modelling techniques can approach the same problem. Some c++ programming skill is required!

## Tools
The toolkit with a short description about basic usage can be found here: [SDDDST](https://github.com/pgabor/sdddst)

During the project you can use several tools based on your preferences. E.g.: python, bash, gnuplot, etc...
Do not be afraid to modify the actual source of the tool (you actually have to do it), but keep in mind if you modify something, the functionality has to stay intact most of the time, otherwise you are going to get invalid results!

## Tasks
1. Download and build the source on your computer. Study the available documentation and the help menu. Play around with it ;) Create a configuration with two dislocations in non equilibrium state (with same and different Burgers-vectors) and relax the system. Analyse the results and the log file!
2. Create a small program which is able to extract how the field of a dislocation looks like which is in the origo of the simulation cell. Plot it!
3. Compare the available periodic fields. What happens if you change the following line in "include/constants.h" so fewer periodic images is taken into consideration during the analytic field calculation?
    
    ```cpp
    #define ANALYTIC_FIELD_N 8
    ```
4. Create a random dislocation system with 64 dislocations. Relax the system into equilibrium with the above N for (1,2,3,4) with the analytic periodic field. Compare the log files and the results. Can you see any difference?
5. From now on, use elte's periodic shear stress! What is the difference between a single dislocation's shear stress field and where we use periodic boundaries?
6. Create several different random dislocation configurations with the same dislocation count. Relax them into equilibrium! Average the average dislocation speed - simulation time data. What can be observed?
7. Experiment with the external stress protocols on your relaxed systems. What can you observe? What does it mean?
8. Observe with different configurations and system sizes how the dislocation's relative distance change with the external stress. Make the appropiate modifications in the source if this is needed!
9. Optional: Create your own external stress module with a chosen function based on self chosen properties and apply it to one or two systems. Analyze it!

## Reading materials
* [Dislocations - Wikipedia](https://en.wikipedia.org/wiki/Dislocation)
* Hirth & Lotte: **Theory of dislocations**
* Péter Dusán Ispánovity, István Groma, Géza Györgyi, Ferenc F. Csikor and Daniel Weygand: **Submicron Plasticity: Yield Stress, Dislocation Avalanches, and Velocity Distribution**
* Péter Dusán Ispánovity, István Groma, Géza Györgyi, Péter Szabó and Wolfgang Hoffelner: **Criticality of Relaxation in Dislocation Systems**
* H H. M. Cleveringa, E. Van Der Gissen & A. Needleman: **Comparison of discrete dislocation and continuum plasticity predictions for a composite material**

## Note:
The tool is under continous improvement so it worth to check it out when you work with it if there is an update. Git rulez :)
