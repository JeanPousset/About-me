# Finite Element Method library

## Description

The goal of this school project was to understand how a Finite Element Modeling (FEM) solver works. To do this, I coded a FEM library from scratch in C, guided by my teacher [Eric DARRIGRAND](https://perso.univ-rennes1.fr/eric.darrigrand-lacarrieu/) and inspired by the architecture of the IRMAR laboratory's FEM library (Melina++ and [XLiFE++](https://xlifepp.pages.math.cnrs.fr/)). For this reason, I cannot make the code public. Instead, there is only this readme file listing the parts covered in this FEM library construction.

- Reading mesh files and constructing the associated digital mesh
- Management of dynamically allocated contiguous C matrices to optimize performance
- Evaluation of basic functions, their gradients and the transformations
- Evaluation strategies for each element, combination to construct the discretization matrix
- Optimized memory storage management of matrices (profile storage, ordered and disordered Morse storage)
- Linear system resolution using Cholesky factorization
- Convergence test on various cases of P1 finite elements (triangle and quadrangle), Neumann and Dirichlet conditions.

## In addition...

This project is divided into several modules to handle every steps needed to solve a physical problem with a Finite Element Method. I have endeavored to make this project as complete as possible. To this end, I have written very detailed documentation using **Doxygen** and created a very robust **makefile**.
