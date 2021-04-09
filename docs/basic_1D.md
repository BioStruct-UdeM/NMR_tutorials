---
title: Basic 1D - Analyzing NMR data
author: Normand Cyr
date: 2021-04-07
...

## Setup

Now that you have your sample ready, that meets the [sample
requirements](../sample_requirements/) and is in an NMR tube, you can
insert it in the [Bruker spinner](../overview_instrumentation/#sample-tube-and-spinner) and
adjust the depth using the sample depth gauge as depicted below:

![Sample depth gauge](../img/sample_depth_gauge.gif)

Source: [Bruker - BSMS
manual](http://triton.iqfr.csic.es/guide/man/bsms/chap5.2.htm)

In the present case, **d** should be at least 15 mm, ideally 20 mm. This
corresponds to about 500 µl in a 5 mm tube. Do not hesitate to confirm
with the NMR manager that your tube is properly positioned.

<p class="warning_box">
  Never insert a sample tube without a spinner in the NMR magnet! The tube will break and cause expensive magnet bore and probe clean up!
</p>

### Sample insertion

There is usually a dust cap on top of the sample bore of the magnet in
order to prevent dust and debris from entering the bore. In order to
insert your sample along with its spinner, you first need to remove it
and put it aside, on the top of the magnet.

Then, in TopSpin, on the control computer, enter the command `ej` to
activate the air lift and if it is the case, *eject* the sample already
present in the magnet. Climb up the stairs and replace the previous
sample in the bore (red touret) with yours. Make sure the air lift is
activate so that your sample does not *fall* in the bore. The pneumatic
system should be powerful enough to maintain your sample on top.

![Sample insertion from the top of the magnet](../img/insert_sample.png)

Come back to the control computer and type `ij` in TopSpin to *inject*
your sample in the bore. Your sample will then slowly lower down into
the core of the magnet and in the [NMR
probe](../overview_instrumentation/#nmr-probe).

### Setting the temperature

The first thing to do following the insertion of your sample in the
magnet, is to set the temperature, as most chemical shifts are
temperature dependent, including the lock signal. Use the command `edte`
to open the temperature window in TopSpin. The current temperature is
written in the center of the window (25.0 °C), and is labeled as
corrected (`Corr.`)

![edte window](../img/edte_window.png)

The temperature set on the computer is slightly different than the
actual temperature in the magnet.

![Temperature dialog](../img/temperature_dialog.png)

### Lock

The lock is a separate NMR spectrometer within the spectrometer which is
specific to deuterium. In order to produce a high resolution NMR
spectrum of a sample, it is key to keep a constant magnetic field
strength over the duration of the experiment. This is achieved by
"locking" the spectrometer to the frequency of deuterium, *ie* by
centering the deuterium signal to a predefined frequency. This signal is
constantly monitored and compensations for the external magnetic field
(B~0~) drift are made in order to keep the resonance frequency constant.

Modern NMR magnets do not drift much beyond 4 to 5 Hz per hour. Yet,
this would be sufficient to lose spectral resolution (*eg* J-coupling)
over a 1 hour experiment. As a reference, below are the current (as of
February 2020) magnet drifts for our NMR spectrometers.

<style type="text/css">
  .tg-lboi{border-bottom:inherit;border-color:inherit;text-align:left;vertical-align:middle}
  .tg-9wq8{border-bottom:inherit;border-color:inherit;text-align:center;vertical-align:middle}
  .tg-c3ow{border-bottom:inherit;border-color:inherit;text-align:center;vertical-align:top}
  .tg-0pky{border-bottom:inherit;border-color:inherit;text-align:left;vertical-align:top}
  .center {margin-left:auto;margin-right:auto;width:50%;border-bottom: 1px solid #dee2e6;margin-bottom: 21px;margin-top: 21px}
</style>
<table class="center table table-striped table-hover">
  <tbody><tr>
    <th class="tg-lboi">Magnet</th>
    <th class="tg-9wq8">Drift, Hz/h</th>
  </tr>
  <tr>
    <td class="tg-0pky">500 MHz</td>
    <td class="tg-c3ow">2.4</td>
  </tr>
  <tr>
    <td class="tg-0pky">600 MHz</td>
    <td class="tg-c3ow">0.2</td>
  </tr>
  <tr>
    <td class="tg-0pky">700 MHz</td>
    <td class="tg-c3ow">0.2</td>
  </tr>
</tbody></table>

### Tune and match

### Shim

## Data acquisition

## Processing

## References
