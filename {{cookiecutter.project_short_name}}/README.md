<!--
SPDX-FileCopyrightText:  Open Energy Transition gGmbH

SPDX-License-Identifier: AGPL-3.0-or-later
-->

# {{cookiecutter.project_name}}

<img src="https://raw.githubusercontent.com/open-energy-transition/oet-website/main/assets/img/oet-logo-red-n-subtitle.png" alt="Open Energy Transition Logo" width="260" height="100" align="right">

<!-- Add your badges here
[![REUSE status](https://api.reuse.software/badge/github.com/open-energy-transition/[PROJECT_NAME])](https://api.reuse.software/info/github.com/open-energy-transition/[PROJECT_NAME])
[![REUSE Compliance Check](https://github.com/open-energy-transition/[PROJECT_NAME/actions/workflows/reuse-compliance.yml/badge.svg?event=schedule)](https://github.com/open-energy-transition/[PROJECT_NAME]/actions/workflows/reuse-compliance.yml)
-->


{{cookiecutter.short_description}}

This repository contains the entire project supported by [Open Energy Transition (OET)](https://openenergytransition.org/), including code and report. The philosophy behind this repository is that no intermediary results are included, but all results are computed from raw data and code.

## Repo structure

* `config`: configurations used in the study
* `data`: place for raw data
* `report`: contains all files necessary to build the report; plots and result files are generated automatically
* `workflow`: contains the Snakemake workflow
* `resources`: will contain all results (does not exist initially)

## Getting ready

You need [mamba](https://mamba.readthedocs.io/en/latest/) to run the analysis. Using mamba, you can create an environment from within you can run it:

    mamba env create -f environment.yaml

## Run the analysis

    snakemake -call

This will run all analysis steps to reproduce results and eventually build the report.

To generate a PDF of the dependency graph of all steps `resources/dag.pdf` run:

    snakemake -c1 --use-conda -f dag

## Licenses

See SPDX license identifiers and the folder `./LICENSES`.
