# MaDeLaNe 2026 — S1-M1 Connectivity Analysis

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/maierav/madelane26/blob/main/MaDeLaNe26_S1M1_Rasters.ipynb)

Colab notebook for exploring intracortical microstimulation (ICMS) data from
[Shelchkova et al. (2023) *Nature Communications*](https://doi.org/10.1038/s41467-023-43140-2).

## What's in here

**`MaDeLaNe26_S1M1_Rasters.ipynb`** — a Colab-ready notebook that:

- Loads raw spike + stimulation data (one `.mat` file per S1 electrode x M1 channel pair)
- Plots **train-aligned rasters** (20 trials of 1-s ICMS) with Gaussian-smoothed SDFs
- Plots **pulse-locked rasters** (ms timescale) for detecting short-latency monosynaptic responses
- Shows three response types: tonic excitation (MC56), biphasic (MC27), and inhibitory (MC129)
- Compares responses on the same M1 neuron to different S1 electrodes (somatotopic specificity)
- Multi-channel overview panel across 10 M1 channels

## Data

Raw data from [DABI](https://dabi.loni.usc.edu/), Shelchkova et al. "Connectivity Paper", S1M1 Data, RawData.

Participant C1 has ~13,800 `.mat` files (62 stim electrodes x ~200 motor channels).
Each file is HDF5 (MATLAB v7.3) containing spike times and stimulation timestamps.

## Usage

1. Download the `RawData/C1` folder from DABI
2. Open the notebook in Colab
3. Update `DATA_DIR` to point at your copy
4. Run all cells

## Reference

Shelchkova, N.D., Downey, J.E., Greenspon, C.M. et al. *Microstimulation of human
somatosensory cortex evokes task-dependent, spatially patterned responses in motor cortex.*
Nat Commun **14**, 7368 (2023).
