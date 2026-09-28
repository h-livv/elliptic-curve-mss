# Conjunctive Hierarchical Multi-Secret Sharing

A minimal SageMath reproduction of the construction presented in:

> **Conjunctive Hierarchical Multi-Secret Sharing Scheme using Elliptic Curves**  
> Mohan Chintamani, Prabal Paul, Laba Sa — *Indian Journal of Pure and Applied Mathematics*, 2024.

## Current Scope

This repository currently implements the foundational parts of the scheme:

- Finite-field and elliptic-curve setup
- Extension field construction
- Level 1 share generation
- Level 2 share generation
- Elliptic-curve point shares \(b_iP\)
- Section 3.2 reconstruction
- Construction of \(Q\)
- Secret recovery using the pairing as a black box

The implementation currently covers **Levels 1 and 2 and one secret**.

## Goal

The purpose is to understand and reproduce the paper's construction from first principles before extending it to:

- Higher hierarchy levels
- Multiple secrets
- Unauthorized-access experiments
- Computational hardness / attacker experiments

## Requirements

- [SageMath](https://www.sagemath.org/)

## Running

```bash
sage level_1_2.sage
```

The code is intentionally kept simple and closely follows the mathematical construction in the paper.