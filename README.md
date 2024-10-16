# cookiecutter-project

Forked and modified from [PyPSA/cookiecutter-project](https://github.com/PyPSA/cookiecutter-project).

This repository provides [cookiecutter](http://cookiecutter.readthedocs.io) templates for reproducible projects.
Projects build with these templates aim at full automation, and use `Python`, `mamba/conda`, `Git`, `Snakemake`, and `Latex` to create a PDF report out of raw data, code, and text. 

## Getting Started

Make sure you have cookiecutter installed, otherwise install it with [mamba](https://mamba.readthedocs.io/en/latest/):

    mamba create -n cookiecutter cookiecutter -c conda-forge
    mamba activate cookiecutter

Then create a repository using:

    cookiecutter gh:open-energy-transition/cookiecutter-project

Follow the setup guide.

Once the repository is created, move into the folder.

    cd [PROJECT NAME]

Create a new project on GitHub and push the new repository.

    git init
    git commit -A -m "Initial commit"
    gh repo create

Follow the setup guide.

Set up [pre-commit.ci](https://pre-commit.ci/).

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
