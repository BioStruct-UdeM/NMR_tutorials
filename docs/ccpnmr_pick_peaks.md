---
title: Peak picking
author: Normand Cyr
date: 2021-04-09
...

# Peak picking

There are two main ways to pick peaks in CcpNmr: (1) automatic and (2)
manual peak picking.

## Automatic method

The easiest approach is to let the software decide which signals are
peaks and position their maxima automatically. In order to do so, in
`window1`, hold down the `Shift` and `Ctrl` keys while dragging around
an area with the left button of the mouse pressed. Once you release the
left button, CcpNmr will find the contour extrema and define them as
peaks.

![Automatic peak picking](../img/ccpnmr/automatic_peak_picking.png)

As you can see from the image above, several peaks were placed on
signals that are likely corresponding to noise. Hence while using the
automatic method, you need to make sure your contour levels are
appropriate in order to prevent picking peaks from the noise!

A visual inspection is highly recommended following the procedure. In
order to delete unwanted peaks, you can select one peak (or multiple
peaks by holding the `Shift` button while selecting the peaks) by
left-clicking on the peak of interest, and then pressing the `Delete`
key, then accepting the deletion.

![Delete peaks](../img/ccpnmr/delete_peaks.png)

## Manual method

Sometimes, you want to pick peaks manually, or want to add a second peak
mark over a signal representing overlapping peaks. To do so, hold down
the `Ctrl` key and left-click on the location where you want to pick a
peak. A cross will appear.

You can then move it while it is being selected by moving the mouse to
the appropriate location and press the `p` key. You may even be able to
center it in the peak signal by pressing `Shift + p`.

## Inspecting the peak list

A table containing a list of peaks for each spectrum can be found here:
`Peaks > Peak Lists` and select the `Peak Table` tab. In that table, you
will find information about each peak (position, assignment, height and
volume, *etc*.).

![Peak table](../img/ccpnmr/peak_table.png)

You can also export the information in a text file by right-clicking in
the table and selecting `Export`.

![Export peak data](../img/ccpnmr/export_peak_data.png)

## Next step

In the step, we will go over [setting up a project](../project_setup/)
and assigning root resonances.
