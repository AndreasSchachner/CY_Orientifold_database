# CQSV Database for Calabi-Yau Reflection Orientifolds

This database contains Calabi-Yau orientifolds and their underlying polytope and triangulation data as described in our paper available on the ArXiv: [ArXiv](https://arxiv.org).

Authors: Chiara Crinò, Fernando Quevedo, Andreas Schachner, Roberto Valandro

Contact E-Mail: &#97;&#110;&#100;&#114;&#101;&#97;&#115;&#46;&#115;&#99;&#104;&#97;&#99;&#104;&#110;&#101;&#114;&#64;&#103;&#109;&#120;&#46;&#110;&#101;&#116;

## Available data

The database contains the following data:

* <b>Polytope data</b>: We present the data of favourable 4D reflexive polytopes obtained from the [KS database](http://hep.itp.tuwien.ac.at/~kreuzer/CY/) together with the GLSM charge matrix, Hodge numbers and Euler characteristics.

* <b>Triangulation data</b>: Utilising [CYTools](https://cytools.liammcallistergroup.com), we computed fine, regular, star triangulations (FRSTs) of favourable polytopes. Our database contains information about the simplices used for each FRST as well as about the 2nd Chern class, the SR ideal and triple intersection numbers.

* <b>Orientifolds</b>: We provide information about the O-plane configurations for reflection involutions z_i -> z_i of a single toric coordinate z_i. We computed the D3-charges from Op-planes and D7-branes where we cancel the D7-tadpole in two ways:
    - locally with SO(8)-stacks or 
    - non-locally using fully recombined Whitney branes.
    
* <b>Fibrations</b>: By looking for 2D reflexive sub-polytopes using the algorithm of [1907.09482](https://inspirehep.net/literature/1745921), we determined the possible genus one fibrations.

* <b>Divisor topologies</b>: We computed the Hodge numbers for all prime toric divisors together with their Euler number and arithmetic genus. 

* <b>Diagonal divisors</b>: We check the presence of diagonal del Pezzo divisors necessary to realise the [LVS](https://inspirehep.net/literature/676185).

## How to read the data

We provide a notebook outlining the format of datafiles contained in the database.

Questions, comments and suggestions can be directed to &#97;&#110;&#100;&#114;&#101;&#97;&#115;&#46;&#115;&#99;&#104;&#97;&#99;&#104;&#110;&#101;&#114;&#64;&#103;&#109;&#120;&#46;&#110;&#101;&#116;.


## Employed open-source software

The following open-source projects were used in generating this database and the publication: 

* [Sage](https://www.sagemath.org) and [CYTools](https://cytools.liammcallistergroup.com) for polytope and triangulation data

* modified version of [TOPCOM](http://www.rambau.wm.uni-bayreuth.de/TOPCOM/) [[GPLv2](http://www.gnu.org/licenses/gpl-2.0.html)] that can be found [here](https://github.com/LiamMcAllisterGroup/topcom)

* the [Computational Geometry Algorithms Library](https://www.cgal.org) [[LGPLv3](http://www.gnu.org/licenses/lgpl-3.0.html)]

* multiple Python packages including [SciPy](https://www.scipy.org/), [NumPy](https://numpy.org/), [pplpy](https://gitlab.com/videlec/pplpy), [OR-Tools](https://developers.google.com/optimization), [scikit-sparse](https://github.com/scikit-sparse/scikit-sparse), [pandas](https://pandas.pydata.org), [matplotlib](https://matplotlib.org), [seaborn](https://seaborn.pydata.org) and [flint-py](https://gitlab.com/alisianoi/flint-py).


## Datastructure:

    .
    ├── Data                           # orientifold data ...
    │   └── Complete                   # ... for complete scan of triangulation data for h^1,1<=7
    │          └── h11_2               # ... for h^1,1=2
    │          └── h11_3               # ... for h^1,1=3
    │          └── h11_4               # ... for h^1,1=4
    │          └── h11_5               # ... for h^1,1=5
    │          └── h11_6               # ... for h^1,1=6
    │          └── h11_7               # ... for h^1,1=7
    │   └── Random                     # ... for random scan of triangulation data for 7<=h^1,1<=12
    │          └── h11_7               # ... for h^1,1=7
    │          └── h11_8               # ... for h^1,1=8
    │          └── h11_9               # ... for h^1,1=9
    │          └── h11_10              # ... for h^1,1=10
    │          └── h11_11              # ... for h^1,1=11
    │          └── h11_12              # ... for h^1,1=12
    └── CY_database_notebook.ipynb     # notebook with instructions to read data files
    └── README.md                      # readme file
    

<br>
<br>
<br>

# Useful packages and related databases:

The list below contains software and databases which are related to our data.

## Open source code and tools:

### CYTools

Authors: M. Demirtas, L. McAllister, A. Rios-Tascon 

Website: [CYTools](https://cytools.liammcallistergroup.com) and [GitHub](https://github.com/LiamMcAllisterGroup/cytools)

Description: CYTools is a powerful software package developed by the group of L. McAllister at Cornell University specifically designed to study Calabi-Yau manifolds arising from the Kreuzer-Skarke database. Among others, it enables us to compute triangulations efficiently for any value of <img src="https://render.githubusercontent.com/render/math?math=\color{white}h^{1,1}\leq 491">. We utilised this package to manipulate polytope data and to compute triangulations.


### CohomCalg

Authors: R. Blumenhagen, B. Jurke, T. Rahn, H. Roschy

Website: [cohomCalg](https://github.com/BenjaminJurke/cohomCalg)

Description: Efficient tool to computing sheaf cohomologies for line bundles on toric varieties.


## CY manifold and orientifold databases:

### KS database:

Authors: M. Kreuzer, H. Skarke

Website: [KS database](http://hep.itp.tuwien.ac.at/~kreuzer/CY/)

Description: The database contains among others a classification of 4D and 5D reflexive polytopes with the former being heavily used in developing this database. Further, it provides information on the classification scheme for reflexive polyhedra and data of Landau-Ginzburg models and reflexive Gorenstein cones. 

### CICY threefold database:

Authors: P. Candelas, A. M. Dale, C. A. Lutken, R. Schimmrigk

Website: [CICY threefolds](http://www-thphys.physics.ox.ac.uk/projects/CalabiYau/cicylist/)

Description: A list of all 7,890 Calabi-Yau manifolds defined as complete intersections in products of projective spaces.

### CICY fourfold database:

Authors: J. Gray, A. S. Haupt, A. Lukas

Website: [CICY fourfolds](http://www-thphys.physics.ox.ac.uk/projects/CalabiYau/Cicy4folds/index.html)

Description: A complete list of 921,497 Calabi-Yau four-folds defined as complete intersections in products of projective spaces.

### AGHJN database:

Authors: R. Altman, J. Carifio, J. Gray, X. Gao, Y. He, V. Jejjala, B. D. Nelson 

Website: [AGHJN database](http://www.rossealtman.com/toriccy/)

Description: This database contains all triangulations and geometries obtained from 4D reflexive polytopes in the [KS database](http://hep.itp.tuwien.ac.at/~kreuzer/CY/) up to <img src="https://render.githubusercontent.com/render/math?math=\color{white}h^{1,1}=6"> including non-favourable cases which are omitted in our database. Moreover, the authors consider divisor exchange involutions which give rise to non-trivial <img src="https://render.githubusercontent.com/render/math?math=\color{white}h^{1,1}_{-}">.

### CICY orientifold database:

Authors: F. Carta, J. Moritz and A. Westphal 

Website: [CICY orientifold database](https://www.desy.de/~westphal/orientifold_webpage/cicy_orientifolds.html)

Description: A database of orientifolds obtained from both favourable and non-favourable CICY threefolds. It includes both reflection and exchange involutions. They apply their database to checking the necessary conditions for ultra-light throat axions (thraxions) as proposed in [1812.03999](https://arxiv.org/abs/1812.03999).


