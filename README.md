# Introductory Machine Learning Workshop

**Stage: learning material with legacy notebook code.** This repository is named AzureML, but its inspected artifact is an introductory workshop notebook. It does not demonstrate an Azure service deployment.

## Process

Explore a labeled dataset, prepare feature and target arrays, fit a classifier, then use a separate test split to evaluate predictions. The notebook first demonstrates fitting and predicting, then introduces a stratified training/test split and classification metrics. A later section explores linear regression.

## Problem

A model can appear successful when it is evaluated on the same observations used to fit it. The workshop helps a learner connect input features, a model, held-out evaluation, and the limits of the result.

## Example

The main classification example uses the Iris dataset: 150 flowers, four measurements per flower, and three species. A k-nearest-neighbors classifier with three neighbors predicts species from the measurements. The later evaluation uses a stratified 20 percent test split with a fixed random seed. The notebook's deliberately unrealistic test input should not be treated as a meaningful flower prediction.

## Impact

The material provides a concrete path from a table to a prediction and evaluation report. Its intended benefit is understanding model evaluation. No new accuracy result, deployed service, production readiness, or business outcome is claimed from this repository review.

## Confirm

**Learning question:** Can the learner explain why held-out evaluation differs from training-set prediction and interpret a confusion matrix?

**Review evidence:** notebook source was inspected on November 20, 2026; the notebook was not executed end to end. A standalone `break` cell and a removed dataset loader prevent treating it as a current run-all example. Read [compatibility notes](COMPATIBILITY.md) before running sections. A successful rerun should record library versions, the split, and actual metrics.

## Relevant features

| Existing notebook feature | What it teaches |
| --- | --- |
| Iris table and visualizations | Relates measured features to labeled categories |
| k-nearest-neighbors example | Shows a simple supervised classification workflow |
| Stratified training/test split | Separates fitting from evaluation while retaining class representation |
| Accuracy, confusion matrix, and classification report | Makes different aspects of prediction quality visible |
| Legacy regression section | Provides historical learning material that requires modernization |

## Open the material

Read [Intro_to_machine_learning.ipynb](Intro_to_machine_learning.ipynb) in GitHub, Jupyter, or Google Colab. The Colab link is embedded in the notebook. Review compatibility before executing or installing dependencies; a current environment is not pinned here.

The notebook credits Galvanize and Andrew Means. This repository preserves workshop material, with those credits retained. The next improvement is a separately reviewed, reproducible modern version of the Iris section.
