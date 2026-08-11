# healthMaps
Code and data resources for a constraint-based framework to diagnose mobility-solvable gaps in healthcare accessibility.

# A constraint-based framework reveals mobility-solvable gaps in healthcare accessibility

This repository contains the code, analytical workflow, and supporting resources associated with the study:

**“A constraint-based framework reveals mobility-solvable gaps in healthcare accessibility”**

The study develops a constraint-based framework for diagnosing why geographic healthcare accessibility gaps persist. Rather than treating poor accessibility as a uniform deficit, the framework distinguishes between accessibility gaps that may be alleviated through improved mobility and those that remain constrained by insufficient healthcare supply.

Using nationwide geocoded healthcare facilities, population data, and large-scale routing-based travel-time estimates across walking and motorized travel scenarios, the analysis characterizes geographic healthcare accessibility across China and identifies heterogeneous accessibility constraints.

## Overview

The framework is designed to move healthcare accessibility assessment from identifying **where access is poor** toward diagnosing **why access gaps arise**.

The main analytical components include:

* construction and processing of a nationwide healthcare facility inventory;
* population-based origin locations for accessibility assessment;
* large-scale routing-based travel-time estimation;
* comparison of walking and motorized healthcare accessibility;
* identification of mobility-solvable and persistent accessibility gaps;
* characterization of accessibility constraints associated with healthcare supply, terrain, and transport networks;
* classification of geographic accessibility regimes;
* constraint-aware allocation analysis for evaluating alternative intervention strategies.

## Key concept

A central distinction in this study is between different types of healthcare accessibility deficits.

**Mobility-solvable gaps** refer to populations that experience poor accessibility under walking conditions but can reach healthcare services within the specified threshold under motorized travel.

**Persistent accessibility gaps** refer to populations that remain poorly served even after accounting for motorized mobility, indicating stronger constraints associated with healthcare supply, geographic remoteness, transport infrastructure, or their interaction.

This distinction provides a basis for separating areas where improving mobility may substantially enhance healthcare access from areas where additional healthcare provision or broader infrastructure investment may be required.

## Data

The study integrates multiple nationwide datasets, including:

* geocoded healthcare facility locations;
* gridded population distributions;
* road-network-based travel-time estimates;
* terrain characteristics;
* transport-network indicators;
* administrative boundaries and related geographic information.

The full analysis includes **544,528 geocoded healthcare facilities** and approximately **177.9 million origin-to-facility routing-based travel-time estimates**.

Due to licensing, redistribution, privacy, or data-provider restrictions, some original datasets may not be directly distributed through this repository. Where possible, links, processing instructions, derived data, or reproducible workflows will be provided.

## Repository structure

The repository will be organized approximately as follows:

```text
.
├── code/
│   ├── preprocessing/
│   ├── accessibility/
│   ├── constraint_classification/
│   ├── allocation/
│   └── figures/
│
├── data/
│   ├── example/
│   ├── derived/
│   └── metadata/
│
├── results/
│   ├── tables/
│   └── figures/
│
├── docs/
│
├── README.md
└── LICENSE
```

The structure may be updated as the repository is finalized.

## Reproducibility

Scripts required to reproduce the principal analyses and figures will be organized by analytical step.

The workflow broadly follows:

```text
Healthcare facilities + Population
                │
                ▼
      Origin–facility routing
                │
                ▼
       Travel-time accessibility
        /                     \
   Walking                 Motorized
        \                     /
                ▼
       Constraint diagnosis
                │
                ▼
 Mobility-solvable / Persistent gaps
                │
                ▼
      Accessibility regimes
                │
                ▼
   Constraint-aware allocation
```

Additional documentation describing input requirements, parameter settings, intermediate outputs, and figure reproduction will be added as the repository is finalized.

## Main findings

The analysis shows that geographic healthcare accessibility deficits do not necessarily represent the same underlying problem.

At the national scale, approximately **310.4 million people** were estimated to live beyond a 60-minute walking accessibility threshold. However, approximately **83.0%** of this walking-defined underserved population could reach healthcare services within 30 minutes under the motorized travel scenario.

These results indicate that a large proportion of apparent accessibility deficits may be potentially alleviated through improvements in mobility rather than through healthcare facility expansion alone.

The study further shows that walking and motorized accessibility are associated with different geographic constraints. Walking accessibility is more strongly related to local healthcare facility availability, whereas motorized accessibility increasingly reflects the combined effects of terrain and transport-network conditions.

In the allocation analysis, a constraint-aware strategy produced substantially greater modelled potential coverage gains than a conventional need-based allocation approach.

## Citation

If you use the code, workflow, or derived resources from this repository, please cite the associated article.

Citation information will be updated upon publication.

```text
Jiang, X. et al. A constraint-based framework reveals mobility-solvable gaps in healthcare accessibility.
```

## Code and data availability

The repository is being prepared to support transparency and reproducibility of the study.

Code associated with the main analytical workflow and figure generation will be made available here. Availability of individual datasets will depend on their original licensing and redistribution conditions.

For datasets that cannot be redistributed directly, we will provide source information and processing instructions where permitted.

## License

A license for the publicly released code will be specified before the final release of the repository.

Please refer to the `LICENSE` file for the applicable terms of use.

## Contact

For questions regarding the study, code, or data resources, please contact the corresponding authors or open an issue in this repository.

