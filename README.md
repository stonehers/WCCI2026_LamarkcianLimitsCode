![ariel-header](./docs/resources/ariel_header.svg)

# ARIEL: Autonomous Robots through Integrated Evolution and Learning

> **WCCI 2026 Submission**
> This repository contains the code for the paper: *"The Limits of Lamarckian Evolution Under the Pressure of Morphological Novelty"*

## Repository Structure

```
.
├── myevo/                      # Main experiment code
│   ├── core/                   # Evolution strategies and main experiment script
│   │   ├── mu_lambda_tree_locomotion.py  # Main entry point
│   │   ├── mu_lambda.py        # (μ+λ) and (μ,λ) evolution strategies
│   │   ├── tree_genotype.py    # Tree-based morphology representation
│   │   ├── fitness_evaluator.py # Robot fitness evaluation
│   │   ├── weight_inheritance.py # Lamarckian weight inheritance
│   │   └── cmaes_inheritance.py  # CMA-ES state inheritance
│   ├── controllers/            # Neural network controllers
│   ├── measures/               # Fitness functions (locomotion, novelty)
│   ├── simulation/             # MuJoCo simulation utilities
│   └── config/                 # Configuration
├── src/ariel/                  # ARIEL framework (robot phenotypes, simulation)
├── examples/                   # Example scripts
└── docs/                       # Documentation
```

<!-- ## Requirements

* [vscode](https://code.visualstudio.com/)
  * [containers ext](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers)
  * [container tools ext](https://marketplace.visualstudio.com/items?itemName=ms-azuretools.vscode-containers)

* Container manager:
  * [podman desktop](https://podman.io/)
  * [docker desktop](https://www.docker.com/products/docker-desktop/)
  
* [vscode containers tut](https://code.visualstudio.com/docs/devcontainers/tutorial)

--- -->
## Installation and Running

This project uses [uv](https://docs.astral.sh/uv/).

To run the code examples please do

```bash
uv venv
uv sync
uv run examples/0_render_single_frame.py
```

<!-- ## TODO: Installation

## Notes

### This project is managed using `uv`

### Python Code Style Guide

This repository uses the `numpydoc` documentation standard.
For more information checkout: [numpydoc-style guide](https://numpydoc.readthedocs.io/en/latest/format.html#) -->

<!-- ### Units

To ensure that Ariel uses a consistent set of units for all simulations, we use [SI units](https://www.wikiwand.com/en/articles/International_System_of_Units), and (astropy)[https://docs.astropy.org/en/stable/index.html] to enforce it (we automatically convert where we can).

For more information, see: [astropy: units and quantities](https://docs.astropy.org/en/stable/units/index.html) and [astropy: standard units](https://docs.astropy.org/en/stable/units/standard_units.html#standard-units). -->

<!-- ### MuJoCo

#### Attachments

Robot parts should be attached using the `site` functionality (from body to body), while robots should be added to a world using the `frame` functionality (from spec to spec).

- [Python → Attachment](https://mujoco.readthedocs.io/en/stable/python.html#attachment)
- [mjsFrame](https://mujoco.readthedocs.io/en/stable/APIreference/APItypes.html#mjsframe)

NOTE: when attaching a body, only the contents of `worldbody` get passed, meaning that, for example, `compiler` options are not!

---

## IMPORTANT!!

Change the default configuration of vscode dev containers to accept podman!

Either by the settings gui:

![vscode-podman-settings](./docs/resources/vscode-podman-settings.png)


## Running the code

* In general you can run the currently open python script via the command palette (`cmd+shift+p`): 
  * `Tasks: Run Task` -> `Run script: uv run {$file}`

### Run GUI: 

* via terminal

```bash
uv run src/ariel/gui_code/litegraph/main.py
```

### Run EA Example

```bash
uv run src/ariel/ec/a004.py
```

### Run MuJoCo Example(s)a

Any from the `examples/` folder

For example (pun intended):

```bash
uv run examples/_hi_prob_dec.py
```

## Neat commands!

### Grab `requirements.tex` automatically
```bash
uv add tool pipreqs
pipreqs path/to/parse --mode no-pin --force
uv add -r requirements.txt
``` -->


