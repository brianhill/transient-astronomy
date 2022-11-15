## Record of Work &mdash; Term 3

Transient Astronomy [home page](./)

*An [index of our analyses](./analyses/index.html)*

*A [moon phases table](./resources/MoonPhasesTable.png) for planning observing sessions*

### Week 0 &mdash; First Observations

* 2022-10-18 &mdash; Observed [NGC 869](./analyses/2022-10-1819-NGC_869/index.html)
* 2022-10-21 &mdash; Observed [Supernova 2022vqz](./analyses/2022-10-2122-SN_2022vqz/index.html)
* 2022-10-24 &mdash; Observed [Supernova 2022vqz](./analyses/2022-10-2425-SN_2022vqz/index.html)

### Week 1 &mdash; Start Development of Analysis Pipeline

* 2022-10-25 &mdash; Created [Development Environment](./software/development_environment.html) consisting of Anaconda Python distribution, TextMate 2.0, and Xcode Command-Line Developer Tools (for git) &mdash; Created GitHub accounts &mdash; Created clones of this git repository and did first shared edits
* 2022-10-29 &mdash; Made first Jupyter notebook and installed [ccdproc](https://ccdproc.readthedocs.io/en/latest/)

### Week 2 &mdash; Establish Image Calibration Part of Pipeline

* 2022-11-03 &mdash; Did small demonstration for TDS (Mark and Ryan were guests). Sofia and Luke led deployment of scope, observation, and shut down, using our [setup and teardown procedure](./equipment/SetupAndTeardownProcedure.pdf)
* 2022-11-05 &mdash; Used ccdproc for [image calibration](./resources/ImageCalibration.pdf) of our 2022-10-2425 data
* 2022-11-06 &mdash; Created a test notebook to thoroughly validate our image calibration code

### Week 3 &mdash; Establish Image Alignment Part of Pipeline

* 2022-11-13 &mdash; Used [astroalign](https://astroalign.quatrope.org/en/latest/) for alignment

### Week 4 &mdash; Establish Visualization Part of Pipeline &mdash; Start Photometry

* 2022-11-14 &mdash; Used [astropy visualization](https://astroalign.quatrope.org/en/latest/) to normalize and stretch the images for visual examination
* 2022-11-16 &mdash; Combine all the aligned lights and apply aperture-annulus photometry using [photutils](https://photutils.readthedocs.io/en/stable/getting_started.html) and in particular [photutils.aperture](https://photutils.readthedocs.io/en/stable/aperture.html).

## To-Do

*Various loose ends*

* Tests of our usages of astroalign
* Experimentation with better image-stretching routines
