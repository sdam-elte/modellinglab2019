# Simulation of CERN LHC TEPX Silicon Pixel Detector for HL-LHC upgrade

## Investigation of tracking efficiency and the effect of the cooling pipe

### Introduction

At the High-Luminosity LHC (expected to become operational in 2027), on average 140-200 proton-proton collisions will happen in every bunch crossing, i.e. at every 25 ns. This high particle flux requires highly granular and radiation hard detector technology.

The precise measurement of the luminosity (L) - that characterises the collision rate (dN/dt = L * total_cross_section) provided by the accelerator - is essential as it affects almost all physics measurements carried out at the LHC. To reach the target precision of 1%, the detector must provide a linear response over more than 4 orders of magnitude in instantanous luminosity as well as excellent stability and high availability over the full data taking period.

The CMS collaboration chosen Silicon pixel detector technology to answer the technological challenges. The main luminometer of the experiment will be the forward extension of the pixel detector (TEPX). The modules of TEPX must be kept at low tempreature  using CO2 cooling to operate the detctor with low noise. The current plans place the cooling pipes between the detector layers. While it has the advantage of efficient cooling, the pipes might scatter or absorb the particles that we want to measure. 

The aim of the project is to quantify this effect with the help of the Geant4 particle physics simulation which was developed at ELTE.

![Image](Sketch-of-one-quarter-of-the-layout-of-the-CMS-Tracker-for-HL-LHC-in-the-r-z-view.png "Hl-LHC upgraded CMS Tracking system")

![Image](TEPX_PCB.jpg "Layout of a TEPX detector layer")

### Project plan

Step 1: Install Geant4 [3]. A guide on installation can be found:
https://sites.google.com/view/geant4elte/how-to-install-geant4

Step 2: Download the TEPX simulation source code which was developed at ELTE, compile it and visualize the geometry of the detector elements in the Geant4 simulation.

![Image](TEPX_Screenshot2020-02-09_233312.png "TEPX Simulation")

Step 3: The detectors and the cooling pipes are included in the simulation. The task of the student is to include CO2 (the two phase cooling material in the pipes) in the simulation.

Step 4: Install ROOT [4]
Develop an analysis code that analyzes the output of the Geant4 simulation. This should be automatized as different types of particles and several particle energies need to be investigated.

Step 5: Run the simulation and the consequent analysis code developed in step 4 to understand the effect of the beam pipe for different energies and particles on the efficiency and fake rate of finding coincidences in the overlapping detector layers.

### References

[1] https://www.researchgate.net/publication/323786425_Beam-dynamic_effects_at_the_CMS_BRIL_van_der_Meer_scans

[2] https://arxiv.org/pdf/1806.11245.pdf

[3] https://geant4.web.cern.ch/

[4] https://root.cern.ch/

### Contacts

Gabriella.Pasztor@ttk.elte.hu and galgoczi@caesar.elte.hu
