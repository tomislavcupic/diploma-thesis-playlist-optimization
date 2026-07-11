# Spotify Playlist Multi-Objective Optimization

This repository contains the implementation, experiments, and accompanying materials for my diploma thesis on **multi-objective optimization of Spotify playlists using evolutionary algorithms**.

## Overview

The objective of this project is to optimize Spotify playlists by simultaneously considering multiple conflicting criteria through **Multi-Objective Evolutionary Algorithms (MOEAs)**.

The project implements and compares three well-known optimization algorithms:

* NSGA-II (Non-dominated Sorting Genetic Algorithm II)
* NSGA-III (Non-dominated Sorting Genetic Algorithm III)
* MOEA/D (Multi-Objective Evolutionary Algorithm based on Decomposition)

The algorithms are evaluated on their ability to generate high-quality Pareto-optimal playlist solutions under different optimization objectives.

---

## Repository Structure

```text
.
├── thesis/                 # Diploma thesis
├── presentation/           # Defense presentation
├── src/                    # Source code
├── data/                   # Datasets and Spotify data
├── experiment_notebook/            # Experiment scripts
├── results/                # Experimental results and figures
└── README.md
```

---

## Project Objectives

The optimization process considers multiple playlist characteristics simultaneously:

* Coherence vector containing:
    - energy
    - positivity
    - loudness
    - tempo
* Playlist diversity of artists
* Popularity

Since these objectives are often conflicting, the algorithms search for a set of Pareto-optimal playlist solutions instead of a single optimal playlist.

---

## Algorithms

### NSGA-II

A fast elitist multi-objective evolutionary algorithm based on:

* Non-dominated sorting
* Crowding distance
* Elitist selection

---

### NSGA-III

An extension of NSGA-II designed for many-objective optimization problems using reference points to improve diversity among solutions.

---

### MOEA/D

A decomposition-based evolutionary algorithm that decomposes the multi-objective problem into multiple scalar optimization subproblems.

---

## Experimental Evaluation

The implemented algorithms are compared using multiple performance indicators, such as:

* Hypervolume (HV)
* Generational Distance (IGD)
* Spread/Diversity metrics

The repository contains the scripts used to reproduce the experiments presented in the thesis.

---

## Running the Project

Clone the repository:

```bash
git clone https://github.com/tomislavcupic/spotify-playlist-multiobjective-optimization.git
cd spotify-playlist-multiobjective-optimization
```

Run the desired experiment:

```bash
python main.py
```

---

## Repository Contents

* Diploma thesis (PDF)
* Thesis defense presentation
* Complete implementation
* Experimental setup
* Evaluation scripts
* Generated results and figures

---

## Technologies

* Python
* Kaggle
* Evolutionary Computation
* Multi-Objective Optimization
* NumPy
* pandas
* matplotlib

---

## Citation

If you use this repository in your work, please cite the accompanying diploma thesis.

---

## License

This repository is intended for academic and research purposes.

If you reuse parts of the implementation, please provide appropriate attribution.
