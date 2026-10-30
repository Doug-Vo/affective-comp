# Affective Computing — Speech Emotion Recognition

Small GRU and CRNN models on **CREMA-D**, trained on clean vs extra “messy” copies, tested on **held-out speakers** (clean and *simulated* degraded audio). A White House clip is a **qualitative demo only** (no labels, not an accuracy result).

The degraded test is **not** real-world field audio. It applies phone band-limiting + reverb + noise (and sometimes cut-off) to the same 9 CREMA-D test speakers.

## Notebook

Run `ser_realworld_audio.ipynb` with Python **3.11** 

## CREMA-D

1. Download CREMA-D (AudioWAV).
2. Unzip so wav files sit at:

```text
datasets/AudioWAV/*.wav
```

Example filename: `1001_DFA_ANG_XX.wav`.


## Demo video (optional)

Place the White House webm (https://commons.wikimedia.org/wiki/File:Yes_We_Can-_People_Share_Their_Most_Memorable_Moments_from_the_Obama_Presidency.webm) at:

```text
test_video/Yes_We_Can-_People_Share_Their_Most_Memorable_Moments_from_the_Obama_Presidency.webm
```

Without this file, CREMA-D training and the 8-row table still run. The demo cells will stop.

## Run order

1. Create a 3.11 venv and `pip install -r requirements.txt`.
2. Put CREMA-D in `datasets/AudioWAV/`.
3. Open `ser_realworld_audio.ipynb` and Run All.

