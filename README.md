# Tingyu-Neurolearning
---

An EEG hyperscanning study created by Ting-Yu et al.

## Experimental Environment

* Software is based on [Unity](https://unity.com/) and [labstreaminglayer](https://github.com/sccn/labstreaminglayer). 
* Using [Tobii eye tracker 5](https://gaming.tobii.com/product/eye-tracker-5/) to track subjects' eye moving.
* Brainproduct [BrainAmp](https://www.brainproducts.com/solutions/brainamp/) as EEG device.

## Experimental paradigms

* A number of mathematics problems to test subjects' problem solving skills.
* Using simulated sound effect to test whether it would enhance subjects' discussion.

## Data processing

1. Seperate the EEG data to two part (two subjects)
2. Band-pass filter (1~50Hz)
3. Resampple (1000 -> 250 Hz)
4. Re-referece (TP9, TP10)
5. ASR (k = 20)
6. ICA
7. ICLabel (keep brain and others)
8. Calculate EEG index - workload, engagement, emotion, etc.
