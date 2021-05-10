# Detect_Symmetry

A python package to perform symmetry detection and generator extraction on raw data. Follows the paper by Sven
Krippendorf and Marc Syvaeri on 
[Detecting symmetries with neural networks](https://iopscience.iop.org/article/10.1088/2632-2153/abbd2d).

### Notes
This project is under heavy development and is therefore not available on PyPi. I would not expect major API breaks but
certainly addition of functionality. 

### Installation
Currently it is only possible to install SymDet from source and it will remain like this until it has been thoroughly
tested on experimental data and a larger number of symmetry groups.

#### Install from source

**pip installation**
```bash
git clone https://github.com/SamTov/SymDet.git
cd SymDet
pip3 install . --user
```

**conda installation**
```bash
git clone https://github.com/SamTov/SymDet.git
cd SymDet
conda create -n SymDet python=3.8
conda activate SymDet
pip3 install .
```

#### Documentation

There is a live version of the documentation hosted at 
[https://symdet.readthedocs.io/en/latest/](https://symdet.readthedocs.io/en/latest/). Alternatively you can build it 
from source using

```bash
cd Symdet/docs
make html
```

You can then browse the documentation locally using your favourite browser.

### Getting started

Because SymDet is not designed for single purpose, you will need to interface with different libraries and classes
directly. This isn't as bad as it sounds and we have a number of tutorials to explain how this works. Broadly there
are two modules relevant to most analysis, these are the analysis and generators modules. 

* **analysis**: This module contains the necessary methods for analyzing raw data and extraction symmetry 
  groups from it.
* **generators**: This module contains all of the modules necessary for extracting Lie group generators from the 
  symmetry groups.
  
 As a first step I would suggest looking at the [examples](https://github.com/SamTov/SymDet/tree/main/examples)
 directory and following along with some tutorials.

#### Comments
This is a really young project and any comments or contributions would be welcome. If you see issues in the
documentation (particularly if you're a mathematician) I would always welcome the feedback.