## Development Environment

*Documentation of our development environment choices and procedures*

### Anaconda

The [2022.10 release](https://www.anaconda.com/blog/anaconda-distribution-2022-10) (or higher) of the Anaconda Distribution is the starting point for our development environment. Key tools, services, and apps supporting our work in the Anaconda Distribution of Python are git, GitHub, and TextMate 2.0. All team members are running macOS on MacBooks of various vintages, but we expect our analysis pipeline to be completely portable to any other platform supported by Anaconda.

We begin by making a new environment from the base environment:

`conda create --name transient --clone base`

followed by

`conda activate transient`

It is a good idea to put that in your .zshrc file so that you don't accidentally try to launch jupyter in the base environment.

### `ccdproc`

Out data processing pipeline will use [ccdproc](https://ccdproc.readthedocs.io/en/latest/) for image calibration (lights, darks, flats, and biases).

`conda install -c conda-forge ccdproc`

This installed `ccdproc-2.3.1` and various other dependencies.

### `astroalign`

We plan to use [astroalign](https://astroalign.quatrope.org/en/latest/) for alignment.

### `photutils`

We plan to use [photutils](https://photutils.readthedocs.io/en/stable/getting_started.html) for aperture-annulus photometry.

### Launching  Jupyter

In a Jupyter notebook, we will follow the [Getting Started](https://ccdproc.readthedocs.io/en/latest/getting_started.html) documentation for `ccdproc`.

First we need to get Jupyter started. In a Terminal window:

`cd ~/Projects/transient-astronomy/analyses`

`jupyter notebook`
