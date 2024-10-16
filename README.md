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

Follow the setup guide. The project will be named `[PROJECT NAME]` in the next steps.

Once the repository is created, move into the folder.

    cd [PROJECT NAME]

Create a new project on GitHub and push the new repository.

    git init
    git add -A
    git commit -m "Initial commit"
    gh repo create

Follow the setup guide.

Set up [pre-commit.ci](https://pre-commit.ci/).

## Project Structure

The generated repository will have the following structure:

```

|____config
| |____config.yaml
|____data
| |____.gitkeep
|____LICENCES
| |____AGPL-3.0-or-later.txt
| |____CC0-1.0.txt
| |____CC-BY-4.0.txt
|____report
| |____sections
| | |____abstract.tex
| | |____conclusion.tex
| | |____discussion.tex
| | |____introduction.tex
| | |____methods.tex
| | |____results.tex
| | |____supplementary.tex
| | |____.gitkeep
| |____static
| | |____.gitkeep
| |____references.bib
| |____report.tex
|____resources
| |____.gitkeep
|____results
| |____.gitkeep
|____workflow
| |____envs
| | |____.gitkeep
| |____notebooks
| | |____.gitkeep
| |____plots
| | |____.gitkeep
| |____rules
| | |____.gitkeep
| |____scripts
| | |____dummy.py
| |____submodules
| | |____.gitkeep
| |____Snakefile
|____.github
| |____workflows
| | |____reuse-compliance.yml
|____.reuse
| |____dep5
|____environment.yaml
|____matplotlibrc
|____README.md
|____.gitattributes
|____.gitignore
|____.pre-commit-config.yaml
|____.syncignore-receive
|____.syncignore-send

```

## License

This cookiecutter template is forked and modified from [PyPSA/cookiecutter-project](https://github.com/PyPSA/cookiecutter-project). This template is MIT licensed itself.
