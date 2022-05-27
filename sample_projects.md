# Sample projects
PhysiCell includes several sample projects to illustrate capabilities and suggest modeling possibilities. 


## Working with sample projects 
In general, building and running these projects consists of the following steps:

1. **Populate a project:** Use the following Makefile rule (from a terminal / command project in your PhysiCell root directory):

    ```
    make project_name
    ```

    where `project_name` is one of the sample projects listed below. For example, to populate the "cancer biorobots" sample project:

    ```
    make cancer-biorobots-sample
    ```

1. **Build the project:** Just run make:

    ```
    make
    ```

1. **Run the project:** Run the executable created by the compiler. If the name of the program is `PROGRAM_NAME`, run

    ```
    ./PROGRAM_NAME
    ```

    (Windows users should omit the `./`.)

    As of Version 1.10.0, each PhysiCell sample project displays the name of the executable as the final step of compiling. 

    One simple way to determine the name of the executable is to use grep on the Makefile:

    ```
    grep PROGRAM_NAME Makefile
    ```

    For example, to run the cancer biorobots example, the executable name is `cancer_biorobots`, so you run:

    ```
    ./cancer_biorobots
    ```

    The project will create a series of SVG images files, as well as MultiCellDS save files (a combination of matlab and XML files). It will also place a copy of your configuration file in the output directory. See [???]() and the [PhysiCell blog]().

1. **(Optional) Clear your data to prepare for a new run:** If you want to clean up your data, use: 

    ```
    make data-cleanup
    ```

    This clears all data from your output directory. 

1. **(Optional) Clear out the project / return to a clean slate:** If you want to build and run a different sample project, or clear out the sample materials to create your own, you need to "depopulate" the sample project:

    ```
    make reset
    ```

## Sample projects included in every download 
Here are the sample projects included as of Version 1.10.0:

* `biorobots-sample` is a 2-D example of 3 cell types: cargo cells, worker cells (which seek out cargo
cells and haul them to a destination), and director cells (which attract worker cells).
* `cancer-biorobots-sample` extends the biorobots example to (1) simulate a 2-D tumor that develops a necrotic core, (2) so that cargo cells are hauled towards hypoxic tumor regions, and (3) so
that released cargo cells secrete a chemotherapeutic compounds.
* `heterogeneity-sample` simulates a 2-D tumor with heterogeneous “genetics” that drive differential
proliferation.
* `cancer-immune-sampl`e extends the heterogeneity example to 3D, and introduces a new immune
cell type (modeling T cells) that migrate towards tumor cells, temporarily adhere, test for immunogenicity, and initiate apoptosis.
* `virus-macrophage-sample` simulates a basic virus that diffuses, is uptaken by cells, replicates, and
then is released in cell lysis. Macrophages eat and degrade infected cells. This is a test of internalized
substrate tracking first released in PhysiCell 1.5.0.
* `beta-testing` is a small project that can be used for beta testing new features. Don’t count on it
remaining unchanged from release to release.
* `template` is the template for creatiung a new 2D or 3D project. 
See [???](). 
