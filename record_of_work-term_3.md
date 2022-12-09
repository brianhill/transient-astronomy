## Record of Work &mdash; Term 3

Transient Astronomy [home page](./)

See also [Record of Work - Term 4](./record_of_work-term_4.html)

### Week 0 &mdash; First Observations

* 2022-10-18 &mdash; Observed [NGC 869](./analyses/NGC_869/2022-10-1819-NGC_869/index.html)
* 2022-10-21 &mdash; Observed [Supernova 2022vqz](./analyses/SN_2022vqz/2022-10-2122-SN_2022vqz/index.html)
* 2022-10-24 &mdash; Observed [Supernova 2022vqz](./analyses/SN_2022vqz/2022-10-2425-SN_2022vqz/index.html)

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
* 2022-11-15 &mdash; Brian presented ([slide deck](https://brianhill.github.io/resources/2022-11-15-BRDSC.pdf)) [Presentation to The Basin and Range Dark Sky Cooperative (BRDSC)](https://brdarkskies.org/about/), November 15th, 2022 &mdash; Will likely have an on-site assessment by Dan Duriscoe, Principal at [Night Sky Metrics](https://nightskymetrics.com)
* 2022-11-16 &mdash; Combined all the aligned lights and then found all the stars using [photutils](https://photutils.readthedocs.io/en/stable/getting_started.html) 

### Week 5 &mdash; Improve Visualization Part of Pipeline &mdash; Attempt first g' and r' Observations of Brightening Supernova

* 2022-11-19 &mdash; Observed candidate [Supernova AT2022aaco](./analyses/SN_AT2022aaco/2022-11-1920-SN_AT2022aaco/index.html) (Brian, Luke, and Sofia)
* 2022-11-20 &mdash; Observed candidate [Supernova AT2022aaco](./analyses/SN_AT2022aaco/2022-11-2021-SN_AT2022aaco/index.html) (Brian and Ben)
* 2022-11-21 &mdash; Apply aperture-annulus photometry using [photutils.aperture](https://photutils.readthedocs.io/en/stable/aperture.html) &mdash; Write a routine that takes a numpy array and does row-wise subtraction of median values &mdash; Improve LogStretch routine
* 2022-11-23 &mdash; Observing session (Luke and Sofia) &mdash; Encountered instrument problems(!)

### Week 6 &mdash; Selected 2nd Brightening Supernova

* 2022-11-27 &mdash; POSTPONED: Work with Dan Duriscoe to determine local sky brightness
* 2022-11-29 &mdash; [SN_2022abik](./analyses/SN_2022abik/index.html)

### Week 7 &mdash; Summarized and Presented Work to Date

* 2022-12-03 &mdash; Calibration runs for SN 2022abik
* 2022-12-08 &mdash; Delivered [Transient Astronomy at Deep Springs-Part I](./presentations/2022-12-08-TransientAstronomyAtDeepSprings-PartI.pdf) as a Deep Springs community address

### Week 8 &mdash;
