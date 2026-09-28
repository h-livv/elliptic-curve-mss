# Elliptic Curve Multi-Secret Sharing

Reproduction of Chintamani, Paul, and Sa's Conjunctive Hierarchical Multi-Secret Sharing Scheme using Elliptic Curves.

## Scope

This repository contains an **end-to-end scoped reproduction of the scheme through Level 2**, implemented in SageMath.

The current implementation reproduces:

- Construction of the finite fields and elliptic curve used in the paper
- Generation of Level 1 shares
- Generation of Level 2 shares
- Distribution of elliptic-curve point shares
- Reconstruction of the hidden coefficient points from authorized shares
- Construction of $Q$
- Pairing-based secret recovery
- Recovery of the secret $K_1$

The implementation therefore follows the complete path

$$
\text{construction}\rightarrow \text{share distribution} \rightarrow \text{authorized reconstruction}\rightarrow Q \rightarrow K_1.
$$

The current scope is limited to **Levels 1 and 2 and one secret**.

## Next Steps

- Extend the implementation to additional secrets
- Implement the remaining hierarchy levels
- Reproduce the paper's full numerical example
- Investigate the scheme from an external attacker's perspective

## Requirements

- [SageMath](https://www.sagemath.org/)

## Running

```bash
sage level_1_2.sage
```

## Reference

Mohan Chintamani, Prabal Paul, Laba Sa,  
*Conjunctive Hierarchical Multi-Secret Sharing Scheme using Elliptic Curves*,  
Indian Journal of Pure and Applied Mathematics, 2024.
