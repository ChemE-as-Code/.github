# ChemE-as-Code

**Chemical plant design as code.** A process plant kept as plain files in a git repository:
P&IDs in DEXPI 2.0.1, engineering lists in YAML, decisions in Markdown. Engineers and AI coding
agents edit the same files, and every change is checked, reviewed and versioned like software.

## What you can do with it

- **Draw and check P&IDs** as text: validation with file and line, a formatter that keeps diffs
  small, rendering and a visual diff between revisions.
- **Design the process**: block and process flow diagrams from YAML, stream tables with the
  source of every value, simulation in DWSIM, reactions, kinetics and reactors.
- **Lay out the plant in 3D**: equipment, pipe routes, steel, cable trays and ducts, with clash
  and access checks.
- **Assess it**: equipment datasheets and cost estimates, material take-off, techno-economic
  analysis and life cycle assessment.
- **Review it** in the browser with the read-only viewer.

## Repositories

| | |
|---|---|
| [`core`](https://github.com/ChemE-as-Code/core) | the `cheme` command-line tool and the skills for AI agents |
| [`project-template`](https://github.com/ChemE-as-Code/project-template) | an empty plant: press **Use this template** to start one |
| [`process-library`](https://github.com/ChemE-as-Code/process-library) | real plants, one folder per process, e.g. an air separation unit |
| [`viewer`](https://github.com/ChemE-as-Code/viewer) | a web viewer for a plant repository |

## Getting started

1. Install the tool: `uv tool install git+https://github.com/ChemE-as-Code/core.git`
2. Start a plant: **Use this template** on [`project-template`](https://github.com/ChemE-as-Code/project-template),
   or `cheme init my-plant`.
3. Work in it with your editor or a coding agent; run `cheme validate` after every change.

## Who we are

ChemE-as-Code is developed by the [Process Intelligence Research](https://www.pi-research.org/)
group at the Department of Chemical Engineering, Delft University of Technology, led by
[Artur M. Schweidtmann](https://www.tudelft.nl/tnw/over-faculteit/afdelingen/chemical-engineering/principal-scientists/artur-schweidtmann).

> Status: research prototype. <!-- EDIT before going public: release state and licence -->
