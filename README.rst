muonlabdocs
===========

This repository includes documentation, installation instructions, and exercises for everything surrounding the MuonLab detectors 
used for teaching and outreach purposes. 

More information on the MuonLab detectores is available here: https://www.nikhef.nl/muonlab/ 

The required software is described here: https://gitlab.nikhef.nl/muonlab/muonlab  

Prerequisites
-------------

You should have an installation of the conda or mamba package managers installed. It also helps if you have git installed 
but this is not strictly necessary. 

Installation
------------

To install the required packages for the muonlab software, install the conda environment (you can also use mamba instead of conda if you have mamba installed). 

.. code:: bash
    conda env create -f environment.yml

(Note that on conda-forge only PyQt5 is available!)
This will set up a new conda environment that has all necessary packages installed to run the muonlab software. 
Next, you will have to follow the installation instructions of the muonlab software, see here: https://gitlab.nikhef.nl/muonlab/muonlab. 

In essence, you clone the muonlab repository:

.. code:: bash
    git clone https://gitlab.nikhef.nl/muonlab/muonlab.git

Then, switch to the directory you cloned the repository to. Then try to run the GUI:

.. code:: bash
    python GUI/MuonLab_GUI_PyQt5.py

Make sure to use the script with the `_PyQt5` extension, since this is what is installed with conda at the moment. The version of the GUI
without this extension will try to run the GUI with PyQt6. 

License
-------
This project is licensed under a 3-clause BSD style license - see the
``LICENSE`` file.
