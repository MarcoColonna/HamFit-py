Version 0.0.1 with pyhef implementation

HamF_py.py : is the actual module you want to import (pip installable in the future)

B02DstTauNu_TauMu.config : configuration file used to produce the Reader object in the example

B02DstTauNu_TauMu.ibynb : first example of reading a config file, handling a hammer histogram with the current interface and fitting using iminuit

MC_gen: contains the code used to produce the MC for the example
root: contains the MC produced, and the hammer .dat files for the example

TO START:

if you want to run the example (which is very basic right now) all you have to do is download the repository and (if necessary) change the path to the linking of Hammer in "HamF_py.py" to your local path to the hammer module.
Hammer 1.3 is required to use the BLPRXP parametrization in the example.
If you have a conda environment containing the python interface of Hammer 1.3 installed you can immedeatly run the example without changing anything

You can than open the jupyter-notebook "B02DstTauNu_TauMu.ibynb" and try to execute the very basic code inside to:

-read a config file and build a fitter object out of it

-try to change the FFs and the WCs to see how the shape of the contributions change

-apply a nll scan using iminuit over the PS of the Scalar WC
