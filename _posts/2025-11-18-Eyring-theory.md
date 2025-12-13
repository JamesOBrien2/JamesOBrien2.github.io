---
layout: post
title: Calculating Reaction Rates using Eyring Theory
date: 2025-11-18 14:13:00
description: This is a post describing the steps required for calculating Reaction Rates using Eyring Theory.
tags: Tutorial
categories: tutorials
---

# Eyring Theory

The Eyring equation is based on Transition State Theory and is used for describing the relationship between reaction rates and temperature. Whilst similar to the Arrhenius equation, the Eyring equation can be appled to gas, condensed, and mixed-phase reactions.

$$
\begin{align}
    k=\frac{k_{B}T}{h}e^{-\frac{ΔH^{\ddag}}{RT}}e^{\frac{ΔS^{\ddag}}{R}}\\
\end{align}
$$

Apply this to a typical bimolecular reaction (K is the equilibrium constant):

$$
\begin{align}
    A + B \rightarrow C\\
    K=\frac{[C]}{[A][B]}
\end{align}
$$

Inclusion of a Transition state complex produces the following:

$$
\begin{align}
    A + B \rightleftharpoons AB^\ddag \rightarrow C\\
    K=\frac{[AB^\ddag]}{[A][B]}
\end{align}
$$

The rate of the reaction is equal to the number of activated complexes decomposing to form products.

...

$$
\begin{align}
    rate=\nu[AB^\ddag]\\
    rate=\nu[A][B]K^\ddag\\
    rate=k[A][B]
\end{align}
$$

This can be rewritten as:

$$
\begin{align}
    k=\nu[AB^\ddag]=\nu[A][B]K^\ddag
\end{align}
$$

# Calculating Reaction Rates

## Step 1

- Calculate ...
