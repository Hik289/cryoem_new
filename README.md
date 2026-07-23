# CryoEM Refinement Utilities

<p align="center">
  <a href="#license"><img src="https://img.shields.io/badge/license-pending-0E7C66.svg" alt="License"></a> <a href="#paper-or-reference"><img src="https://img.shields.io/badge/paper-reference-1F4E79.svg" alt="Paper or reference"></a> <img src="https://img.shields.io/badge/language-Python-3776AB.svg" alt="Python">
</p>

<p align="center">
  <strong>Python scripts for cryo-EM refinement experiments and FSC visualization.</strong>
</p>

<p align="center">
  <img src="assets/readme-figure.png" alt="CryoEM Refinement Utilities overview" width="100%">
</p>

The overview figure highlights the intended loop: load particle or volume representations, refine the model, measure reconstruction quality, and inspect FSC curves before the next run.

## Overview

This project groups lightweight refinement scripts for cryo-EM experiments, with separate entry points for volume-level and point-level refinement plus plotting utilities for Fourier shell correlation diagnostics.

## What Is Included

- `e2gmm_refine.py`: main refinement script for the reconstruction workflow.
- `e2gmm_refine_point.py`: point-based refinement variant for geometry-focused experiments.
- `my_plotfsc.py`: utility for plotting FSC-style quality curves.

## Quick Start

1. `git clone git@github.com:Hik289/cryoem_new.git`
2. `python -m venv .venv && source .venv/bin/activate`
3. `python -m pip install -U pip numpy scipy matplotlib`
4. Run the refinement scripts with the dataset paths required by your experiment environment.

## Suggested Workflow

1. Start with the smallest runnable script or notebook listed above.
2. Keep raw data paths and credentials outside the repository.
3. Save generated figures, tables, and reports under the existing result folders.
4. When an experiment becomes stable, record the exact data window, parameters, and command used to reproduce it.

## Repository Map

- `assets/readme-figure.png`: README overview figure.
- Project scripts and notebooks: core research entry points.
- Result or report folders: generated artifacts used for analysis and review.

## Paper or Reference

No external paper link is currently attached to this project. For now, the code, notebooks, and notes in this repository are the primary reference artifact.

## License

No explicit license file is included yet. Add one before public reuse, redistribution, or package release.

## Maintenance Notes

- Add a pinned environment file if this project is prepared for external installation.
- Keep large datasets outside Git and document where each script expects them locally.
- Prefer small, named experiment outputs over overwriting shared result files.
