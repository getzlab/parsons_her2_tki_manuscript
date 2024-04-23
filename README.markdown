
This repository contains supplementary code for the Parsons et al. manuscript:

_Genomic mechanisms of resistance to tyrosine kinase inhibitors in HER2 amplified breast cancer._ Parsons et al. 2024

The Jupyter and RMarkdown notebooks in this repository generate the figures shown in the manuscript. 

For questions about the code in this repository, please reach out to David Merrell (merrell@broadinstitute.org).

# How to reproduce manuscript figures

## Clone this repository

`$ git clone git@github.com:getzlab/parsons_her2_tki_manuscript.git`

For the remainder of this document, we assume you've `cd`'d into this directory:

`$ cd parsons_her2_tki_manuscript/`

## Install dependencies

We recommend installing [Miniconda](https://docs.anaconda.com/free/miniconda/miniconda-install/) and [creating a conda environment using the `config.yaml`](https://conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html#creating-an-environment-from-an-environment-yml-file) in this directory.

`$ conda env create -f environment.yml`

## Download data from Zenodo

Data for this repository is stored on Zenodo:

https://doi.org/10.5281/zenodo.11053092

Download the tarball `parsons_her2_tki_data.tar.gz` and unpack it in this directory:

`$ tar -xvzf parsons_her2_tki_data.tar.gz`

At this point, there should be a subdirectory called `data` containing several files:
```
$ ls data/
H_matrix.tsv
ONC_ID_to_Manuscript_ID_mapping_paired.txt
[...]
```

You are now ready to run the notebooks and reproduce the figures.

## Run the notebooks

Here we list the figures and the notebooks that generate them.

[See this information about running Jupyter notebooks.](https://jupyter-notebook-beginner-guide.readthedocs.io/en/latest/execute.html)

[See this information about running RMarkdown notebooks.](https://bookdown.org/yihui/rmarkdown/notebook.html)

### Figure 1
- 1A: This panel was generated using Microsoft PowerPoint (**TODO: cite BioRender for images?**)
- 1B: [comuts.ipynb](comuts.ipynb)
- 1C: [pathways.Rmd](pathways.Rmd)

### Figure 2
- 2A: [comuts.ipynb](comuts.ipynb)
- 2B-D: [copy_number.Rmd](copy_number.Rmd)

### Figure 3
- 3A: [swimmer.ipynb](swimmer.ipynb)
- 3B-G: These panels were generated using Adobe Illustrator. The source data were the outputs of PhylogicNDT, as well as sample and treatment data for the selected participants.

### Figure 4
- 4A: [comuts_brain_mets.ipynb](comuts_brain_mets.ipynb)
- 4B: This panel was generated using PathwayMapper[^1] 

### Supplementary Figure 1
- [copy_number.Rmd](copy_number.Rmd)

### Supplementary Figure 2
- [copy_number.Rmd](copy_number.Rmd)

### Supplementary Figure 3
- 3A-B: [comuts.ipynb](comuts.ipynb)

### Supplementary Figure 4
- [comuts_brain_mets.ipynb](comuts_brain_mets.ipynb)

# Licensing

See LICENSE.txt for details.

[^1]: Istemi Bahceci, Ugur Dogrusoz, Konnor C La, Özgün Babur, Jianjiong Gao, Nikolaus Schultz, PathwayMapper: a collaborative visual web editor for cancer pathways and genomic data, Bioinformatics, Volume 33, Issue 14, July 2017, Pages 2238–2240, https://doi.org/10.1093/bioinformatics/btx149
