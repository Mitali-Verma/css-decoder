## Problem Interpretation 
We address the CSS quantum error correction decoding challenge across three sequential stages: 
# Stage 1 (Matrix Learning): 
Recover a hidden CSS parity check matrix H ≈ [[HX, 0], [0, HZ]] through adaptive queries to an oracle, where HX ∈ GF(2)^(15×70) and HZ ∈ GF(2)^(15×70). 
# Stage 2 (Clean Decoding): 
Given a syndrome s from the hidden H, find an error vector e_hat in the correct coset without noise. 
# Stage 3 (Noisy Robust Decoding):
 Under ~13.5% random bit flips in syndromes and extended matrices with redundancy, recover valid error estimates while minimizing redundancy overhead.

## High-Level Method Summary 
1. Stage 1: Basis-vector querying (70 queries for HX, 70 for HZ) + CSS commutation validation + low-weight operator sampling for distance estimation. 
2. Stage 2: GF(2) Gaussian elimination solvers: solve HX·eZ = sX and HZ·eX = sZ independently. 
3. Stage 3: Majority-voting denoising across redundant syndrome bits + Stage 2 decoder on cleaned syndrome + noise rate estimation. 

##  Scoring Summary

| Stage | Base Points | Bonus | Criteria |
|-------|-------------|-------|----------|
| **Stage 1** | 35 | +5 | H equivalence + CSS validity / Distance estimate |
| **Stage 2** | 40 | +5 | Coset correctness / Hamming distance |
| **Stage 3** | 25 | +5 | Coset with efficiency (lower r) / Noise estimate p |
| **TOTAL** | **100** | **+15** | **115 max points** |



