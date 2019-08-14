python simulator for integrated modelling of 5G (pysim5g)
===========================================

[![Build Status](https://travis-ci.com/edwardoughton/pysim5g.svg?branch=master)](https://travis-ci.com/edwardoughton/pysim5g)
[![Coverage Status](https://coveralls.io/repos/github/edwardoughton/pysim5g/badge.svg?branch=master)](https://coveralls.io/github/edwardoughton/pysim5g?branch=master)

Description
===========
**pysim5g** is an open-source software tool, based on the Monte-Carlo method, for integrated engineering-economic modelling of 5G.

Statistical analysis can be performed under different radio interference scenarios for assessing system-level performance of 4G/5G co-existence in the sub-6GHz spectrum bands. 

Users can simulate the deployment of new networks delivering different levels of Quality of Service (QoS) for diffferent propagation environments.

Quantified cost analytics provide insight into the economics of (i) ultra-dense networks, (ii) 5G spectral efficiency gains and (iii) the capacity and coverage of 4G/5G co-existence for sub-6GHz spectrum bands.

Setup and configuration
=======================

All code for **pysim5g** is written in
Python (Python>=3.5) and has a number of dependencies.
See `requirements.txt` for a full list.

Using conda
-----------

The recommended installation method is to use [conda](http://conda.pydata.org/miniconda.html),
which handles packages and virtual environments,
along with the `conda-forge` channel which has a host of pre-built libraries and packages.

Create a conda environment called `pysim5g`:

    conda create --name pysim5g python=3.5

Activate it (run each time you switch projects)::

    activate pysim5g

First, install required packages including `fiona`, `shapely`, `numpy`, `rtree` and `pyproj`:

    conda install fiona shapely numpy rtree pyproj

For development purposes, run this command once per machine:

    python setup.py develop

To install pysim5g permanently:

    python setup.py install

To build the documentation:

    python setup.py docs

The run the tests first install:

    conda install pytest

Followed by:

    pytest

Background and funding
======================

The **python simulator for integrated modelling of 5G (pysim5g)** was funded by the
UK [Digital Catapult's](http://www.digicatapult.org.uk) ESPRC-funded Researcher in Residence
programme.

Contributors
============
- Edward J. Oughton (Oxford)
- Kostas Kotsaros (Digital Catapult)
- Fariborz Entezami (Digital Catapult)
- Dritan Kaleshi (Digital Catapult)
- Catarina Fernandes (Digital Catapult)
- Tom Russell (Oxford)
- Jon Crowcroft (Cambridge)
