SHG Yield for Semiconductor Surfaces
====================================

[![DOI](https://zenodo.org/badge/11697217.svg)](https://zenodo.org/badge/latestdoi/11697217)

SHGYield is a python program for calculating the second-harmonic generation (SHG) yield for semiconductor surfaces.

You will first need the electron density and matrix elements calculated using [ABINIT](http://www.abinit.org), an open source ab-initio software. You can use these to produce the components of the nonlinear susceptibility tensor, either with your own software or using [TINIBA](https://github.com/bemese/tiniba), our own optical response software. All the theory is derived step-by-step in my [Ph.D. thesis](https://github.com/roguephysicist/thesis-phd) and references therein. This software has been used in the following publications:

* [Phys. Rev. B 94, 115314](https://doi.org/10.1103/PhysRevB.94.115314)
* [Phys. Rev. B 93, 235304](https://doi.org/10.1103/PhysRevB.93.235304)
* [Phys. Rev. B 91, 075302](https://doi.org/10.1103/PhysRevB.91.075302)
* [arXiv:1604.07722](https://arxiv.org/abs/1604.07722)

Tested with Python 2 and 3, and Anaconda Python 4+ on Mac OS X and Linux. It should work on any system with the required Python packages installed. The user can choose to include the effects of multiple reflections if desired, and select several parameters for calculating these effects. Read the articles above and the appropriate thesis sections for more details.

requirements:
sys, math, numpy, scipy

usage:
`python shgyield.py <sample.in>`

License
------------------------------------

Copyright 2017 Sean M. Anderson and Bernardo S. Mendoza.

SHGYield is free software made available under the BSD-3-Clause License. For details please see the LICENSE file.
