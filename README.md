<!-- [![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](https://raw.githubusercontent.com/DeMaCS-UNICAL/I-DLV/master/LICENSE) ) -->
[![GitHub release](https://img.shields.io/github/release/DeMaCS-UNICAL/I-DLV.svg)](https://github.com/DeMaCS-UNICAL/I-DLV/releases/latest)
[![GitHub issues](https://img.shields.io/github/issues/DeMaCS-UNICAL/I-DLV.svg)](https://github.com/DeMaCS-UNICAL/I-DLV/issues)
[![I-DLV website](https://img.shields.io/website-up-down-green-red/https/demacs-unical.github.io/I-DLV.svg?label=I-DLV-website)](https://demacs-unical.github.io/I-DLV/)

# I-DLV : the new Intelligent Grounder of DLV

_I-DLV_ is a full-fleged Answer Set Programming and Datalog reasoner. It supports the [ASP-Core-2](https://www.mat.unical.it/aspcomp2013/files/ASP-CORE-2.03c.pdf) standard language; nevertheless, the system supports additional linguistic extensions such as list terms and external atoms. _I-DLV_ is also a full-fledged deductive database system, supporting query answering powered by the Magic Sets technique.

_I-DLV_ has also been integrated as the grounding module of the completely renewed second version of the logic-based Artificial Intelligence system [DLV](https://dlv.demacs.unical.it).

I-DLV is free for academic and non-commerical educational use, as well as for use by non-profit organisations. 

# How to cite I-DLV

[<img src="https://cdn.iconscout.com/icon/free/png-256/quote-16-433627.png" alt title="Cite" width="13" height="13" />](https://dblp.org/rec/bibtex/conf/aiia/CalimeriFPZ16)
[<img src="https://dblp.org/img/paper.dark.hollow.16x16.png" alt title="See on dblp.org" />](https://dblp.org/rec/conf/aiia/CalimeriFPZ16) Francesco Calimeri, Davide Fuscà, Simona Perri, Jessica Zangari: I-DLV: The New Intelligent Grounder of dlv. AI*IA 2016: 192-207

# Publications

[<img src="https://cdn.iconscout.com/icon/free/png-256/quote-16-433627.png" alt title="Cite" width="13" height="13" />](https://dblp.org/rec/bibtex/journals/ia/CalimeriFPZ17)
[<img src="https://dblp.org/img/paper.dark.hollow.16x16.png" alt title="See on dblp.org" />](https://dblp.org/rec/html/journals/ia/CalimeriFPZ17) Francesco Calimeri, Davide Fuscà, Simona Perri, Jessica Zangari: I-DLV: The new intelligent grounder of DLV. Intelligenza Artificiale 11(1): 5-20 (2017)

# Download
You can download the latest stable release of _I-DLV_ in the [release section of github](https://github.com/DeMaCS-UNICAL/I-DLV/releases).

<!-- # Installation
The source code of _I-DLV_ can be downloaded [here](https://github.com/DeMaCS-UNICAL/I-DLV.git).

On Linux O.S. in order to build _I-DLV_ is required g++-4.9 (or more recent) and the tools flex and bison.

It is also required the library [HTD](https://github.com/mabseher/htd/releases), version "htd 1.1 (rc1-bugfix)". 

By typing:

        make

an _I-DLV_ executable file will be generated in the _build/release_ folder.
-->

# Usage as ASP grounder

_I-DLV_ can interoperate with the state-of-the-art solvers [_wasp_](https://github.com/alviano/wasp) and [_clasp_](https://sourceforge.net/projects/potassco/files/clasp/). Indeed, by default _I-DLV_ output is produced in a numeric format compliant with the mentioned solvers. 

In order to interoperate with a solver type:
 
    ./idlv [filename [filename [...]]] | ./solver_executable

In order to obtain the ground program in textual format type:
 
    ./idlv --t [filename [filename [...]]]
    
# Usage as Datalog reasoner 

I-DLV can be also adopted as Datalog reasoner. Indeed, the system when fed with a disjunction-free and stratified under negation program is able to fully evaluate it and compute its perfect model. 

To this end, one can type:

    ./idlv --t [filename [filename [...]]] 
    
In case a query is provided, _I-DLV_ automatically enables the Magic Sets technique; in order to obtain only the query answers as output type: 

    ./idlv --query [filename [filename [...]]]
    
# Guide
  
For a detailed description of _I-DLV_ capabilities please visit the [official guide](https://github.com/DeMaCS-UNICAL/I-DLV/wiki).

# Core Team

* [Francesco Calimeri](https://www.mat.unical.it/calimeri) 
* [Francesco Pacenza](https://francescopacenza.it)
* Simona Perri
* [Jessica Zangari](https://sites.google.com/view/jessica-zangari/home-page)

# Members

* Antonino Agostino
* Bruno Barbara
* Giuseppe Benvenuto
* Davide Fuscà
* Nicola Greco
* Elena Mastria
* Giovanni Melissari
* Matteo Perfidio
* Agostino Rizzo

For additional details and bug report, please write to i-dlv@googlegroups.com. 

