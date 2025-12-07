Project Overview

This repository provides two datasets and a complete implementation for software requirement prioritization using multiple artificial intelligence and optimization techniques. The project integrates K-Means clustering with four prioritization methods: Particle Swarm Optimization (PSO), Fuzzy Logic, a replacement-based biological Genetic Algorithm method (RBM-GA), and the Adaptive KGAPSO–Fuzzy hybrid technique.
The purpose of this project is to offer a publicly accessible, reproducible framework for evaluating requirement prioritization across a wide range of dataset sizes.

Datasets
Dataset 1: Online Case Study Dataset

Dataset 1 is derived from real-world online case studies.
It contains Excel files with two primary attributes for each requirement:

Technical Dependency (scaled 1–5)

User Preference (scaled 1–5)

These values reflect realistic requirement characteristics from actual systems.

Dataset 2: Synthetic Dataset

Dataset 2 is synthetically generated to provide controlled variability and scalability.
It includes the same two attributes (technical dependency and user preference, both scaled 1–5) but allows consistent testing across a variety of dataset sizes.

Dataset Availability

Both datasets are provided as Excel files with sizes ranging from:
20, 50, 100, 200, 500, 1000, 1500, and 2000 requirements.

These datasets are publicly accessible and allow analysis on both real-world and synthetic requirement sets.

Rationale for Using Both Datasets

Using both real and synthetic datasets provides the following advantages:

Generalization Assessment: Performance of prioritization techniques can be validated across natural and artificially generated patterns.

Scalability Evaluation: Larger synthetic datasets enable testing of algorithm behavior at high volumes.

Benchmarking: Availability of two dataset types ensures stronger comparison across different algorithmic approaches.

Reproducibility: Synthetic datasets allow consistent replication of experiments.

Methodology and Code Functionality

The Python/Colab implementation follows a structured sequence:

1. Data Loading

Users manually upload Dataset 1 or Dataset 2 (Excel format).
The program extracts the technical dependency and user preference columns.

2. Preprocessing

Values are normalized using standard scaling techniques to ensure fair comparison between attributes.

3. Clustering Using K-Means

K-Means clustering is used to group requirements into three clusters.
Clustering enhances accuracy by:

Grouping similar requirements

Reducing computational load

Allowing independent prioritization of each cluster

4. Prioritization Techniques

Each cluster is prioritized using four different algorithms:

PSO (Particle Swarm Optimization)

An optimization method inspired by swarm intelligence; used to determine an optimal prioritization sequence.

Fuzzy Logic Method

Handles uncertainty using fuzzy membership values, generating flexible prioritization scores.

Replacement-Based Biological Genetic Algorithm (RBM-GA)

A genetic algorithm that incorporates biological replacement strategies to improve convergence.

Adaptive KGAPSO–Fuzzy Technique

A hybrid model combining:

K-Means clustering

Genetic Algorithm

PSO

Fuzzy Logic

This technique adapts based on cluster performance and produces the highest prioritization accuracy among the tested methods.

5. Final Score Calculation

A combined priority score is generated for each requirement using weighted contributions from:

Technical dependency

User preference

The final prioritized list includes:

Priority score

High/medium/low priority categories

Accuracy and computation time evaluations

Project Purpose

This project provides a validated, reproducible system for requirement prioritization research.
It enables users to analyze multiple prioritization approaches, test scalability, and benchmark performance on datasets of varying sizes.

Why This Project Is Useful

Offers publicly available datasets for academic and industrial research

Provides a complete pipeline for requirement prioritization

Supports testing of multiple AI-based optimization strategies

Includes hybrid techniques not commonly documented together

Getting Started
1. Clone or download the repository:
git clone https://github.com/Rahila7/KPSO-FUZZY/new/Dataset-1-and-Dataset-2-and-Final-Code

2. Open the provided Google Colab notebook.

The notebook guides users through:

Uploading datasets

Running clustering

Applying all four prioritization techniques

Exporting prioritized results

3. Upload Dataset 1 or Dataset 2 in Excel format.

The program processes any dataset size within the repository.

Support and Help

Users may request assistance by opening an issue in this repository.
Support is available for:

Dataset questions

Code execution

Algorithm behavior

Bug reports

Contributors and Maintenance

This project is maintained by:

Rahila Anwar

Contributions are welcome through pull requests and issue submissions.

Enables comparison of accuracy and computation time
