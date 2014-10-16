# BIOMD0000000305: Kolomeisky2003_myosin

## Installation

Download this repository, and install with distutils

`python setup.py install`

Or, install using pip

`pip install git+https://github.com/biomodels/BIOMD0000000305.git`

To install a specific version (in this example, from the 2014-09-16 BioModels release)

`pip install git+https://github.com/biomodels/BIOMD0000000305.git@20140916`

## Usage

Importing the model package.

`import BIOMD0000000305 as model`

Get the SBML string from the model

`print model.sbmlString`

If [python-libsbml](https://pypi.python.org/pypi/python-libsbml) bindings are
installed, the libsbml.SBMLDocument object is also accessible

`model.sbml`


# Model Notes


This is the 2 state model of Myosin V movement described in the article:  
**A simple kinetic model describes the processivity of myosin-v.**   
Kolomeisky AB , Fisher ME Biophys. J. 84(3):1642-50 (2003); PubmedID:[
12609867](http://www.ncbi.nlm.nih.gov/pubmed/12609867)  

Abstract:  
Myosin-V is a motor protein responsible for organelle and vesicle transport in
cells. Recent single-molecule experiments have shown that it is an efficient
processive motor that walks along actin filaments taking steps of mean size
close to 36 nm. A theoretical study of myosin-V motility is presented
following an approach used successfully to analyze the dynamics of
conventional kinesin but also taking some account of step-size variations.
Much of the present experimental data for myosin-V can be well described by a
two-state chemical kinetic model with three load-dependent rates. In addition,
the analysis predicts the variation of the mean velocity and of the
randomness-a quantitative measure of the stochastic deviations from uniform,
constant-speed motion-with ATP concentration under both resisting and
assisting loads, and indicates a substep of size d(0) approximately 13-14 nm
(from the ATP-binding state) that appears to accord with independent
observations.

The model differs slightly from the published version. The ATP and ADP bound
forms of myosin are called S0 and S1. The state transition and binding
constants are called k_1, k_2, k_3 and k_4 instead of k00, u01, k'0 and w01.
Similarly the state loading factors are named th_1, th_2, th_3 and th_4
instead of θ+0, θ+1, θ-0 and θ-1. The species fwd_step1, fwd_step2, back_step1
and back_step2 count the number of state changes of each kind the myosine
molecules have taken over time.  
The model can be evaluated in a deterministic continuous or stochastic
discreet fashion. The parameter V holds the (forward) speed at each time
point, the V_avg the overall way divided by the simulation time and the amount
of myosine molecules.

Originally created by libAntimony v1.4 (using libSBML 3.4.1)

This model originates from BioModels Database: A Database of Annotated
Published Models (http://www.ebi.ac.uk/biomodels/). It is copyright (c)
2005-2011 The BioModels.net Team.  
For more information see the [terms of
use](http://www.ebi.ac.uk/biomodels/legal.html).  
To cite BioModels Database, please use: [Li C, Donizelli M, Rodriguez N,
Dharuri H, Endler L, Chelliah V, Li L, He E, Henry A, Stefan MI, Snoep JL,
Hucka M, Le Novère N, Laibe C (2010) BioModels Database: An enhanced, curated
and annotated resource for published quantitative kinetic models. BMC Syst
Biol., 4:92.](http://www.ncbi.nlm.nih.gov/pubmed/20587024)


