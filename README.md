# RESS for Alakazam

A plugin for [Alakazam](https://github.com/markspan/Alakazam): rhythmic entrainment source separation: for each tagged frequency, a spatial filter over the scalp channels, added as a channel, so that a frequency-tagged response is read from one component rather than from an electrode chosen by hand.

It was part of Alakazam until it became a plugin of its own, so that it can be
installed, upgraded and documented on its own.

## Manual

The manual is on this repository's pages:
<https://markspan.github.io/AlakazamRESS/>.

## Installing

In Alakazam, **Install plugins** on the Alakazam tab lists this repository:
select it and press **Install**. It installs the latest release. A zip from
the [releases](https://github.com/markspan/AlakazamRESS/releases), or one built with
`build`, installs the same way through **From a link**, and so does the link
to this repository. The tool appears on the Tools tab, as it did before.

It needs Alakazam V0.4.5.4 or newer, the first without `RESS` built
in. Workspaces and templates made with the built-in tool open and
recalculate as before once the plugin is installed; Alakazam offers to
install it when one needs it.

## Building and testing

```matlab
build()                                    % dist/RESS-<version>.zip
runtests('tests')                          % the tool's tests and the install
```

The tests need Alakazam's source: the folder in `ALAKAZAM_ROOT`, or the
Alakazam repository beside this one.

The method is implemented here from Cohen and Gulbinaite's article (2017, NeuroImage 147, 43-56, doi:10.1016/j.neuroimage.2016.11.036), which a publication using it should cite.

## Licence

GPL-3.0, as Alakazam.
