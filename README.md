# SpikyPop 
 Matlab-module for calculation of extracellular action potentials (EAPs) from neuron models and networks. This package mainly relies on the NEURON simulator (http://www.neuron.yale.edu/neuron), the LFPy Python-package (https://www.frontiersin.org/articles/10.3389/fninf.2013.00041/full) and Matlab software.
 
Simulating extracellular recordings of neuronal populations is a challenging task to understand extracellular field potentials at different scales. Detailed neuronal compartmental models with active/passive compartments are generally used which could lead to a high computational burden. On the contrary, simplified models have already been proposed such as the dipolar model. The latter has been used but it is biophysically not very realistic. A compromise must be found between detailed compartment models and point or dipole models of neurons.

 The simulator takes the form of a linear geometry based filter that can model the shape of EAPs by taking into account its generation in the cell body and its propagation along the axon. The method is based on the convolution of the somatic membrane current given by the Hodgkin-Huxley dynamics and a geometrical filter taking into account the relative position of the electrode. 
 
 
 For more details, see :
 
 H. Tran, S. Le Cam, R. Ranta and V. Louis-Dorr. Modelling and analysis of extracellular action potentials. In Journal of Computational Neuroscience, 2019. [under review]
 
 H. Tran, R. Ranta, S. Le Cam and V. Louis-Dorr. Extracellular recordings simulation : a time-efficient method to model action potentials signatures of neuronal populations. In the NeuroFrance, Marseille, France, 2019.
   
 H. Tran, R. Ranta, S. Le Cam and V. Louis-Dorr. Simulating extracellular signatures of action potentials using single compartment neurons and geometrical filtering. In the 27th Computational Neuroscience (CNS), Seattle, USA, 2018.
 https://hal.archives-ouvertes.fr/hal-01917383

# User guide 

It is recommended to run the different files under Ubuntu/Debian/MacOS - especially for the NEURON simulator and the LFPy Python-package.

**** Step for reproducing EAPs from single neurons :

1/ Modify the .hoc file to choose the neuron morphology.

2/ Import the .hoc file in the LFPy python-package (for installation, see https://github.com/LFPy/LFPy) and save the different data (EAPs).

3/ Import the saved data in matlab and run the main file (don't forget to modify the morphology parameters to match with the ones of the .hoc file)

**** Step for reproducing EAPs from neuronal population :




#

The method was developed within the team of 'Neurosciences des systèmes et de la cognition' belonging to the CRAN - Centre of Research in Automatic of Nancy - Nancy, France.

If you have any questions concerning the method, please send en email to harry.tran@univ-lorraine.fr
