# friendly-enigma
final project AY250: preprocess neural data (for Wallis lab)


## Overview

0. `convert_raw_data.m`: load raw data (.bhv2, .pl2) and save as .mat
1. next step
2. next step

### 0. convert raw data

During a typical session, we record 3 types of data concurrently:
1. Behavior: the task events and subject responses are controlled by the MATLAB Toolbox [MonkeyLogic](https://monkeylogic.nimh.nih.gov/); task events saved in .bhv2
2. Local field potentials (LFP): voltage signals < 250Hz are sampled at 100Hz and recorded with [Plexon's OmniPlex system](https://plexon.com/plexon-systems/omniplex-neural-recording-system/); continuous data saved in .pl2
3. Spiking data (SPK): voltage signals > 250Hz are sampled at 40kHz and recorded with [Plexon's OmniPlex system](https://plexon.com/plexon-systems/omniplex-neural-recording-system/); waveforms (4 st. dev threshold crossings) are manually sorted into unique sources (neurons) with [Plexon's OfflineSorter](https://plexon.com/products/offline-sorter/); threshold crossing timestamps saved in .pl2

To sync these data streams, we send duplicate task event codes from the PC controlling behavior to the PC recording neural data.

These unique filetypes were designed to for MATLAB and Windows machines, and are not easily accessible with Python. To avoid spending my entire project on just opening the raw data in Python, I first convert everything to .mat files in MATLAB.

### 1. next step


### 2. next step
