# ChemE-as-Code

**Chemical plant design as code.** A process plant kept as plain files in a git repository:
P&IDs in DEXPI 2.0.1, engineering lists in YAML, decisions in Markdown. Engineers and AI coding
agents edit the same files, and every change is checked, reviewed and versioned like software.

The example designs in the [Process Atlas](https://atlas.cheme-as-code.org) were produced by AI
agents under human direction and are not approved for construction, operation or safety
decisions.

## What you can do with it

- **Draw and check P&IDs** as text: validation with file and line, a formatter that keeps diffs
  small, rendering and a visual diff between revisions.
- **Design the process**: block and process flow diagrams from YAML, stream tables with the
  source of every value, simulation in DWSIM, reactions, kinetics and reactors.
- **Lay out the plant in 3D**: equipment, pipe routes, steel, cable trays and ducts, with clash
  and access checks.
- **Assess it**: equipment datasheets and cost estimates, material take-off, techno-economic
  analysis and life cycle assessment.
- **Review it** in the browser with the read-only [Viewer](https://github.com/ChemE-as-Code/core/tree/main/viewer).

## Repositories

| | |
|---|---|
| [`core`](https://github.com/ChemE-as-Code/core) | the `cheme` command-line tool, the skills for AI agents and the web Viewer (`viewer/`) |
| [`project-template`](https://github.com/ChemE-as-Code/project-template) | an empty plant: press **Use this template** to start one |
| [`process-library`](https://github.com/ChemE-as-Code/process-library) | example plant designs, one folder per process, e.g. an air separation unit |

## Getting started

1. Install the tool: `uv tool install git+https://github.com/ChemE-as-Code/core.git`
2. Start a plant: **Use this template** on [`project-template`](https://github.com/ChemE-as-Code/project-template),
   or `cheme init my-plant`.
3. Work in it with your editor or a coding agent; run `cheme validate` after every change.

## Who we are

ChemE-as-Code is developed by the [Process Intelligence Research](https://www.pi-research.org/)
group at the Department of Chemical Engineering, Delft University of Technology, led by
[Artur M. Schweidtmann](https://www.tudelft.nl/tnw/over-faculteit/afdelingen/chemical-engineering/principal-scientists/artur-schweidtmann).

## Contributors

| | Name | Role |
|---|---|---|
| <img src="https://raw.githubusercontent.com/ChemE-as-Code/core/main/.github/readme/schweidtmann.jpg" alt="Artur M. Schweidtmann" width="50"> | [Artur M. Schweidtmann](https://www.pi-research.org/author/artur-schweidtmann/) | ChemE-as-Code and Process Atlas (principal investigator) |
| <img src="https://raw.githubusercontent.com/ChemE-as-Code/process-library/main/.github/readme/weber.jpg" alt="Jana M. Weber" width="50"> | Jana M. Weber | Process Atlas |
| <img src="https://raw.githubusercontent.com/ChemE-as-Code/core/main/.github/readme/alimin.png" alt="Achmad A. Alimin" width="50"> | [Achmad A. Alimin (Angga)](https://www.pi-research.org/people/achmad-a-alimin/) | Safety and HAZOP; layout STL export |
| <img src="https://raw.githubusercontent.com/ChemE-as-Code/core/main/.github/readme/rupprecht.jpg" alt="Sophia Rupprecht" width="50"> | [Sophia Rupprecht](https://www.pi-research.org/people/sophia-rupprecht/) | Inherited thermodynamic model selection, phase calculations, units and skills; design case study |
| <img src="https://raw.githubusercontent.com/ChemE-as-Code/core/main/.github/readme/evanvoorbergen.png" alt="Elise" width="50"> | [Elise](https://github.com/evanvoorbergen) | Inherited reaction identification, kinetics retrieval, filtering and unit conversion |

## Status and license

Research preview: research output, not engineering advice. [`core`](https://github.com/ChemE-as-Code/core)
is licensed under AGPL-3.0-or-later; the process data and designs in
[`process-library`](https://github.com/ChemE-as-Code/process-library) under CC BY 4.0. Each
repository states its full terms.
