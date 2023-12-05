# Quantum Quirks Unraveling Protein Folding Through an Advanced Interface.
Modification of the IBM public code by adding protein folding in different phrases as well as the study of folding at a polar/apolar interface.


<p align="center">
  <img src="https://user-images.githubusercontent.com/117435891/200289004-db421486-5826-4e49-9c70-ff0aad7a60a9.gif" width="3840" height="250" />
</p>


<div align="center">
  
[![GitHub forks](https://img.shields.io/github/forks/DanielCondeTorres/Quantum-Quirks-Unraveling-Protein-Folding-Through-an-Advanced-Interface.)](https://github.com/DanielCondeTorres/Quantum-Quirks-Unraveling-Protein-Folding-Through-an-Advanced-Interface./network)
[![GitHub issues](https://img.shields.io/github/issues/DanielCondeTorres/Quantum-Quirks-Unraveling-Protein-Folding-Through-an-Advanced-Interface.)](https://github.com/DanielCondeTorres/Quantum-Quirks-Unraveling-Protein-Folding-Through-an-Advanced-Interface.)
![GitHub pull requests](https://img.shields.io/github/issues-pr/DanielCondeTorres/Quantum-Quirks-Unraveling-Protein-Folding-Through-an-Advanced-Interface.)
[![GitHub stars](https://img.shields.io/github/stars/DanielCondeTorres/Quantum-Quirks-Unraveling-Protein-Folding-Through-an-Advanced-Interface.)](https://github.com/DanielCondeTorres/Quantum-Quirks-Unraveling-Protein-Folding-Through-an-Advanced-Interface./stargazers)
![GitHub repo size](https://img.shields.io/github/repo-size/DanielCondeTorres/Quantum-Quirks-Unraveling-Protein-Folding-Through-an-Advanced-Interface.)
[![GitHub license](https://img.shields.io/github/license/DanielCondeTorres/Quantum-Quirks-Unraveling-Protein-Folding-Through-an-Advanced-Interface.)](https://github.com/DanielCondeTorres/Quantum-Quirks-Unraveling-Protein-Folding-Through-an-Advanced-Interface.)
![GitHub language count](https://img.shields.io/github/languages/count/DanielCondeTorres/Quantum-Quirks-Unraveling-Protein-Folding-Through-an-Advanced-Interface.)

![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
</div>

# Description of the challenge
Antimicrobial peptides (AMPs) are critical components of the innate immune system that are present in all living organisms [1]. These peptides have been primarily associated with a defensive role against exogenous infections caused by bacteria, viruses and fungi, and are considered powerful and versatile endogenous antibiotics, capable of resisting bacterial adaptation for millions of years. However, recent research advances have pointed to the link between AMPs and a broader spectrum of diseases, such as cancer and various human inflammatory and autoimmune diseases, including ageing [2, 3]. ageing [2, 3].

In general, the study of peptide and protein folding is an intrinsically very complex problem whose practical solution is beyond the reach of classical algorithms even in very simplified models such as the one that considers amino acids as simple spheres with different hydrophobic-polar character [5, 6]. In this scenario, quantum computers emerge as a promising tool despite the current state of intermediate noise level technology (NISQ). Recent work has attempted to solve this problem for relatively short amino acid sequences [7, 8] in homogeneous media. In relation to our study, the complexity is further increased because the structure and functionality of AMPs are strongly influenced by the inhomogeneous and anisotropic environment in which they exhibit their activity, specifically, the membrane-water interface. This particularity highlights the need to intensify efforts in the development of quantum computing techniques, which may lead to significant discoveries in the study and development of new antimicrobial peptides, thus expanding the frontiers of our scientific understanding and therapeutic potential.


<p align="center">
  <img src="https://user-images.githubusercontent.com/117435891/199940424-2ad7347e-bbcb-4425-bfc6-bb7a3fca7413.gif" alt="animated"  />
</p>


 



<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li><a href="#introduction-movie_camera">Introduction</a></li>
    <li><a href="#general-pre-requirements-computer">Pre-requirements</a></li>
    <li><a href="#required-files-">Required-files</a></li>
    <li><a href="#usage-%EF%B8%8F">Usage</a></li>
    <li><a href="#wiki-">Wiki</a></li>
    <li><a href="#distribution-of-tasks-%EF%B8%8F">Distribution of tasks</a></li>
    <li><a href="#faqs-interrobang">FAQs</a></li>
    <li><a href="#contributing-%EF%B8%8F">Contributing</a></li>
    <li><a href="#cite-mortar_board">Cite</a></li>
    <li><a href="#license-green_book">License</a></li>
  </ol>
</details>

<!-- Introduction --> 
## Introduction :movie_camera:
In SuPepMem the simulations have been performed with the [martini_v2.2](http://cgmartini.nl/) force field, using the [Gromacs 2020](https://www.gromacs.org/) Software, highlighting the following simulation parameters:
- Simulation length (ns): 5000
- Electric field (kJ mol-1 nm-1 e-1): 0
- Temperature (K): 300 (v-rescale)
- Pressure (Bar): 1 (parrinello-rahman semiisotropic)
-  Time step (fs) : 25 
<!-- Pre-requirements -->
## General Pre-requirements :computer:

In order to run the program it is necessary to have the following requirements installed:

The program is written in Python language so Python version 3 or higher is required. Also, for python programs to work properly the following libraries are needed:
- [Os](https://docs.python.org/3/library/os.html)
- [Re](https://docs.python.org/3/library/re.html)
- [Sys](https://docs.python.org/3/library/sys.html)
- [Json](https://docs.python.org/3/library/json.html)
- [Time](https://docs.python.org/3/library/time.html)
- [Argparse](https://docs.python.org/3/library/argparse.html)
- [Subprocess](https://docs.python.org/3/library/subprocess.html)
- [Pandas](https://pandas.pydata.org/)
- [MDAnalysis](https://www.mdanalysis.org/) 
- [mpl_toolkits.axes_grid1](https://matplotlib.org/stable/tutorials/toolkits/axes_grid.html)
- [Numpy](https://numpy.org)
- [Matplotlib](https://matplotlib.org)
- [Supepdex](https://github.com)*

To be able to use these libraries, it is recommended to work with anaconda environment.

In case the user wishes to see trajectories, the use of the [VMD](https://www.ks.uiuc.edu/Research/vmd/) program is recommended.


If you are working in an anaconda environment and you need to install a specific module:

```
conda install module
```

or, if you have pip installed:

```
conda install pip
```
```
pip install module
```

*Supepdex is an external module (supepdex.py) of the main program SuPepMem.py needed to ...


<!-- Required-files -->
## Required files 📋
- A TPR file with the description of the system.
- A XTC file with the trajectory of the simulation with no correction.
- The folder where those files are, i.e. the system folder.
- The folder for the outcome of the analysis.

<!-- Usage -->
## Usage ⚙️
In order to run this program, the following command has to be used:
```
python supepmem_analysis.py
         -tpr SYSTEM_STRUCTURE.tpr
         -xtc TRAJECTORY.xtc
         -f   $PATH/TO/FILES
         -o   $PATH/TO/OUTCOME
         -dt  SIMULATION_TIMESTEP
         -it  INITIAL_TIME_SIMULATION
         -lt  LAST_TIME_SIMULATION
         -st  SKIP_TIME_BETWEEN_FRAMES
         -ait INITIAL_TIME_AVERAGES
         -alt LAST_TIME_AVERAGES
         -ast SKIP_TIME_BETWEEN_FRAMES_AVERAGING
```
This will execute the program and all the statistic calculations will also be performed. It is **important** to point out that in order to...




## Wiki 📖

Additional information about SuPepMem can be found in our [Wiki](https://github.com/DanielCondeTorres/SuPepMem/wiki) (...Work in progress...) as well as on the [SuPepMem](https://supepmem.com/) website itself.


<!-- DISTRIBUTION OF TASKS -->
## Distribution of tasks ✒️ 
Project coordinator: Ángel Piñeiro, M.Bastos and Rebeca García-Fandino

- Main program (Python program): Fabián Suarez-Leston
- Collaborators: G.F Tolufashe, A.Muñoz, U.Veleiro, M.Calvelo
- Creation of the SuPepMem website: C.Porto
- GitHub Designer: Daniel Conde Torres and Alejandro Seco


<!-- FAQs -->
## FAQs :interrobang:

### What is SuPepMem?

SuPepMem is a living project. It is expected to grow with simulations of more peptides in different membrane models and using different atomistic and coarse grained force fields. 

<p align="center">
  <img src="https://user-images.githubusercontent.com/117435891/199971517-f9f27119-0f85-4f91-8f05-e9b48a32f27c.png" />
</p>

### Can I use the analysis scripts with other force fields?
...


<!-- CONTRIBUTING -->
## Contributing 🖇️
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

<!-- Cite --> 
## Cite :mortar_board:

[Citation: F. Suarez-Leston, M. Calvelo, G. F Tolufashe, A. Muñoz, U. Veleiro, C. Porto, M. Bastos, Á. Piñeiro, R. Garcia-Fandino, SuPepMem: A database of innate immune system peptides and their cell membrane interactions, Comput. Struct. Biotechnol. J. 2022, 20, 874-881](https://www.sciencedirect.com/science/article/pii/S2001037022000320)

<!-- License --> 
## License :green_book:
Data in SuPepMem is made available under an CCBY 4.0 License. You are entitled to access and use the services and download or extract data. If you need the data from the SuPepMem Database for research, please cite our publications.
