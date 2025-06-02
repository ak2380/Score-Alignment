# Score-Alignment

> **Proof-of-work archive** for my 2024-25 research project titled Musical Score to Performance Alignment using Statistical Inference. 
> The notebooks, audio assets and incremental experiment logs collected here mirror the weekly progress described in my logbook and final report.

---

## Repository map

| Path | Contents | Purpose |
|------|----------|---------|
| **`HMM VERSIONS/`** | 13 Jupyter notebooks `HMM_1.ipynb` … `HMM_13.ipynb`. Descriptive filenames highlight each design change (Sigmoid-likelihood, RMS gating, Scaled-covariance …). | Step-by-step evolution of the Hidden-Markov-Model pipeline. Each notebook is a runnable experiment. |
| **`AUDIO SEPARATION FILES/`** | 6 notebooks (`Piano Audio Separation.ipynb` + versions v2–v5, `Project Notebook 1.ipynb`). | Parallel work-package on Gaussian-Process piano source separation baseline HPSS, median-filter prototypes, GP kernels |
| **`MIDI Files/`** | 7 symbolic scores. | Ground-truth material for alignment tests. |
| **`MP3 Files/`** | 7 audio performances (44.1 kHz) matching the MIDI files. | Shared test set for alignment and separation experiments. |

---

## Proof-of-work checkpoints

1. **Incremental notebooks**  
   * Each notebook shows code, narrative, plots produced during that week’s work. 

2. **Reproducible artifacts**  
   * Every notebook runs end-to-end using only the assets in `MIDI Files/` and `MP3 Files/` plus standard Python libs (`numpy`, `scipy`, `librosa`, `pretty_midi`, …).  

3. **Versioned methodology**  
   * File names capture the core methodological tweak, so each result in the thesis can be traced to the exact code revision.

---

## Quick-start

```bash
git clone https://github.com/<user>/Score-Alignment.git
cd Score-Alignment
```

Once you have cloned the repository and accessed the files, you can run the experiments within each Jupyter notebook using the supplied audio files and MIDI scores.
