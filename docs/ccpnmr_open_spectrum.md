---
title: Spectrum visualization
author: Normand Cyr
date: 2021-04-09
...

# Spectrum visualization

## Opening a spectrum

You can open a single spectrum via `Project > Open Spectra`. A new
dialog window will open. Choose the proper file format of your spectra
(Bruker, NMRView, NMRPipe *etc*.) and then navigate to the location of
the data file.

![Open spectra](../img/ccpnmr/open_spectra.png)

Select the spectrum (you can also select multiple spectra) you want to
open. It will appear in the list of spectra to open at the bottom of the
dialog window. It is now a good time to rename the spectrum by
double-clicking on `Expt_1` and changing the name to something more
meaningful (*e.g.* `HN-ubiquitin`).

![Open spectra - change name](../img/ccpnmr/open_spectra_name.png)

Click on `Open Spectrum`. A verification window will then open. Make
sure this is the spectrum you want to open, click `Commit` and in the
next window, select the appropriate `Type Synonym` (`15N HSQC/HMQC` in
this example).

![Verify spectra](../img/ccpnmr/verify_spectra.png)

Once you have done that (if opening multiple spectra, it needs to be
done for each of them), click on `Close - All Done` and your spectrum
will open in a new window.

![Nhsqc window](../img/ccpnmr/Nhsqc.png)

### Bruker data

In the case of Bruker spectra, you only need to reach the root folder of
your experiment and CcpNmr will recognize the
`<expno>/pdata/<procno>/procs` folder automatically.

![Open Bruker spectra](../img/ccpnmr/open_spectra_Bruker.png)

## Navigation

You can now navigate through your spectrum using the [mouse
buttons](ccpnmr.md/#mouse-navigation) and [keyboard
shortcuts](ccpnmr.md/#keyboard-shortcuts). Here is a reminder of the
mouse functions used in CcpNmr.

<style type="text/css">
  .tg-c3ow{border-color:inherit;text-align:center;vertical-align:top}
  .tg-fymr{border-color:inherit;font-weight:bold;text-align:left;vertical-align:top}
  .tg-7btt{border-color:inherit;font-weight:bold;text-align:center;vertical-align:top}
  .tg-0pky{border-color:inherit;text-align:left;vertical-align:top}
  .center {margin-left:auto;margin-right:auto;width:50%;border-bottom: 1px solid #dee2e6;margin-bottom: 21px;margin-top: 21px}
</style>
<table class="center table table-striped table-hover">
<thead>
  <tr>
    <th class="tg-fymr">Mouse button</th>
    <th class="tg-7btt">Action</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0pky">Left</td>
    <td class="tg-c3ow">Select peak</td>
  </tr>
  <tr>
    <td class="tg-0pky">Left + Shift</td>
    <td class="tg-c3ow">Select peaks in region</td>
  </tr>
  <tr>
    <td class="tg-0pky">Left + Ctrl</td>
    <td class="tg-c3ow">Pick peak</td>
  </tr>
  <tr>
    <td class="tg-0pky">Left + Shift + Ctrl</td>
    <td class="tg-c3ow">Pick peaks in region</td>
  </tr>
  <tr>
    <td class="tg-0pky">Right</td>
    <td class="tg-c3ow">Options menu</td>
  </tr>
  <tr>
    <td class="tg-0pky">Wheel</td>
    <td class="tg-c3ow">Drag spectrum</td>
  </tr>
  <tr>
    <td class="tg-0pky">Wheel + Roll</td>
    <td class="tg-c3ow">Zoom</td>
  </tr>
  <tr>
    <td class="tg-0pky">Wheel + Shift + Roll</td>
    <td class="tg-c3ow">Navigate through planes of 3D spectrum</td>
  </tr>
</tbody>
</table>

## Spectrum window menu buttons

At the top of the spectra window lies 4 buttons (`Spectra`, `Contours`,
`Peaks` and `Strips`) that give access to various viewing options.

The `Spectra` button opens the list of spectra currently loaded in the
window (named `window1` by default - this can be changed via
`Ẁindow > Windows`, double-clicking on the window name and changing it).
In order to hide a spectrum, you can click on its name.

![Spectra button](../img/ccpnmr/spectra_bar_button.png)

The `Contours` button enable you to adjust the contour levels. The
arrows rise, or lower the contour (base level), in a similar way as the
`e` and `r` keys. The `+1` and `-1` buttons let you change the number of
levels and the `Pos/Neg` button let you show/hide positive and negative
signals. Note that the changes will apply only to the active (displayed)
spectra in the current window.

![Contour button](../img/ccpnmr/contour_bar_button.png)

Finally, the `More..` button will open another dialog window which
enable you to fine-tune the contour parameters.

![Spectrum contour levels
button](../img/ccpnmr/spectrum_contour_levels.png)

The `Peaks` button let you show/hide peaks from the various spectra
displayed in the active window.

![Peaks button](../img/ccpnmr/peaks_bar_button.png)

Finally, the `Strips` button let you add, remove activate and navigate
through strips. This option is very useful when analyzing 3D datasets.

![Strips button](../img/ccpnmr/strips_bar_button.png)

Example of strips

![Strips example](../img/ccpnmr/strips_demo.png)

## Customizing the colours and the spectra order

The default teal colour proposed by CcpNmr for the first spectrum that
you open may not be the most attractive colour. In order to change it,
got to `Experiment > Spectra`, then `Display Options` tab.

![Change the colour of the
spectra](../img/ccpnmr/change_spectrum_colour.png)

When you have multiple spectra, it is possible to define the order
(rank) which they will follow in the stack. To do so, change the `Rank`
number for each spectrum to match to order you want to see them (lower
number will bring the spectrum higher in the stack).

## Next step

Once your spectrum is loaded, you can start [picking
peaks](../ccpnmr_pick_peaks/).
