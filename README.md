# BLA_1D_Toy_model_example
Bayesian Linear Analysis Application on 1D Toy Model

The 1D Toy model example:
$f(\text{x}) = \sin(2 \pi \text{x})$

Emulator specification:

$\text{Cov}[f(\text{x}), f(\text{x}')] = \sigma^2 \exp{\lbrace - \frac{|\text{x} - \text{x}^{\prime}|^2}{\theta^2} \rbrace}; $

$\text{E}_{D}[f(\text{x})] = \text{E}[f(\text{x})] + \text{Cov}[f(\text{x}), D]\text{Var}^{-1}[D](D - \text{E}[D]); $

$\text{Var}_D[f(\text{x})] = \text{Var}[f(\text{x})] - \text{Cov}[f(\text{x}), D] \text{Var}^{-1}[D]\text{Cov}[D,f(\text{x})]$.

Implausibility Measure (for History Matching):
$I^{2}(x)=\frac{(\text{E}_D[f(\text{x})]-z)^2}{\text{Var}_D[f(\text{x})] + \text{Var}[\epsilon] + \text{Var}[e]}$

We code this toy model in R, so please ensure you have installed R and RStudio (any version is acceptable).
You need to install the exterior package "plgp" (a convenient package that computes the Euclidean distance between each pair of inputs).

Note: This repository provides an independent, minimal implementation of the emulator by Bayes Linear Analysis for illustrative purposes only. It does not reproduce or redistribute any teaching or tutorial code used in supervised coursework or internal research workflows. Standard numerical linear algebra methods (e.g., computing the inverse matrix by using solve()) are common in textbooks and public software implementations.)
