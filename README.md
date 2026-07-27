# CryoEM Refinement Utilities

<p align="center">
  <a href="#license"><img src="https://img.shields.io/badge/license-pending-0E7C66.svg" alt="License"></a> <a href="#paper-or-reference"><img src="https://img.shields.io/badge/paper-reference-1F4E79.svg" alt="Paper or reference"></a> <img src="https://img.shields.io/badge/language-Python-3776AB.svg" alt="Python">
</p>

<p align="center">
  <strong>Conference-style artifact for cryo-EM refinement and FSC diagnostics.</strong>
</p>

<p align="center">
  <img src="assets/readme-figure.png" alt="CryoEM Refinement Utilities overview" width="100%">
</p>

## Abstract

This repository is organized as a conference-style artifact for cryo-EM refinement experiments. It is written for a reviewer or collaborator who wants to identify the exact entry points, understand the expected outputs, and reproduce the core evidence without reverse-engineering the folder layout. The central question is: **How can refinement variants be inspected with lightweight scripts and reconstruction-quality diagnostics?**

## Contribution Summary

- Separate entry points for volume-level and point-level refinement.
- FSC plotting utility for quality checks.
- Small script surface for reviewer inspection.

## Artifact at a Glance

| Item | Details |
| --- | --- |
| Research question | How can refinement variants be inspected with lightweight scripts and reconstruction-quality diagnostics? |
| Primary contribution | Separate entry points for volume-level and point-level refinement; FSC plotting utility for quality checks; Small script surface for reviewer inspection |
| Main entry points | `e2gmm_refine.py`, `e2gmm_refine_point.py`, `my_plotfsc.py` |
| Runtime | Python with NumPy, SciPy, and Matplotlib |
| Data expectation | Experiment-specific cryo-EM inputs configured locally |
| Expected evidence | Refinement artifacts and FSC-style diagnostic plots |

## Repository Structure

| Item | Details |
| --- | --- |
| Entry points | `e2gmm_refine.py`, `e2gmm_refine_point.py`, `my_plotfsc.py` |
| Experiment assets | Experiment-specific cryo-EM inputs configured locally |
| Generated artifacts | Refinement artifacts and FSC-style diagnostic plots |
| Documentation role | README records the reproducibility protocol, reviewer-facing checks, and citation metadata |

## Reproducibility Protocol

1. Clone the repository: `git clone git@github.com:Hik289/cryoem_new.git`.
2. Prepare the runtime listed in **Artifact at a Glance**.
3. Start from the main entry points rather than auxiliary folders.
4. Run the smallest script or notebook first to verify local paths and package versions.
5. Record the command, data window, random seed, machine type, and software versions for each full run.
6. Store regenerated figures, logs, tables, checkpoints, or reports in named output folders so the original artifacts remain inspectable.

## Evaluation Protocol

| Check | Expected reviewer action |
| --- | --- |
| Entry-point clarity | Confirm the listed scripts or notebooks are the natural starting points. |
| Minimal execution | Run a small case before attempting the full experiment. |
| Output traceability | Map every regenerated output back to a command and data setting. |
| Result inspection | Compare generated artifacts with the expected evidence listed above. |
| Extension hygiene | Add new experiments as clearly named scripts, notebooks, or output folders. |

## Expected Results

A successful reproduction should produce or refresh the following evidence: Refinement artifacts and FSC-style diagnostic plots. If local datasets or machine-specific paths are required, document those paths outside the committed code before sharing the artifact.

## Known Limitations

- Large datasets, private data paths, and machine-specific settings may need local configuration.
- Some historical notebooks or scripts may reflect exploratory runs; prefer the entry points listed above for review.
- For archival release, add a pinned environment file and a small public fixture when possible.

## Paper or Reference

No external paper link is currently attached to this project. Cite the repository snapshot when using the artifact in academic work.

## Citation

If a paper is attached, cite the paper first and this artifact second. Otherwise cite the repository snapshot used for the experiment.

```bibtex
@misc{cryoem_new_artifact_2026,
  title = {{CryoEM Refinement Utilities}},
  author = {Hik289},
  year = {2026},
  howpublished = {\url{https://github.com/Hik289/cryoem_new}},
  note = {Conference-style research artifact}
}
```

## License

No explicit license file is included yet. Add one before public reuse, redistribution, or package release.

## Reviewer Checklist

| Claim | Inspection path |
| --- | --- |
| Code availability | Core scripts, notebooks, and utilities are tracked in this repository. |
| Reproducibility | The protocol above states setup, entry points, and output expectations. |
| Data transparency | Local or private data dependencies should be documented before external release. |
| Result traceability | Generated outputs should live in named result, report, log, checkpoint, or output folders. |
