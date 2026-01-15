# BLA_1D_Toy_model_example
Bayesian Linear Analysis Application on 1D Toy Model

The 1D Toy model example:
$f(\text{x}) = \sin(2 \pi x), x \in \text{x}$
Emulator specification:
$\text{Cov}[f(x), f(x')] = \sigma^2 \exp{\lbrace - \frac{|x - x^{\prime}|^2}{\theta^2} \rbrace} \\ \text{E}_{D}[f(\text{x})] = \text{E}[f(\text{x})] + \text{Cov}[f(\text{x}), D]\text{Var}^{-1}[D](D-\text{E}[D]) \\ \text{Var}_D[f(\text{x})] = \text{Var}[f(\text{x})] - \text{Cov}[f(\text{x}), D] \text{Var}^{-1}[D]\text{Cov}[D,f(\text{x})]$

We code this toy model in R, so please ensure you have installed R and RStudio (any version is acceptable).
You need to install exterior packages "plgp" (a convenient package to compute the Euclidean distance between each input pair) and "viridisLite" (a package for colour choice when visualising results).
