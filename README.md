# AM-Window-ICF-Framework
REPO 2 — NPA-D-26-00134 (Framework théorique)
# Angular-Momentum-Windowed Phenomenological Framework for CF/ICF

**Manuscript:** An Angular-Momentum-Windowed Phenomenological Framework for
Complete and Incomplete Fusion of α-Cluster Projectiles

**Authors:** Ntumba Lobo, Ashok Kumar Chaubey, Edmond Phuku Phuati,
Jérémie Muswema, Patrick Dedetemo Kimilita, Emmanuel Ndiadia Kandolo

**Journal:** Nuclear Physics A (Manuscript No. NPA-D-26-00134)

---

## Overview

This repository contains supplementary numerical materials for the
angular-momentum-windowed phenomenological framework extending the
Hauser–Feshbach (HF) formalism to include incomplete fusion (ICF)
of α-cluster projectiles.

## Framework Summary

The framework partitions entrance-channel partial waves into:
- **Low-ℓ window** [0, ℓ_cr]: Complete fusion (CF) — standard HF
- **High-ℓ window** [ℓ_cr+1, ℓ_g]: Peripheral break-up → partial fusion (ICF)

The geometric weight of the high-ℓ window:

  w_HL = (ℓ_g² - ℓ_cr²) / ℓ_g²

is approximately mass-independent (~0.56) across a factor 7 in target mass.

## Key Results (Table 1 of manuscript)

| System | C* | V_CB (MeV) | ℓ_cr (ℏ) | ℓ_g (ℏ) | w_HL |
|--------|----|------------|----------|---------|------|
| 20Ne+27Al | 47V | 30.3 | 20 | 30 | 0.56 |
| 20Ne+59Co | 79Rb | 55.7 | 35 | 53 | 0.56 |
| 20Ne+93Nb | 113Sb | 77.8 | 48 | 72 | 0.56 |
| 20Ne+197Au | 217Fr | 128.5 | 75 | 113 | 0.56 |

At nominal parameters (r₀=1.07 fm, a=0.63 fm, E/V_CB=2.0, γ=0.66).

## Sensitivity Analysis Summary (Table 3 of manuscript)

| Quantity | 20Ne+27Al | 20Ne+59Co | 20Ne+93Nb | 20Ne+197Au |
|----------|-----------|-----------|-----------|------------|
| w_HL nominal | 0.56 | 0.56 | 0.56 | 0.56 |
| w_HL min–max | 0.46–0.72 | 0.43–0.70 | 0.44–0.69 | 0.43–0.70 |
| w_HL spread | 0.25 | 0.27 | 0.25 | 0.27 |
| ℓ_cr nominal | 20 | 35 | 48 | 75 |
| ℓ_cr min–max | 15–24 | 26–42 | 36–57 | 55–90 |

**Robust conclusion:** w_HL is approximately mass-independent (±0.02 across systems).
**Fragile conclusion:** Absolute value of w_HL carries ±0.13 uncertainty (dominated by γ).

## Parameters

| Parameter | Nominal | Range tested |
|-----------|---------|-------------|
| r₀ (nuclear radius) | 1.07 fm | 1.00–1.15 fm |
| a (surface diffuseness) | 0.63 fm | 0.55–0.75 fm |
| E/V_CB | 2.0 | 1.5–2.5 |
| γ (ℓ_cr/ℓ_g ratio) | 0.66 | 0.55–0.75 |

## LMT Recovery Conditions

The LMT ansatz is recovered as a special case under two **additional** assumptions:

1. **Assumption 2 (Saturated break-up):** P_BU^(k)(ℓ,E) → 1 throughout [ℓ_cr+1, ℓ_g]
2. **Assumption 3 (Geometric–mass identification):** w_HL = F^(k*) = A_f^(k*)/A_p

Note: w_HL ≈ 0.56 for ²⁰Ne-induced reactions, which differs from all four
LMT mass fractions F ∈ {0.20, 0.40, 0.60, 0.80}.
LMT recovery requires γ ≈ 0.63 for F=0.60 (16O break-up mode), approximately satisfied.

## Three Testable Consequences

1. **Mode ranking:** σ_BU^(k)/σ_R ordered by inverse break-up threshold (vs LMT: ordered by F^(k))
2. **Mass scaling:** w_HL approximately mass-independent at fixed E/V_CB (LMT has no analogous prediction)
3. **Threshold structure:** σ_BU^(k)/σ_R rises sharply at E_c.m. ≈ V_CB + E_thresh^(k)/F^(k), then plateaus below F^(k)

## Companion Paper

This framework provides the theoretical basis for the phenomenological analysis in:

N. Lobo et al., "PACE4-Based Channel-by-Channel Exclusion Analysis of
Fusion Mechanisms in the 20Ne + 59Co System," Nuclear Physics A (2026).

Repository: https://github.com/cmn13013-dev/20Ne-59Co-ICF-Analysis

## Contact

ntumbalobo1988@gmail.com | cmn13013@nitech.jp

## License

Creative Commons Attribution 4.0 (CC-BY-4.0)
