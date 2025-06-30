---
title: "List of Software"
layout: post
date: 2016-11-06 16:45:46 PM EST
author: Tong Zhang
category: blog
tag:
- python
- programming
- computer
---
When I was working at the linear accelerator driven free-electron laser facility, I've
developed a lot of different software to do the machine commissioning/operation, numerical simulation/modeling, etc. Each one below could be the name of the software project,
or software package, or GitHub repository.

- ``felapps``

    > A Python package developed for the commissioning of 
    > free-electron laser facility, with the intention of providing useful
    > toolkits for the high-level applications, both command line 
    > interface (CLI) and graphical user interface (GUI) applications are 
    > developed.

    * [Source code](https://github.com/archman/felapps){:target="_blank"}
    * [Documentation](https://archman.github.io/felapps/){:target="_blank"}
    * [PyPI](https://pypi.python.org/pypi/felapps){:target="_blank"}

- ``beamline``

    > A Python package created for the accelerator (e.g. LINAC)
    > online-modeling (simulation code: `Elegent`), trying to supply both CLI and GUI 
    > working environment, upon which extensions/tools could be 
    > developed to solve specific problems.

    * [Source code](https://github.com/archman/beamline){:target="_blank"}
    * [Documentation](https://archman.github.io/beamline/){:target="_blank"}
    * [PyPI](https://pypi.python.org/pypi/beamline){:target="_blank"}

- ``pydraw``

    > A Python GUI application to illustrate the basic 
    > features of Python and wxPython.

    * [Source code](https://github.com/archman/pydraw){:target="_blank"}

- ``pelican``

    > A C++ CLI application to simulate the free-electron
    > laser process, i.e. the radiation amplification procedure originated from the 
    > interaction between electron beam and radiation itself.

    * [Source code](https://github.com/archman/pelican){:target="_blank"}

- ``vFEL``

    > EPICS soft-IOC (C/C++) application for virtual FEL machine 
    > (FEL simulation section is to be done with `Genesis 1.3`), the data source should be 
    > came from ``beamline`` model,
    > so the two packages should be used together.

    * [Source code](https://github.com/archman/vFEL){:target="_blank"}

- ``modu``

    > A C++ CLI application to simulate the interaction between electron
    > beam and optical laser, basically the modulation process happened when electron
    > beam goes through the modulator undulator (critical physics process of a seeded FEL),
    > the generated electron beam phase space distribution could be used
    > by ``Elegant`` or ``Genesis 1.3``.

    * [Source code](https://github.com/archman/modu){:target="_blank"}

- ``pyrpn``

    > A RPN solver written with Python, RPN is brief for 
    > "Reverse Polish Notation". ``beamline`` package depends on this package to
    > parse the RPN expressions used in the `Elegant` input file. 

    * [Source code](https://github.com/archman/pyrpn){:target="_blank"}
    * [PyPI](https://pypi.python.org/pypi/pyrpn){:target="_blank"}