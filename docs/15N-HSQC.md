---
title: Running a 15N-HSQC
author: Normand Cyr
date: 2019-09-06
...

# Running a <sup>15</sup>N-HSQC

## Pulse programs available

In the Bruker pulse program catalogue, there are several pulse programs available. These include:

the standard echo / anti-echo versions with sensitivity improvement:

- **`hsqcetfpf3gpsi`**
- `hsqcetfpf3gpsi2`

along with their TROSY versions:

- `trosyetf3gpsi`
- `trosyetf3gpsi2`
- **`trosyetfpf3gpsi`**

SO-FAST HMQC:

- **`sfhmqcf3gpph`**
- `sfhmqcf3gpphiasi`

BEST version with TROSY options:

- `b_hsqcetf3gpsi`
- `b_trosyetf3gpsi`
- `b_trosyetf3gpsi.2`
- `b_trosyetf3gpsi.3`

Pulse sequences already tested and standard parameters implements on our systems are in **bold**.


## Standard parameters

### Standard 15N-HSQC

For the standard 15N-HSQC (`hsqcetfpf3gpsi`): `PROT_N-HSQC`

For the TROSY version of the 15N-HSQC (`trosyetfpf3gpsi`): `TROSYETF3GPSI` (from the Bruker library)

For the SO-FAST 15N-HMQC (`sfhmqcf3gpph`): `PROT_SFHMQC`

### BEST versions

 if you want to investigate downfield shifted signals  (such  as  tryptophan  side  chain  resonances)  or  signals  which  are  very  close  to  the  water  frequency,  the  bandwidth  and/or offset frequency may need to be fine tuned. The offset is simply changed by altering the parameter cnst19 (or cnst54), but  changing  the  bandwidth  requires  all  shape  lengths  and  amplitudes  to  be  recalculated.  The  python  script  “bestbw”  provides  an  easy-to-use  solution  for  changing  both  these  parameters

The Python program `bestbw` lengths and amplitudes can be used to change the excitation bandwidth and recalculate the shape lengths and amplitudes of the pulses.

For the BEST version of the 15N-HSQC (`b_hsqcetf3gpsi`): `B_HSQCETF3GPSI` (from the Bruker library)

For the BEST version with TROSY of the 15N-HSQC (`b_trosyetf3gpsi`): `B_TROSYETF3GPSI` (from the Bruker library)
