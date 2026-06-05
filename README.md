# CoolAi

Neural network replacement for CoolProp — 400× faster, engineering-grade accuracy for water.

**Live site:** https://mahdiqoo.github.io/CoolAi/

## Features
- 18,248 parameter model trained on 1.49M CoolProp states
- Single-pass inference: Density, Enthalpy, Entropy, Cp, Cv, Speed of Sound, Viscosity, Conductivity
- Perfect two-phase accuracy via analytic saturation tables
- Exports: PyTorch, TorchScript (GPU/CPU), ONNX
- Validated: MAPE 0.017–0.145%, R² > 0.99999

## Speed
- 100k evaluations: 0.0679s (all 8 props) vs CoolProp vectorized ~2.89s (1 prop)
- **413.7×** vs scalar, **40.8×** vs vectorized, **~340×** for 8 properties

## Usage
C++ recommended for minimum overhead. Python works best in batch mode (larger batch = higher speedup).

Contact for model access: see website.

---
© 2026 Mahdi Dehghan
