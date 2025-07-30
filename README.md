# space-behaviour

Mechanistic simulation framework tracing how spaceflight-related exposures—especially radiation—propagate from first-principles physics to biological and cognitive outcomes.

## Purpose

This project builds an open, falsifiable, end-to-end model that maps:

radiation tracks → molecular damage → gene network response → synaptic degradation → working-memory decline

It serves as both a scientific tool and a proof-of-concept for applying theoretical modeling to psychiatric and cognitive risk in spaceflight.

## Structure

- meta/ — planning documents (workflow.md, workflow-condensed.md)
- modules/ — core simulation code
- notebooks/ — interactive Julia notebooks for each module
- data/ — radiation spectra, chromatin maps, gene parameters
- figures/ — plots for reports and manuscripts

## MVP Roadmap (12 months)

| Phase | Module                        | Output                        |
|-------|-------------------------------|-------------------------------|
| Q1    | Dose → DNA                    | dose_to_damage.ipynb         |
| Q2    | p53 SDE model                 | p53_ensemble.ipynb           |
| Q3    | Synapse loss + graph rewiring| tracks_to_tasks.ipynb        |
| Q4    | Reservoir net + demo         | Public v0.1 release + paper  |

See meta/workflow-condensed.md for full milestone breakdown.

## Julia Stack

- DifferentialEquations.jl – radiation + GRN dynamics  
- Graphs.jl – neural circuits  
- Flux.jl – reservoir computing  
- Makie.jl – interactive visualization  
- Agents.jl – optional cell population modeling  

## Long-Term Vision

This repo begins with radiation exposure but will expand to include other space stressors (e.g., microgravity, circadian disruption) and their cognitive/psychiatric effects.

It lays the foundation for a general-purpose simulation engine for space-behaviour coupling.
