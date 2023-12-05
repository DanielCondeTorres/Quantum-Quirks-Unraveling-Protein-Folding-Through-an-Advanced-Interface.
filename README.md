# Quantum Quirks Unraveling Protein Folding Through an Advanced Interface.
Modification of the IBM public code by adding protein folding in different phrases as well as the study of folding at a polar/apolar interface.

<p align="center">
  <img src="https://github.com/DanielCondeTorres/Quantum-Quirks-Unraveling-Protein-Folding-Through-an-Advanced-Interface./assets/117435891/456188df-bc99-4fa7-adcd-7449412f5ee3" />
</p>







  
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
In this repository, quantum computational methods have been developed and optimised to efficiently and accurately address the folding of amino acid sequences (peptides) at a polar/apolar interface, emulating a realistic model of the water/membrane interface, which is fundamental to understand the structure and function of Antimicrobial Peptides (AMPs) in specific biological contexts. It also allows the study of folding in both polar and non-polar monophases.

<!-- Pre-requirements -->
## General Pre-requirements :computer:

In order to run the program it is necessary to have the following requirements installed:

The program is written in Python language so Python version 3 or higher is required. Also, for python programs to work properly the following libraries are needed:
- [Qiskit](https://www.ibm.com/quantum/qiskit)
- [Matplotlib](https://matplotlib.org)
- [Numpy](https://numpy.org)
- [Re](https://docs.python.org/3/library/re.html)
- [Os](https://docs.python.org/3/library/os.html)
- [Mayavi](http://docs.enthought.com/mayavi/mayavi/)
- [Imageio](https://pypi.org/project/imageio/) 
- [Sys](https://docs.python.org/3/library/sys.html)
- [Time](https://docs.python.org/3/library/time.html)
- [Collections](https://docs.python.org/3/library/collections.html)
- [Glob](https://docs.python.org/3/library/glob.html)
- [Fileinput](https://docs.python.org/es/3/library/fileinput.html)


To be able to use these libraries, it is recommended to work with anaconda environment.


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


<!-- Required-files -->
## Required files 📋
No external file is required.

<!-- Usage -->
## Usage ⚙️
In order to run this program, the following command has to be used:
```
make run # To perform the search for the most stable state of your amino acid sequence
make representation # To get a picture of the most stable structure of your system.
make plots # It allows to obtain the evolution of the energy with the number of iterations.
```
### In the main.py file, in the inputs section we can choose:
  INPUTS:
  
    * main_chain: string            # amino acid sequence
    * ws_phase_1: float             # average interaction of an amino acid with solvent in phase 1
    * ws_phase_2: float             # average interaction of an amino acid with solvent in phase 2
    * cs_phase_1: float             # model solvent in phase 1
    * cs_phase_2: float             # model solvent in phase 2
    * exchange_solvent: float       # energy exchange between interfaces
    * correction_mj: bool           # indicates whether we decide to use the Miyazawa-Jerningan potential upgrade or not.
    * one_solvent_parameter: bool   # These options do not affect the calculation of two phases, is only if we want to add a parameter to modulate the interaction of amino acids according to their hydrophobicity value with the phase.
    * penalty_back: float           # A penalty parameter used to penalize turns along the same axis. This term is used to eliminate sequences where the same axis is chosen twice in a row. In this way we do not allow for a chain to fold back into itself.
    * penalty_chiral: float         # A penalty parameter used to impose the right chirality.
    * penalty_1: float              # A penalty parameter used to penalize local overlap between beads within a nearest neighbor contact.
    * maxiter: float                # Number of iterations to be performed.


Not interface when: 

```
cs_phase_1 == cs_phase_2 and ws_phase_1 == ws_phase_2
```

The original IBM work can be obtained by setting up:

```
* ws_1 = ws_2
* cs_1 = cs_2
* exchange_sovent_solvent = 0
* correction = False
* one_solvent_paramenter = False
* penalty_back = 10
* penalty_chiral = 10
* penalty_1 = 10
```


## In the qiskit_research/protein_folding/interface_bead_interaction/interface_parameters.py file:
Allows us to modify different parameters related to the creation of the interface.

``` 
* displacement_of_the_interface_plane: float  # Value for the displacement of the interface plane. 
* axis: int                                   # Axis perpendicular to the interface.  Axis to be selected for defining the plane of the interface: The possible values are 0, 1, 2 or 3.
* cls._instance._weight_interface: abs(float) # Value for the importance of the interface. Initial value must be positive!
```             

Value for the weight to be given to the interface Hamiltonian:

* If weight_interface > 0, the hydrophobic solvent goes below the plane and the hydrophilic solvent goes on top.
* If weight_interface < 0, the hydrophobic solvent  goes on top of the plane and the hydrophilic solvent goes below.

The sign will be given according to the selected values of phase 1 cs and phase 2 cs: 

```
if cs_phase_1 > cs_phase_2:
    mj_modified_parameters = -1
elif cs_phase_2 > cs_phase_1:
    mj_modified_parameters = 1
```

Therefore, in the first case the importance of the interface will be cls._instance._weight_interface *-1 and in the second case cls._instance._weight_interface*1.


# Quantum simulation parameters

Brief summary:

* cs > 0: model hydrophilic solvents (water)
* cs < 0: model hydrophobic solvents (oil)

* w: describes the average interaction of an amino acid with solvent
* w > 0: aminoacids repel the solvent
* w < 0:  aminoacids interact on average attractively with the solvent






## Wiki 📖

Additional information about SuPepMem can be found in our [Wiki](https://github.com/DanielCondeTorres/SuPepMem/wiki) (...Work in progress...) as well as on the [SuPepMem](https://supepmem.com/) website itself.


<!-- DISTRIBUTION OF TASKS -->
## Distribution of tasks ✒️ 
Project coordinator: Ándres Gómez, Ángel Piñeiro and Rebeca García-Fandino

- Main program (Python program): Daniel Conde-Torres, Mariamo Mussa-Juane, Daniel Faílde, Ángel Piñeiro, Ándres Gómez, Ángel Piñeiro and Rebeca García-Fandino
- GitHub Designer: Daniel Conde-Torres, Mariamo Mussa-Juane and Daniel Faílde


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
