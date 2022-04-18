# Database for Calabi-Yau reflection orientifolds

This database contains Calabi-Yau orientifolds together with their underlying polytope and triangulation data as described in our paper available on the ArXiv: 

Author: Andreas Schachner

E-Mail: &#97;&#110;&#100;&#114;&#101;&#97;&#115;&#46;&#115;&#99;&#104;&#97;&#99;&#104;&#110;&#101;&#114;&#64;&#103;&#109;&#120;&#46;&#110;&#101;&#116;


## How to read the data:

We provide a notebook outlining the format of datafiles contained in the database.

Questions, comments and suggestions can be directed to &#97;&#110;&#100;&#114;&#101;&#97;&#115;&#46;&#115;&#99;&#104;&#97;&#99;&#104;&#110;&#101;&#114;&#64;&#103;&#109;&#120;&#46;&#110;&#101;&#116;.

## Open source code and other databases:

* M. Kreuzer, H. Skarke http://hep.itp.tuwien.ac.at/~kreuzer/CY/

* R. Atlman, J. Carifio, J. Gray, X. Gao, Y. He, V. Jejjala, B. D. Nelson http://www.rossealtman.com/toriccy/ : This database contains all triangulations and geometries obtained from 4D reflexive polytopes in the KS database up to <img src="https://render.githubusercontent.com/render/math?math=\color{white}h^{1,1}=6"> including non-favourable cases which are omitted in our database. Moreover, the authors consider divisor exchange involutions which give rise to non-trivial odd moduli counted by $`h^{1,1}_{-}`$

* F. Carta, J. Moritz and A. Westphal https://www.desy.de/~westphal/orientifold_webpage/cicy_orientifolds.html : 

* CYTools M. Demirtas, L. McAllister, A. Rios-Tascon https://cytools.liammcallistergroup.com :


## Datastructure:

    .
    ├── Data                           # orientifold data ...
    │   └── Complete                   # ... for complete scan for h^1,1<=6
    │          └── h11_2               # ... for <img src="https://render.githubusercontent.com/render/math?math=\color{white}h^{1,1}=2">
    │          └── h11_3               # ... for h^1,1=3
    │          └── h11_4               # ... for h^1,1=4
    │          └── h11_5               # ... for h^1,1=5
    │          └── h11_6               # ... for h^1,1=6
    │          └── h11_7               # ... for h^1,1=7
    │   └── Random                     # ... for random scan for 7<=h^1,1<=12
    │          └── h11_7               # ... for h^1,1=7
    │          └── h11_8               # ... for h^1,1=8
    │          └── h11_9               # ... for h^1,1=9
    │          └── h11_10              # ... for h^1,1=10
    │          └── h11_11              # ... for h^1,1=11
    │          └── h11_12              # ... for h^1,1=12
    └── CY_database_notebook.ipynb     # notebook to read datafiles
    └── README.md                      # Readme file
    
    
