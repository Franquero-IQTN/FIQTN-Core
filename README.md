# FIQTN-Core

[![ORCID](https://img.shields.io/badge/ORCID-0009--0002--6534--8924-A6CE39?logo=orcid&logoColor=white)](https://orcid.org/0009-0002-6534-8924)

**Core computational models, differential equations, and preprints for the Franquero Institute for Quantum-Thermodynamic Neuroscience (IQTN)**

Maintained by Keny Wayne Franquero · [ORCID 0009-0002-6534-8924](https://orcid.org/0009-0002-6534-8924) · [Franquero's Prototyping Laboratories LLC](https://franquerolabs.com) · Contact: [keny@franquerolabs.com](mailto:keny@franquerolabs.com)

---

## What is this?

The Franquero Institute for Quantum-Thermodynamic Neuroscience (IQTN) is a virtual research hub developing quantitative frameworks at the intersection of quantum biology, thermodynamics, and theoretical neuroscience.

This repository hosts the simulation code and numerical methods underlying those frameworks. It is organized as a working research codebase, not a packaged library — expect frequent revisions as models evolve and predictions are refined.

---

## Frameworks

### FMQC — Franquero Model of Quantum-Thermodynamic Consciousness

A hypothesis-generating quantum-thermodynamic framework proposing that sustained conscious processing requires a low-entropy, quantum-coherent substrate (plausibly within neural microtubules) actively protected from thermal decoherence by a biological cooling and routing system — cerebrospinal fluid flow, astrocytic heat transport, and mitochondrial thermogenic switching.

The model is formalized as a modified stochastic Kuramoto network with temperature-dependent classical and quantum coupling, a homeostatic adaptation variable, and thalamocortical pacemaker forcing. Simulations reproduce four clinical signatures: sharp global bifurcation at a critical temperature, graceful focal degradation, topological hub vulnerability, and hysteretic anesthetic recovery.

**Status:** Preprint, v1.1 · [Zenodo DOI](https://doi.org/10.5281/zenodo.23244798)

### FEF — Franquero Entropy Framework

A foundational physics framework deriving quantum evolution from entropic gradient flow, replacing the frozen-time Wheeler–DeWitt constraint with evolution along relative entanglement entropy. Provides a first-principles derivation of the decoherence superoperator used phenomenologically in FMQC.

**Status:** Preprint, v1.0 · [Zenodo DOI](https://doi.org/10.5281/zenodo.21910477)

### FDF — Franquero Dynamics Framework

A quantitative computational model for temporal optimization of combination immunotherapy: glycocalyx modification, CD28/4-1BB costimulation, and checkpoint inhibition. Predicts optimal dosing and sequencing to achieve 100% target-cell killing in silico.

**Status:** Provisional patent application, 2026 · [Zenodo DOI](https://doi.org/10.5281/zenodo.21911438)

---

## Repository structure

FIQTN-Core/
├── fmqc/
│   ├── fmqc_figures.py         # Simulation + Figure 1–5 generation
│   ├── requirements.txt        # Python dependencies
│   └── README.md               # FMQC-specific usage notes
├── fef/                        # In progress
├── fdf/                        # In progress
├── figures/                    # Output directory for generated figures
├── docs/                       # Preprints and manuscripts
└── README.md                   # This file

---

## Getting started

### Requirements

- Python 3.9 or later
- NumPy, SciPy, Matplotlib, NetworkX

### Install

```bash
git clone https://github.com/Franquero-IQTN/FIQTN-Core.git
cd FIQTN-Core
pip install -r fmqc/requirements.txt
 
Run the FMQC simulation
cd fmqc
python fmqc_figures.py
 
Outputs five PNG and PDF figures to figures/. Runtime is approximately 3–5 minutes on a standard laptop. 
 
Code principles
• Reproducibility: Deterministic seeds; every run produces identical figures.
• Transparency: All parameters declared in a single dataclass for easy review.
• Modularity: Each figure in its own function; modify one without touching the others.
• Explicit caveats: Models are simplified by design; limitations are documented in the manuscript. 
 
Citation
 
If you use this code or the FMQC framework in your work, please cite:
@misc{franquero_fmqc_2026,
  author       = {Franquero, Keny Wayne},
  title        = {The Franquero Model of Quantum-Thermodynamic Consciousness
                  (FMQC), Version 1.1},
  year         = 2026,
  publisher    = {Zenodo},
  doi          = {10.5281/zenodo.23244798},
  url          = {https://doi.org/10.5281/zenodo.23244798}
}
 
For the entropy framework:
@misc{franquero_fef_2026,
  author       = {Franquero, Keny Wayne},
  title        = {The Franquero Entropy Framework (FEF): Derivation via
                  Variational Principle and Entropic Gradient Flow},
  year         = 2026,
  publisher    = {Zenodo},
  doi          = {10.5281/zenodo.21910477},
  url          = {https://doi.org/10.5281/zenodo.21910477}
}
 
For the dynamics framework:
@misc{franquero_fdf_2026,
  author       = {Franquero, Keny Wayne},
  title        = {The Franquero Dynamics Framework (FDF): A Quantitative Model
                  for Temporal Optimization of Glycocalyx Modification,
                  Costimulation, and Checkpoint Inhibition in Immunotherapy},
  year         = 2026,
  publisher    = {Zenodo},
  doi          = {10.5281/zenodo.21911438},
  url          = {https://doi.org/10.5281/zenodo.21911438}
}
 
 
License
• Documentation and preprints: Creative Commons Attribution 4.0 International (CC BY 4.0)
• Code: MIT License 
See LICENSE for details. 
 
Contributing and collaboration
 
This is currently a single-investigator research repository. Collaboration inquiries, replication attempts, and critical feedback are welcome — please open an issue or email keny@franquerolabs.com.
 
The frameworks are hypothesis-generating, not empirically validated. Contributions that rigorously test, falsify, or refine the predictions are especially encouraged. 
 
Contact
 
Keny Wayne Franquero
Founder, Franquero's Prototyping Laboratories LLC
keny@franquerolabs.com
ORCID: 0009-0002-6534-8924
Franquero-IQTN · Cottonwood, Arizona, USA
