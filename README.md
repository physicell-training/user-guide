# PhysiCell User Guide
This is the home of the future user guide for PhysiCell. 

## Brief overview 

### What is PhysiCell

### About this user guide 
This user guide will teach you how to download and use PhysiCell, as well as document the key classes and functions. Wherever possible, it will demonstrate with specific examples. Please note that this guide will be periodically updated. Users should check PhysiCell.MathCancer.org for the latest version. The PhysiCell method paper was published in [PLoS Computational Biology](). 

## Citing PhysiCell
If you use PhysiCell, please cite it as:

We implemented and solved our model using PhysiCell (Version 1.10.2) [1].

> [1] A. Ghaffarizadeh, R. Heiland, S.H. Friedman, S.M. Mumenthaler and P. Macklin. PhysiCell: an Open Source Physics-Based Cell Simulator for 3-D Multicellular Systems, PLoS Comput. Biol. 14(2): e1005991, 2018. DOI: [10.1371/journal.pcbi.1005991](https://dx.doi.org/10.1371/journal.pcbi.1005991).

Because PhysiCell makes extensive use of BioFVM, we suggest you also cite it:

We implemented and solved the model using PhysiCell (Version 1.10.2) [1], with BioFVM [2] to solve the transport equations.

> [1] A Ghaffarizadeh, R Heiland, SH Friedman, SM Mumenthaler, and P Macklin. PhysiCell: an Open Source Physics-Based Cell Simulator for Multicellular Systems, PLoS Comput. Biol. 14(2): e1005991, 2018. DOI: [10.1371/journal.pcbi.1005991](https://dx.doi.org/10.1371/journal.pcbi.1005991)

> [2] A Ghaffarizadeh, SH Friedman, and P Macklin. BioFVM: an efficient parallelized diffusive transport solver for 3-D biological simulations, Bioinformatics 32(8): 1256-8, 2016. DOI: [10.1093/bioinformatics/btv730](https://dx.doi.org/10.1093/bioinformatics/btv730)

Please remember: if you use an additional addon, please make sure to cite it, too! This is critical for scientific rigor (to correctly document your method), reproducibility, and good academic behavior. We have started testing methods to auto-generate suggested citations for addons; see the auto-generated `CITATION.txt` when you run your model. This will be further developed in future versions of PhysiCell.

## Contents 
### Getting started quickly 
#### Development environment and samples
* [Setup](setup.md)
* [Suggested tools](suggested_tools.md)
* [Sample projects](sample_projects.md)

#### Key PhysiCell components 
* [Microenvironment](microenvironment.md)
* [Cells](cells.md)
* [Cell Phenotype](cell_phenotype.md)
* [Cell state](cell_state.md)
* [Cell functions](cell_functions.md)
* [Coloring functions](coloring_functions.md)

#### Typical workflow 
* [Project template](project_template.md)
* [Defining the microenvironment](define_microenvironment.md)
* [Defining cell definitions](define_cell_definitions.md)
* [Custom code](custom_code.md)
* [Compiling and running](compile_run.md)
* [Quick simulation view](quick_simulation_view.md)
* [Loading data in Jupyter notebooks](loading_data_jupyter.md)

#### Advanced workflows 
* [PhysiBoSS]()

### Helpful tools
* [Graphical model editor](graphical_model_editor.md)
* [Python data loader](python_data_loader.md)
* [ImageMagick]()
* [Code editors]()

### Complete examples 
* [Competing tumor clones](competing_tumor_clones.md)
* [Invading bacteria](invading_bacteria.md)

### Community Gallery 
* [Community Gallery]()

### Deeper technical detail

* [Overall code structure](code_structure.md)
* [Cell class]()
* [Cell_State class]()
* [Cell_Functions class]()
* [Cell_Phenotype class]()
* [Custom_Data class]()

## Training materials 


