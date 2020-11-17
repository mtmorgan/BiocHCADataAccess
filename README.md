# Accessing Human Cell Atlas Data in R / Bioconductor

## Key resources

- [Workshop material][] (this resource)
- [GitHub][] source code.

[Workshop material]: https://mtmorgan.github.io/BiocHCADataAccess
[GitHub]: https://github.com/mtmorgan/BiocHCADataAccess

## Demo description

Human Cell Atlas single cell data can be easily represented in R /
Bioconductor data structures, opening the door for extensive
downstream exploration, analysis, and visualization. This
demonstration consists of the following sections.

- [Part A][]: Representing single cell data in R / Bioconductor -- the
  [SingleCellExperiment][].

- [Part B][]: Web-based data discovery, download, and import using [HCAMatrixBrowser][].

- [Part C][]: Programmatic analysis using [HCAExplorer][].

- [Part D][]: Integration with R / Bioconductor single cell workflows outlined in
  the online resource '[Orchestrating Single Cell Analysis with
  Bioconductor][OSCA]'.

- [Part E][]: Future developments.

[Part A]: articles/A_SingleCellDataRepresentation.html
[Part B]: articles/B_HCADataDiscovery.html
[Part C]: articles/C_ProgrammaticExploration.html
[Part D]: articles/D_OSCA.html
[Part E]: articles/E_Directions.html

### Instructors

- [Martin Morgan][]

[Martin Morgan]: mailto:mtmorgan.bioc@gmail.com

### *R* / *Bioconductor* packages used

These packages are the focus of this workshop:

- [HCAMatrixBrowser][]
- [HCAExplorer][]
- [SingleCellExperiment][]
- [LoomExperiment][]
- [OSCA][]

[HCAMatrixBrowser]: https://bioconductor.org/packages/HCAMatrixBrowser
[HCAExplorer]: https://bioconductor.org/packages/HCAExplorer
[SingleCellExperiment]: https://bioconductor.org/packages/SingleCellExperiment
[LoomExperiment]: https://bioconductor.org/packages/LoomExperiment
[OSCA]: https://bioconductor.org/books/3.12/OSCA

## Installation

The material in this demonstration uses the current release version of
Bioconductor. Install R-4.0.3 and Bioconductor 3.12 following [these
instructions][]. Configure your R session for use with Bioconductor
3.12, and enabling installation of GitHub-based packages, with the
following instructions

```
if (!"BiocManager" %in% rownames(installed.packages()))
    install.packages("BiocManager", repos = "https://cran.r-project.org")
BiocManager::install(version = "3.12")

if (!"remotes" %in% rownames(installed.packages()))
    BiocManager::install("remotes")
```

Use `BiocManager::install()` to install and manage R and Bioconductor
packages. Using [BiocManager][] ensures that packages are always
installed from the correct Bioconductor release. The packages required
for this demonstration can be installed from GitHub repository

```
BiocManager::install("mtmorgan/BiocHCADataAccess")
```

[these instructions]: https://bioconductor.org/install/

