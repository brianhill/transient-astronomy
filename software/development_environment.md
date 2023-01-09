## Development Environment

*Documentation of our development environment choices and procedures*

### Anaconda

The [2022.10 release](https://www.anaconda.com/blog/anaconda-distribution-2022-10) (or higher) of the Anaconda Distribution is the starting point for our development environment. Key tools, services, and apps supporting our work in the Anaconda Distribution of Python are git, GitHub, and TextMate 2.0. All team members are running macOS on MacBooks of various vintages, but we expect our analysis pipeline to be completely portable to any other platform supported by Anaconda.

We begin by making a new environment from the base environment:

`conda create --name transient --clone base`

followed by

`conda activate transient`

It is a good idea to put that in your .zshrc file so that you don't accidentally try to launch jupyter in the base environment.

### Launching  Jupyter

First we need to get Jupyter started. In a Terminal window:

`cd ~/Projects/transient-astronomy/analyses`

`jupyter notebook`

### ccdproc

Out data processing pipeline will use [ccdproc](https://ccdproc.readthedocs.io/en/latest/) for image calibration (lights, darks, flats, and biases).

`conda install -c conda-forge ccdproc`

This installed `ccdproc-2.3.1` and various other dependencies.

In a Jupyter notebook, we will follow the [Getting Started](https://ccdproc.readthedocs.io/en/latest/getting_started.html) documentation for `ccdproc`.

### astroalign and twirl

We will use [astroalign](https://astroalign.quatrope.org/en/latest/) for alignment and [twirl](https://github.com/lgrcia/twirl) for plate-solving.

`conda install -c conda-forge astroalign`

Twirl in turn needs astroquery.gaia. Neither twirl nor astroquery are available through the repo.anaconda.com channels, so we use:

`pip install twirl`

`pip install astroquery`

### astropy.visualization

We will use [astropy.visualization](https://docs.astropy.org/en/stable/visualization/index.html) and/or custom stretching routines to examine images at various stages of the data-processing pipeline.

### photutils

We plan to use [photutils](https://photutils.readthedocs.io/en/stable/getting_started.html) for [PSF photometry](https://photutils.readthedocs.io/en/stable/psf.html).

`conda install -c conda-forge photutils`
