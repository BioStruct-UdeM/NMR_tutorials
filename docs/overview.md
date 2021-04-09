---
title: Overview of the instrumentation
author: Normand Cyr
date: 2021-04-07
...

# Overview of the instrumentation

The NMR laboratory of the Structural Biology Platform is equipped with 3
NMR spectrometers:

![Our 3 spectrometers](../img/nmr_spectrometers.png)

-   A **500 MHz spectrometer**, equipped with either a triple resonance
    (TXI) or quadrupole resonance (QXI) room temperature probe.
-   A **600 MHz spectrometer**, equipped with either cryogenic (TCI) or
    room temperature (TXI) triple resonance probe.
-   A **700 MHz spectrometer**, equipped with either a triple resonance
    (TXI) or double resonance broadboard (BBI) room temperature probe.

All three spectrometers enable multi-dimensional, double or triple
resonance experiments with field strengtht typically used in structural
and dynamics studies of proteins and nucleic acids. Additionally,
improved sensitivity is obtained with the cryoprobe on our 600 MHz
spectrometer. Each of our probes accept both 3 and 5 mm NMR tubes
(regular, Shigemi or Bruker Shaped tubes).

Each NMR spectrometer is composed of various parts that will be
discussed below:

![The different parts of the NMR
laboratory](../img/nmrlab-1_annotated.png)

Source: [LEGO
ideas](https://ideas.lego.com/content/project/link/cc82198a-e937-427f-982a-d8854b126577)

## Control computers

Several softwares are in place in order to control the various pieces of
the NMR spectrometer and analyze the data. The following programs are
installed on the control computers:

  Name      Purpose                                 Command to launch
  --------- --------------------------------------- -----------------------------
  TopSpin   Main control and processing software    `topspin`
  BSMS      Bruker Smart Magnet Control System      `bsmsdisp` (within TopSpin)
  MICS      Magnet Information and Control System   `mics` (within TopSpin)
  NMRPipe   Advanced processing scripts             `nmrPipe`

## NMR magnet

The magnet assembly (*aka* the can) is often the most impressive piece
of equipment in a NMR laboratory due in part to the size of its
cryostat. Depending on the field strength, they can easily reach two
stories high (above 5 meters in height).

### Safety around NMR magnets

Several safety rules are in place and need to be understood **before**
entering the NMR laboratory.

#### Magnetic fields

NMR magnets present numerous health hazards caused by the presence of
strong magnetic fields. The strength of the magnetic field increases
with the proximity to the core of the magnet. Each magnet in the NMR
laboratory has its own particularities with respect to stray field. **Do
not cross the yellow plastic chain** (located at the 5 Gauss (0.5 mT)
line) before making sure you do not have anything metallic on you and in
your pockets.

![Safety sign](../img/danger-magnetic.jpg)

Rules to follow around the NMR magnets:

-   Anyone having a medical implant (*eg* Pacemaker) **should not enter
    the NMR room**.
-   Personal metallic items, including watches, wallets, cell phones
    should be left by the controlling computers.
-   Ferrous items, tools in particular, should be kept outside the 5
    Gauss line.
-   Gas cylinders should be manipulated as far as possible from the 5
    Gauss line.
-   Small metallic parts (*eg* staples, paperclips etc.) should be
    carefully disposed in the trash (do not play basketball with them!).

In the event of a fire, we have special non-magnetic fire extinguishers
(white and blue colored) that can be used near the magnets.

#### Cryogenic liquids and risks of quench

The magnet assembly includes cryostats containing liquid helium (4.2 K,
or -268.9°C) and liquid nitrogen (77 K, or -196°C) in order to keep the
magnet coil in a superconducting state. If liquid helium is missing, or
a hot spot is built on the coil, a quench may occur. The definition of a
quench is defined in the Bruker manual as:

> A quench is the very fast de-energizing of the magnet by loss of its
> superconductivity. The stored magnetic energy is converted into heat
> and thus large quantities of helium evaporate. The evaporating helium
> will displace the breathing air.

In the event of a quench, you need to **leave the room immediately**. Do
not try to stop the liquid helium from exiting the NMR magnet; it is too
late. If the oxygen level in the room falls below 19 %, an emergency
evacuation system will be activated and a loud alarm sound will be
heard. Again, **evacuate promptly** and contact the security desk
(extension 7771).

If you are curious, several videos of *controlled* quenches of NMR and
MRI magnets can be found on
[YouTube](https://www.youtube.com/results?search_query=nmr+quench).

### The guts of the magnet

The NMR magnet is composed at is core of an active electromagnet created
by winding several kilometers of superconducting wire kept below its
critical temperature (resistance close to zero at near absolute zero) by
immersion in liquid helium at 4.2 K. This is then kept cool using a
jacket filled with liquid nitrogen at 77 K.

![Schematics of the inside of a NMR
magnet](../img/nmr_spectrometer_inside.svg?sytle=size75)

Source: [Course
Hero](https://www.coursehero.com/sg/organic-chemistry/nuclear-magnetic-resonance-nmr-spectroscopy/)

Both cryogenic liquids slowly boil off over time and need to be
replenished at regular intervals: each week for liquid nitrogen, every 2
months for the liquid helium. More recent magnets, including our 700 MHz
Bruker Ascend, are better insulated and require nitrogen only every 2-3
weeks, and liquid helium every 4 months.

Below is an example of the cross-section of a real magnet. It includes
(**2**) the foil radiation isolation, (**5**) the liquid nitrogen
cryostat, (**10**) the superconducting wire, (**13**) the room
temperature bore tube and (**20**) the liquid helium cryostat. A list of
all the different identified parts can be found
[here](http://www.chem.wilkes.edu/~trujillo/NMR_Course/usask_ca_MAGNET_PICTURES/).

![Cross-section of a NMR
magnet](../img/cross-section_magnet.jpg?style=size50)

Source: [H.A. Trujillo, Wilkes
U.](http://www.chem.wilkes.edu/~trujillo/NMR_Course/usask_ca_MAGNET_PICTURES/)


## Sample tube and spinner

The sample has to be placed in a thin borosilicate glass wall tube of 5
mm in diameter rated at least to the proton frequency of the
spectrometer used. Our probes can also accept Bruker-type Shigemi, 3 mm
and shaped tubes. Then, the sample tube has to be inserted first into a
spinner which is basically a sample holder. Make sure you use a
**Bruker** spinner, not a Varian one. The difference is illustrated
below.

![Bruker vs. Varian spinner](../img/bruker-varian-spinner.jpg)

POM ([polyoxymethylene](https://en.wikipedia.org/wiki/Polyoxymethylene))
blue plastic spinners are the standard spinners used for most bio-NMR
experiments. However, if you need to run your experiment at temperatures
between 0 and 5 °C, or above 80 °C, you will need to use a Kel-F
([polychlorotrifluoroethylene](https://en.wikipedia.org/wiki/Polychlorotrifluoroethylene))
white spinner which is heavier and more resistant to high temperatures
(do not exceed 150 °C!). *Air flow from the BCU II will also need to be
adjusted also.*

It is also imperative that you use the sample depth gauge to ensure that
your sample tube is set at the proper depth, as illustrated below. If
you insert your tube too deep, it will hit the bottom of the probe
insert and will likely **break** resulting in a potential expensive
cleaning and repair procedure. Alternatively, a sample that is not
inserted enough will not be fully exposed to the coils of the probehead.

![Sample depth gauge](../img/sample_depth_gauge.gif)

Source: [Bruker - BSMS
manual](http://triton.iqfr.csic.es/guide/man/bsms/chap5.2.htm)

**d** should be at least 15 mm, ideally 20 mm. This corresponds to about
500 µl in a 5 mm tube.

## NMR probe

It is through the NMR probe that the radio frequencies ("pulses") are
transmitted from the console to the sample, and the NMR signal detected
transferred back to the console (via the [Helmholtz
coils](https://u-of-o-nmr-facility.blogspot.com/2008/03/probe-coil-geometry.html)
- more details [here](https://en.wikipedia.org/wiki/Helmholtz_coil)). It
is composed of a long tube inserted from underneath, through the bore of
the magnet. Connections for cables used for sample temperature and radio
frequencies transmission are made at the base of the probe, while tip
inserts up to the core of the magnet.

Below is the general schematic of a NMR probe, including the position of
the gradient coils, outside of the RF coils.

![Probe diagram](../img/probe_diagram.png)

Source: [UCSD Skaggs School of Pharmacy and Pharmaceutical Sciences NMR
Facility](https://sopnmr.blogspot.com/2018/11/probes.html)

And a picture of the actual coils, if we were to remove the protective
plastic:

![Inside the probe](../img/probe_inside_coils.jpg)

Source: [H.A. Trujillo, Wilkes
U.](http://www.chem.wilkes.edu/~trujillo/NMR_Course/usask_ca_PROBE_PICTURES/)

The NMR probes present at the Structural Biology Platform are all
gradient capable inverse probes where the inner coil is tuned to observe
1H and the outer coil is optimized for decoupling of both 13C and 15N
(named TXI and TCI probes). These are therefore optimized for studying
bio-molecules. The exception is the broadboard inverse (BBI) probe where
the outer coil can be tuned to frequencies between 31P and 15N.

In the case of the cryoprobe (TCI), it additionally uses cryogenically
cooled helium gas (via a compressor) to cool down the detection coils
and the integrated pre-amplifier to \~15 K, in order to minimise thermal
noise and to lower electrical resistance of the RF coils therefore
allowing higher quality factors (Q factors), hence gaining in
sensitivity by a factor of 3-4 folds relative to equivalent room
temperature probes. This is particularly useful to study larger samples,
or samples restricted to low concentration.

## Console and pre-amplifier

The muscles of a NMR spectrometer come from the console. At the
Structural Biology Platform, our spectrometers are equipped with modern
[Bruker AVANCE
NEO](https://www.bruker.com/products/mr/nmr/avance-neo.html) consoles.
These large boxes on wheels house the various power amplifiers and
transceivers that generate, time, transmit/receive and record the NMR
impulsions and signals involved in the NMR experiment. Everything is
connected to the control computer for easy visualization.
