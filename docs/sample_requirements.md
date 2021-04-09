---
title: Sample requirements
author: Normand Cyr
date: 2021-04-07
...

To maximize the quality of the NMR data acquired with our spectrometers,
it is key to correctly handle the sample throughout the process; from
production to NMR data acquisition. The objective of this section is to
propose general guidelines for sample preparation and initial data
acquisition.

# Sample requirement

## Quantity


Biological NMR is intrinsically poorly sensitive and the intensity of
the signal is proportional to the amount of material present in the
observed volume. Thus, you should maximize the quantity of sample
submitted for analysis, while minimizing the volume, in order to get the
highest concentration as possible.

### Volume and concentration

If you use a regular 5 mm NMR tube, a filling length of 40 mm is
recommended, which corresponds to about **550 µl** of sample in a 5 mm
tube with walls 0.4 mm thick. If the volume is limited, 5 mm Shigemi
(*ie* containing susceptibility-matched plugs), or 3 mm tubes (with
slightly reduced sensitivity), can be used and will require less volume.
Below is an illustration of the construction of a Shigemi tube:

![Shigemi tube](../img/shigemi.png)

Source: [JEOL](https://www.jeol.co.jp/en/applications/detail/1867.html)

Summary of optimal volume and quatity for different NMR tubes:

<style type="text/css">
  .tg-lboi{border-bottom:inherit;border-color:inherit;text-align:left;vertical-align:middle}
  .tg-9wq8{border-bottom:inherit;border-color:inherit;text-align:center;vertical-align:middle}
  .tg-c3ow{border-bottom:inherit;border-color:inherit;text-align:center;vertical-align:top}
  .tg-0pky{border-bottom:inherit;border-color:inherit;text-align:left;vertical-align:top}
  .center {margin-left:auto;margin-right:auto;width:75%;border-bottom: 1px solid #dee2e6;margin-bottom: 21px;margin-top: 21px}
</style>

<table class="center table table-striped table-hover">
  <tbody><tr>
    <th class="tg-lboi" rowspan="2">Type of tube<br></th>
    <th class="tg-9wq8" rowspan="2">Volume, µl<br></th>
    <th class="tg-c3ow" colspan="2">Quantity, nmol</th>
  </tr>
  <tr>
    <td class="tg-c3ow">at 100 µM</td>
    <td class="tg-c3ow">at 500 µM</td>
  </tr>
  <tr>
    <td class="tg-0pky">5 mm</td>
    <td class="tg-c3ow">550</td>
    <td class="tg-c3ow">55</td>
    <td class="tg-c3ow">275</td>
  </tr>
  <tr>
    <td class="tg-0pky">5 mm Shigemi</td>
    <td class="tg-c3ow">350</td>
    <td class="tg-c3ow">40</td>
    <td class="tg-c3ow">200</td>
  </tr>
  <tr>
    <td class="tg-0pky">3 mm</td>
    <td class="tg-c3ow">160</td>
    <td class="tg-c3ow">20</td>
    <td class="tg-c3ow">100</td>
  </tr>
</tbody></table>

Practically, on the instruments of the Structural Biology Platform, at
least 100 µM of sample is sufficient for simple checks (1D and 2D
correlation experiments), whereas concentrations beyond **0.5 mM**
should be attained in order to have good SNR on multi-dimensional
experiments within acceptable experiment time. When the quantity and
volume are limited, some options are available to obtain a good
signal-to-noise ratio (SNR):

![Dealing with small amounts](../img/small_amounts.jpg)

Source: [UOttawa NMR facility
blog](https://u-of-o-nmr-facility.blogspot.com/2007/10/i-only-have-05-mg-of-sample-what-can-i.html)

One thing to remember: we can increase the SNR by increasing the number
of scans (`ns`), however the SNR increases as the square root of the
number of scans recorded. So to get a similar SNR with a sample
concentrated at 0.5 mM *vs* at 1.0 mM, 4 times more acquisition scans
will be required (*ie* the experiment will take 4 times longer!).

\[ \text{SNR} \propto \sqrt{\text{nb scans}} \]


## Stability

The sample submitted for NMR analysis has to be chemically stable over
the course of the experiment and presence of contaminants (microbial,
chemical, biochemical) could degrade it to a level beyond usability,
rapidly, especially since most NMR recordings are done at, or near, room
temperature. It is therefore imperative to evaluate the stability of the
sample *prior* to the NMR experiments. This can easily be done by
keeping an unlabeled sample at room temperature for 2 weeks and
verifying its integrity before and after (SDS-PAGE, 1D NMR).

Additionally, the integrity of the sample should be assessed before
**and** after long (more than 6 hours) experiments by running either a
1D proton spectrum, or, better for labeled samples, a 2D ^15^N-HSQC
spectrum. If there is no difference in the spectra, no change in the
chemical environment of the atoms has occurred, hence the sample
remained identical (no degradation *etc*). Simply put:

\[ \text{identical spectra} = \text{identical sample} \]


## Sample buffer

### Buffer pH

In terms of buffer, a slightly acidic environment (**pH around 5.5 -
6.5**) is typical for biological samples (proteins, DNA, RNA) in order
to favor protonation of the exchangeable protons (amide (proteins) and
imino (nucleic acids)). Above a pH of 7.5, it may be difficult to detect
amide protons, more sample will be required, and can result in sample
degradation.

### Buffer ionic strength

Salt (typically in the form of NaCl or KCl) is generally used in sample
buffers in order to prevent non specific ionic interactions and favor
proper folding of the sample. For NMR analysis, ionic strength with a
salt concentrations up to 500 mM is *generally* appropriate (**below 150
mM** being ideal). Higher salt concentrations complicate the tuning and
matching of the probe and result in longer 90° pulse duration which may
need power adjustments exceeding maximal permitted levels for a given
probe. This is particularly true for the cryoprobe.

#### The case of the cryoprobe

When a cryogenic probe is used (as in the case of the [TCI probe on our
600 MHz](../overview_instrumentation/#nmr-probe)), salt concentrations
below 100 mM are preferred in order to reduce signal degradation caused
by the increased *conductivity*, which is a function of both the ion
**concentration** and ion **mobility** .

This latter property may be modulated by using different compounds to
prepare the sample buffer, and may even enable the use of high salt
concentrations. [Kelly *et al*](https://doi.org/10.1021/ja026121b)
describe and illustrate thoroughly the effect of various ionic species
on cryoprobe sensitivity, where they show that "the detrimental effect
of high salt concentrations can be counterbalanced by low ion
mobilities".

> for high salt concentrations, the gain in sensitivity of a particular
> buffer over another buffer becomes independent of the actual ion
> concentration and reaches a maximum that is equal to the square root
> of the ratio of the individual ion mobilities.

In the figure below, we can see that signal-to-noise ratio (value in
parentheses) varies by 2-fold depending on the type of chemicals used to
prepare the NMR buffer.

![SNR for different buffer
compositions](../img/s-n_different_buffers.png)

Sensitivities relative to tripolyphosphate of a 2 mM *p*-aminobenzoic
acid sample dissolved in 200 mM buffer. Source: [Kelly *et al*
(2002)](https://doi.org/10.1021/ja026121b)

Illustrated below is a similar effect on a biological sample (lysozyme
in this case).

![SNR of a lysozyme 1D proton spectrum in different buffer mixtures
](../img/s-n_lysozyme_different_buffers.png)

Source: [Kelly *et al* (2002)](https://doi.org/10.1021/ja026121b)

Therefore, **time used to determine a good, low conductivity buffer
suitable for the biological sample analyzed is always time well
invested**

## Sample preparation

The sample has to be optically clear and free of particles in
suspension. A 5 minute centrifugation, or a filtration through a 0.22 µm
filter will remove any suspended matter.

On the day of the NMR experiment:

-   Add D<sub>2</sub>O to a final concentration of 10 %
-   Measure the pH of the sample and adjust if needed
-   Centrifuge particles down from your sample and filter if needed
-   Determine the exact sample concentration
-   Transfer the sample to a clean NMR tube
-   Label your NMR tube appropriately

## Summary

-   Aim for 500 µM of sample concentration in 500-550 µl (\~250 nmol of
    sample) if using a 5 mm NMR tube
-   Avoid high salt concentrations, or look into alternative, low
    conductivity, buffers
-   If you do not have enough material, consider using a 3 mm tube

Once you know your sample meets the above NMR requirements, you can
reserve some time on the instrument by contacting me by email
([normand.cyr@umontreal.ca](mailto:normand.cyr@umontreal.ca)).
