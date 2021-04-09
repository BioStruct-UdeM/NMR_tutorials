---
title: CcpNmr Analysis
author: Normand Cyr
date: 2021-04-09
...

# CcpNmr Analysis software

## Downloading and installing CcpNmr

As of 2021-02-26, the latest version of CcpNmr Analysis 2 is 2.5.2. You can download the software from the CCPN website [here](https://www.ccpn.ac.uk/v2-software/downloads/2.5). Installation instructions for the various supported operating systems are also outlined on the download page.

*There is now a version 3.0 of CcpNmr Analysis. This version will likely replace version 2 in the future. However, there is currently no working macromolecular structure determination module associated with the software. We therefore recommend that you familiarize yourself with, and use, version 2.5.2*

## Launching CcpNmr

Once CcpNmr is installed, open a terminal window, and reach the `ccpnmr2.5.2` folder. From there, you can launch the program from the
command line interface by typing the command `./bin/analysis`. A small window containing the different menus will appear.

![Menu bar](../img/ccpnmr/menu_bar.png)

## Mouse navigation

Here is a summary of the mouse functions used to navigate through the
NMR spectra and menus.

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

## Keyboard shortcuts

<style type="text/css">
  .tg-cly1{text-align:left;vertical-align:middle}
  .tg-lboi{border-color:inherit;text-align:left;vertical-align:middle}
  .tg-9wq8{border-color:inherit;text-align:center;vertical-align:middle}
  .tg-fymr{border-color:inherit;font-weight:bold;text-align:left;vertical-align:top}
  .tg-7btt{border-color:inherit;font-weight:bold;text-align:center;vertical-align:top}
  .tg-nrix{text-align:center;vertical-align:middle}
  .center {margin-left:auto;margin-right:auto;width:50%;border-bottom: 1px solid #dee2e6;margin-bottom: 21px;margin-top: 21px}
</style>
<table class="center table table-striped table-hover">
<thead>
  <tr>
    <th class="tg-fymr">Key</th>
    <th class="tg-7btt">Function</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-lboi">Cursor (Arrow)</td>
    <td class="tg-9wq8">Pan in window</td>
  </tr>
  <tr>
    <td class="tg-lboi">PgUp</td>
    <td class="tg-9wq8">Zoom Out</td>
  </tr>
  <tr>
    <td class="tg-lboi">PgDn</td>
    <td class="tg-9wq8">Zoom In</td>
  </tr>
  <tr>
    <td class="tg-lboi">Del</td>
    <td class="tg-9wq8">Delete Selected peaks</td>
  </tr>
  <tr>
    <td class="tg-lboi">F1-F12</td>
    <td class="tg-9wq8">Toggle spectrum<br></td>
  </tr>
  <tr>
    <td class="tg-lboi">a&nbsp;&nbsp;</td>
    <td class="tg-9wq8">Assign peak</td>
  </tr>
  <tr>
    <td class="tg-lboi">h&nbsp;&nbsp;</td>
    <td class="tg-9wq8">Add horizontal ruler</td>
  </tr>
  <tr>
    <td class="tg-lboi">m </td>
    <td class="tg-9wq8">Mark cursor position<br></td>
  </tr>
  <tr>
    <td class="tg-cly1">n<br></td>
    <td class="tg-nrix">Remove&nbsp;&nbsp;marks &amp; rulers<br></td>
  </tr>
  <tr>
    <td class="tg-cly1">p </td>
    <td class="tg-nrix">Move selected peak</td>
  </tr>
  <tr>
    <td class="tg-cly1">v </td>
    <td class="tg-nrix">Add vertical ruler</td>
  </tr>
</tbody>
</table>
