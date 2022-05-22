# cookiecutter-project

Forked and modified from [timtroendle/cookiecutter-reproducible-research](https://github.com/timtroendle/cookiecutter-reproducible-research).

This repository provides [cookiecutter](http://cookiecutter.readthedocs.io) templates for reproducible research projects.
Projects build with these templates aim at full automation, and use `Python`, `mamba/conda`, `Git`, `Snakemake`, and `Latex` to create a PDF report out of raw data, code, and text. 

## Getting Started

Make sure you have cookiecutter installed, otherwise install it with [conda](https://conda.io/docs/index.html):

    conda install cookiecutter -c conda-forge

Then create a repository using:

    cookiecutter gh:fneum/cookiecutter-project

## Project Structure

The generated repository will have the following structure:

```

|____LICENSE.md
|____workflow
| |____rules
| | |____.gitkeep
| |____subworkflows
| | |____.gitkeep
| |____scripts
| | |____dummy.py
| |____notebooks
| | |____.gitkeep
|____.syncignore-receive
|____report
| |____report.tex
| |____sections
| | |____results.tex
| | |____abstract.tex
| | |____.gitkeep
| | |____supplementary.tex
| | |____introduction.tex
| | |____discussion.tex
| | |____conclusion.tex
| | |____methods.tex
| |____static
| | |____.gitkeep
| |____report.bib
|____results
| |____.gitkeep
|____data
| |____.gitkeep
|____.github
| |____workflows
| | |____.gitkeep
|____matplotlibrc
|____Snakefile
|____config
| |____config.yaml
|____environment.yaml
|____.reuse
| |____dep5
|____CITATION.cff
|____.syncignore-send
|____envs
| |____dag.yaml
|____resources
| |____.gitkeep
|____.gitattributes
|____README.md
|____.pre-commit-config.yaml
|____.gitignore
```

## License

This cookiecutter template is forked and modified from[timtroendle/cookiecutter-reproducible-research](https://github.com/timtroendle/cookiecutter-reproducible-research). This template is MIT licensed itself.
