# Jense et al. (2024) Emulators

This directory contains the emulators for the paper _A complete framework for cosmological emulation and inference with CosmoPower_. The paper is available as pre-print on [arXiv](https://arxiv.org/abs/2405.07903).

## Note about the P(k) emulators

The P(k) emulators were supposed to be trained with non-linear feedback enabled (using the `mead2020_feedback` model in CAMB and varying `logT_AGN`). By mistake, we ended up setting the model to `mead2020`, which does not include the nonlinear feedback. As a result, the emulators available do not actually contain non-linear feedback. Running camb with the settings presented in the yaml files will have similar behaviour.
