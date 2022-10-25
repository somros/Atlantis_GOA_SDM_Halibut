# Spatial distributions of Pacific halibut from setline data and `sdmTMB`

This repo contains code that maps halibut catches from IPHC's [FISS data](https://www.iphc.int/management/science-and-research/fishery-independent-setline-survey-fiss) to the Atlantis GOA geometry with [`sdmTMB`](https://github.com/pbs-assess/sdmTMB) (Andreson et al. 2022).

The output of this code is not actually used for the S1-S4 parameters for halibut. We use [RACE-GAP and DFO workflow](https://github.com/somros/Atlantis_GOA_SDM_coupling_and_initbiom) because:

1. Consistency with the rest of the groundfish.
2. FISS data not ideal for juveniles.
3. Difficult spatial extrapolation as CPUE is per line and not area.
4. Models fitting RACE-GAP data for both stages of halibut converged in both AK and BC.

The maps produced have validation purpose. 

__References__

Anderson, S.C., E.J. Ward, P.A. English, L.A.K. Barnett. 2022. sdmTMB: an R package for fast, flexible, and user-friendly generalized linear mixed effects models with spatial and spatiotemporal random fields. bioRxiv 2022.03.24.485545; doi: https://doi.org/10.1101/2022.03.24.485545
