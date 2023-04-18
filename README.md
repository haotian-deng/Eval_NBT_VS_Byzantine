# Eval_NBT_VS_Byzantine

#### Introduction
The source code for the paper "Evaluating Network Boolean Tomography Under Byzantine Attack".

This open-sourced project serves as a comprehensive resource for the source code used in the experiments presented in my paper. It encompasses replicating simulations of various scenarios, including both no-attack and Byzantine-attack scenarios. Additionally, it involves diagnosing the performance of links, evaluating the effectiveness of diagnosis algorithms, and analyzing data statistically, able to be visually represented in figures used in the paper.

#### Directory structure
```
eval_nbt_vs_byzantine/
├── datasets/
│   ├── topology_zoo/
│   └── tree_topo/
│
├── data/
│   └── multiple_topos/
│       ├── even_sampling/
│       │   ├── true_data(no_attack_data)/
│       │   └── attack_data/
│       │       └── freq_topic/
│       │           ├── path/
│       │           └── path_attacks/
│       │               └── attack_data/
│       └── uneven_sampling/
│           └── section_sample_times/
│               ├── true_data/
│               └── attack_data/
│                   └── freq_topic/
│                       ├── path/
│                       └── path_attacks/
│                           └── attack_data/
│
├── analysis/
│   ├── figures/
│   └── statistical_analysis/
│
├── examples/
│   ├── figures/
│   └── statistical_analysis/
│
├── simulation_code/
│
├── analysis_code/
|   ├── statistical_analysis/
|   └── data_visualization/
└── utilities/
```


#### Requirements Installation

```
pip install -r requirements.txt
```

#### Detailed Usage

`Code Part`

- `simulation_code`: This section contains the code used for generating simulated network scenarios.
- `diagnosis_code`: This section includes the code used for diagnosing the performance of links in the simulated scenarios.
- `evaluation_code`: This section contains the code used for evaluating the performance of the diagnosis algorithm.
- `analysis_code`: This section includes the code used for analyzing the data statistically and generating visual plots to facilitate interpretation.
- `utilities`: This section contains code used to abstract the tree topology from mesh topology.
- `example_code`: This section includes simple example code that uses `examples/statistical_analysis` to generate visualization plots.

`Data Part`

- `datasets`: This section includes the utilization of datasets sourced from Topology-Zoo, as well as a tree topology set that has been abstracted from mesh topology to tree topology from Topology-Zoo.
- `data`: This section encompasses the scenarios-simulation data, diagnosis data, and evaluation data that were collected and analyzed during the experiments.
- `analysis`: In this section, the statistical data obtained from the `Data` folder is utilized to generate visual plots for further analysis and interpretation.
- `examples`: This section includes sample analysis data that can be visualized using the `example_code` provided. These examples serve as illustrations of the capabilities of the code and showcase the visualization of statistical data to aid in understanding and interpretation.This part provides directly usable results that can be used as a reference or starting point for further research or analysis.

#### Contribution

We hope that this project will be valuable for researchers and developers interested in replicating the experiments in the paper and evaluating the performance of diagnostic algorithms. Please feel free to contribute to the project or use it for your own research purposes.
