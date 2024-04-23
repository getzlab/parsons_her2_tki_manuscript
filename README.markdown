
This repository contains supplementary code for the Parsons et al. manuscript:

_Genomic mechanisms of resistance to tyrosine kinase inhibitors in HER2 amplified breast cancer. Parsons et al. 2024_

The Jupyter and RMarkdown notebooks in this repository generate the figures shown in the manuscript. 

For questions about the code in this repository, please reach out to David Merrell (merrell@broadinstitute.org).


# How to reproduce manuscript figures

## Clone this repository

`$ git clone git@github.com:getzlab/parsons_her2_tki_manuscript.git`

For the remainder of this document, we assume you've `cd`'d into this directory:

`$ cd parsons_her2_tki_manuscript.git`

## Install dependencies

We recommend installing [Miniconda](https://docs.anaconda.com/free/miniconda/miniconda-install/) and [creating a conda environment using the `config.yaml`](https://conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html#creating-an-environment-from-an-environment-yml-file) in this directory.

`$ conda env create -f environment.yml`

## Download data from Zenodo

Data for this repository is stored on Zenodo:

TODO ADD ZENODO REPOSITORY URL

Download the tarball `parsons_her2_tki_data.tar.gz` and unpack it in this directory:

`$ tar -xvzf parsons_her2_tki_data.tar.gz`

At this point, there should be a subdirectory called `data` containing several files:
```
$ ls data/
all_mut_ccfs_maf_bl_geneLists_evidenceLevels.pkl
cnas_paired_all_annot_ptlevel.tsv
[...]
```

You are now ready to run the notebooks and reproduce the figures.

## Run the notebooks

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
- 4B: This panel was generated using PathwayMapper (**TODO: cite PathwayMapper?**)

### Supplementary Figure 1
- [copy_number.Rmd](copy_number.Rmd)

### Supplementary Figure 2
- [copy_number.Rmd](copy_number.Rmd)

### Supplementary Figure 3
- 3A-B: [comuts.ipynb](comuts.ipynb)

### Supplementary Figure 4
- [comuts_brain_mets.ipynb](comuts_brain_mets.ipynb)

## Licensing

See LICENSE.txt for details.
