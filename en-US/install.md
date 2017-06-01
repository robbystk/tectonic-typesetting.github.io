---
layout: default
title: Installation — The Tectonic Project
---

# Installing Tectonic

We distribute Tectonic for both Linux and MacOS machines. Installation
requires that you be comfortable with using a terminal. So does using Tectonic
itself, for that matter.

Because Tectonic relies on a somewhat broad set of support libraries, the
recommended installation method is based on
[Continuum Analytics](https://www.continuum.io/)’ Anaconda Python framework,
even though nothing in Tectonic uses Python.

<p class="bs-callout bs-callout-warning">Suggestions for alternate
installation methods are welcomed! We are happy to provide other installers
but are not sure what the community needs. Please express your preferences at
<a href="https://github.com/tectonic-typesetting/tectonic/issues/4">GitHub
issue #4</a>.</p>


## Using Anaconda (Recommended)
### If you already have Anaconda Python installed:

The support libraries that we use are only provided through
[conda-forge](http://conda-forge.github.io/), a community-led project that
emulates and updates the official Anaconda system. To use Tectonic you must
start using conda-forge packages. *The packages from conda-forge will replace
nearly all of the ones from a stock Anaconda installation, but that’s OK.* The
replacement packages aim to be drop-in replacements for the standard
distribution.

If you are already using conda-forge, you don’t need to change anything.
Otherwise, run this command to enable conda-forge in your installation:

```
conda config --add channels conda-forge
```

The pre-compiled Tectonic installation is distributed through a separate
“channel” that provides the necessary dependencies. To complete the
installation, run these commands:

```
conda config --add channels pkgw-forge
conda install tectonic
tectonic --help # test that the program works
```


### If you need to install both Tectonic and Anaconda Python:

We recommend that you use Continuum’s “Miniconda” installer to get set up
quickly. First, install Miniconda
[according to these official instructions](https://conda.io/docs/install/quick.html).

Once Miniconda is installed you may need to open a new terminal in order for
its changes to take effect. If all went well, the command `conda` will now be
available in your terminal. Proceed using the instructions given in the
previous section.

## Using The AUR on Arch Linux

## Using Cargo

Install [cargo](http://doc.crates.io/), the Rust package manager,
using your system's package installer.
Then run
```
cargo install tectonic
```
to install tectonic and all of its dependencies

## Using the Linux Subsystem on Windows
