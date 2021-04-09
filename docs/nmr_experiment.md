---
title: Running a NMR experiment
author: Normand Cyr
date: 2019-08-12
...

# NMR experiment

To maximize the quality of the NMR data acquired with our spectrometers, it is key to correctly handle the sample throughout the process; from production to NMR data acquisition. The objective of this section is to propose general guidelines for sample preparation and initial data acquision.


## Sample requirement

Biological NMR is intrinsically poorly sensitive and the intensity of the signal is proportional to the amount of material present in the observed volume. If you use a regular 5 mm NMR tube, a filling length of 40 mm is recommended, which corresponds to about 550 µl of sample in a 5 mm tube with walls 0.4 mm thick. If the volume is limited, 5 mm Shigemi, or 3 mm tubes can be used and will require less volume, typically in the 300-350 µl range.

One thing to remember: the signal-to-noise ratio (SNR) increases as the square root of the number of scans recorded. So to get a similar SNR with a sample concentrated at 0.5 mM *vs* at 1.0 mM, 4 times more acquisition scans will be required (*ie* the experiment will take 4 times longer).

\[ \text{SNR} \propto \sqrt{\text{nb scans}} \]

Practically, at least 100 µM of sample is enough for simple checks (1D and 2D correlation experiments), whereas 0.5-1.0 mM should be attained in order to have good SNR on multi-dimensional experiments within acceptable experiment time.

Additionally, the sample has to remain stable during the course of the NMR experiment. Various chemical changes may take place (oxidation, proteolytic degradation, microbial contamination), especially since most NMR recordings are done at, or near, room temperature. In order to assess the stability, it is recommended to record a quick "simple check experiment" (1D or 2D correlation experiment if isotopically labeled - *eg* <sup>15</sup>N-HSQC) before **and** after long term data acquisition. If there is no difference, the sample has not changed.

\[ \text{identical spectra} = \text{identical sample} \]



In terms of buffer, a slightly acid environment is preferred in order to favour protonation of side chains

Salt concentration up to 500 µM is generally ok.


Once you know your sample meets the NMR requirements, you can reserve some time on the instrument by contacting me by email ([normand.cyr@umontreal.ca](mailto:normand.cyr@umontreal.ca)).


## Sample preparation

The sample has to be optically clear and free of particles in suspension. A 5 minute centrifugation, or a filtration through a 0.22 µm filter will remove any suspended matter.

On the day of the NMR experiment:

* Determine exact sample concentration after dialysis
* Keep ~10 ml of dialysis buffer
* Centrifuge particles down from your sample and filter the dialysis buffer


## Setup



## Data acquisition


## Processing


# References

[Kelly AE, *et al* (2002)](https://doi.org/10.1021/ja026121b). Low-conductivity buffers for high-sensitivity NMR measurements. *J Am Chem Soc*.
