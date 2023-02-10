# Transient Astronomy

*A program of directed study and research aimed at pushing the limits of the Deep Springs Observatory and of observing the behavior of transient targets, particularly supernovae.*

Terms 3-6 of Academic Year 2022-2023, Deep Springs College

Mentor/Supervisor: [Prof. Brian Hill](../index.html)

Student Researchers: Luke Suess (DS 21) and Sofia Mikulasek (DS 22)

## Quick Links

#### Work in Progress

* [Index to Targets](./targets/index.html)
* [Record of Work - Term 4](./record_of_work-term_4.html)

#### Target Queries

* [ALeRCE ZTF query](https://alerce.online/?selectedClassifier=stamp_classifier&selectedClass=SN&probability=0.5&ndet=2&ndet=2797&ranking=1&firstmjd=59981&ra=120&dec=55&radius=144000&count=false&page=1&perPage=20) (40&deg; of RA 8h, DEC 55, SN probability > 0.5, discovery MJD > 59981, ordered by discovery, newest first)
* [IAU TNS query](https://www.wis-tns.org/search?&ra=120.0&decl=55.0&radius=40.0&coords_unit=deg&date_start%5Bdate%5D=2023-02-05&date_end%5Bdate%5D=&discovery_mag_min=16&discovery_mag_max=19) (40&deg; of RA 8h DEC 55, discovery mag between 16 and 19, discovery date > 2023-02-05)

#### Weather

* [GFS](https://forecast.weather.gov/MapClick.php?w0=t&w3=sfcwind&w3u=1&w4=sky&w5=pop&w7=rain&w9=snow&w13u=0&w16u=1&w17u=1&AheadHour=0&Submit=Submit&FcstType=graphical&textField1=37.3717&textField2=-117.984&site=all&unit=0&dd=&bw=), [CMC](https://www.cleardarksky.com/c/DpSprObCAkey.html?1), and [ECMWF](https://www.yr.no/en/forecast/graph/2-5346035/United%20States/California/Inyo%20County/The%20Elephant) forecasts

#### Moon Phase

* [Moon Phases &mdash; 2023 &mdash; First Half](./resources/MoonPhases-2023H1.png)

## Syllabus

* [Syllabus](./TransientAstronomySyllabus.pdf) &mdash; A PDF that mirrors what is on this web page

## Overview

This directed study will address the following research questions:

1. In the dark skies and high altitude at the [Deep Springs Observatory](../deep-springs-observatory/index.html), what observational techniques and conditions make us the most sensitive and accurate that we can we be in detecting and estimating the changes in brightness of stars possibly as dim as magnitude 20 with the observatory's relatively modest (250mm) telescope? We fully expect to be able to get to magnitude 19. NB: larger numbers are dimmer in the astronomical magnitude system. Before this directed study even begins, we have become confident that our equipment can do photometry on magnitude 18 stars.
2. What are the best practices in the analysis of the data taken in our observations that again push the brightness limits of our setup?
3. What transient targets are of the most interest given our data-taking and analysis capability? We believe that supernovae identified by the [Zwicky Transient Facility (ZTF)](https://www.ztf.caltech.edu) are within our grasp and that supernovae light curves taken over many nights with our gear will be of sufficient interest to astrophysics researchers that we can contribute our results to refereed publications. Supernovae have various brightnesses with the brightest ones having peak luminosity brighter than magnitude 17 (see the Rochester Astronomy of Science's compendium of [Latest Supernovae](https://www.rochesterastronomy.org/supernova.html)). In the unlikely event that research-quality data on supernovae prove to be beyond what we can get from our setup, we will pursue easier targets (e.g., binary star systems and transiting exoplanets).
4. How does this work inform preparation for the Vera C. Rubin Observatory which is less than two years from its initial large-scale synoptic surveys? For example, can small telescopes do searches for very short time-scale transients (which is one of the signatures for [SETI](https://jradavenport.github.io/seti_with_lsst2023/)?

These questions are necessarily mostly in the realm of experimental technique since our setup is, as we begin this study, only beginning to be proven.

## Schedule and Work Plan

This directed study is a blend of a (1) observational astronomy, (2) data-taking with research ambitions, and (3) developing a data-processing pipeline in Python. This blend fits under the model of &ldquo;Research Experience for Undergraduates (REU),&rdquo; as it is known at many institutions.

To carry these three activities out, we need approximately 7 meetings for theory and organization, 14 meetings for joint observation sessions, and 7 meetings for joint analysis sessions.

These numbers are intentionally aligned with how many analytical and laboratory meetings a one-semester Deep Springs course would have if half of its meetings were analytical and half were laboratory. We will necessarily need to adapt if either the analytical or laboratory work takes an unexpected amount of time, while retaining the total target of approximately the same amount of meetings as a one-semester full-load course.

Because we will be limited by Moon, weather conditions, and our general availability, to maximize the opportunity for joint observation sessions, we are spreading this work over three of the seven-week Deep Springs terms, rather than two, which would be more typical for a full-load one-semester course. Both December and January may have quite a few weeks that are so cold or have such poor weather that it is hard to do quality observing (although optimistically they could offer many mild and clear weeks). Therefore the Term 3 weeks before Thanksgiving, and the Terms 4 and 5 weeks starting at the beginning of February are likely to present the best opportunities to gather high-quality images.

### Project Activities

All three of us need to be fully cognizant and responsible for the results that we produce. This means that we will (outside of regular meeting times) be independently doing analyses of the data we have taken. On the other hand, all three of us do not need to be present for all data-taking sessions, so there will be data-taking sessions consisting of just pairs of us taking additional data once the techniques have been established to all three of our satisfaction. A typical data-taking session during near the third-quarter and new moon phases will run from about 7pm to 11pm, which allows for about two hours for data-taking proper in addition to the necessary targeting, setup, and teardown time of [our equipment](./equipment/index.html). Near the first-quarter moon, data-taking sessions will be pre-dawn instead of in the evening (e.g., from about 2am to 6am).

### Phases

Although there is definitely not a hard delineation or progression between (1) establishing technique, (2) using that technique, and (3) analyzing and writing up results, there are nonetheless three identifiable phases.

In the first phase, we are principally establishing our experimental technique and just starting to establish our analytical technique. In the second phase, we are principally using our experimental technique while still improving our analytical technique. In the third phase, we are still getting additional data using the now-established experimental technique while polishing our analytical technique, and in parallel with that we are writing up the best of the results that we were able to achieve.
Roughly speaking, these three phases will correspond to our activities in the three terms that we propose to do the work (Terms 3, 4, and 5).

### Analytical Work in Python

Analytical work has frequently been referred to above. In the [Spring 2022 Observational Astronomy course](../observational-astronomy/index.html), this work was done in a relatively pedestrian and user-friendly tool called AstroImageJ. Most professional astronomers do similar analyses in other, more versatile environments. Among newer astronomers, Python has become the dominant choice. Established astronomers often use IDL and IRAF. Because Python is becoming dominant as a general-purpose environment and it is free, that will be our choice.

Our analysis will involve establishing Python [Development Environment](./software/development_environment.html) and a data-processing pipeline in this environment which we expect to use (i) [ccdproc](https://ccdproc.readthedocs.io/en/latest/) for [image calibration](./resources/ImageCalibration.pdf) (lights, darks, flats, and biases), (ii) [astroalign](https://astroalign.quatrope.org/en/latest/) and [twirl](https://github.com/lgrcia/twirl) for alignment and plate-solving, (iii) [astropy.visualization](https://docs.astropy.org/en/stable/visualization/index.html) and/or custom stretching routines to examine images, and (iv) [photutils](https://photutils.readthedocs.io/en/stable/getting_started.html) and in particular [photutils.psf](https://photutils.readthedocs.io/en/stable/psf.html) for PSF photometry. These (and other scientific) packages are most commonly accessed and built upon using Jupyter notebooks. Jupyter is an interactive scripting environment for manipulating data, making plots, and running Python code. We will document our Python [development environment](./software/development_environment.html) choices and procedures as well as the notebooks themselves.

Challenges in photometry are to be expected because targets are generally superimposed directly on galaxies of comparable magnitude. We imagine four strategies from which the required artistry in photometry will emerge:
  
  1.  Ordinary PSF photometry
  2.  PSF photometry with a fitted gradient background
  3.  PSF photometry by subtracting PanSTARRS images of the host galaxies (scaled to the plate-scale of our telescope, and possibly convolved to model our seeing)
  4.  PSF photometry one to two months after the supernovae have achieved peak brightness, using our images of the essentially-bare galaxies as background

## Grading / Evaluation

* Observational Work &mdash; 25% &mdash; This will be comprised of approximately 14 data-taking sessions
* Analytical Work &mdash; 25% &mdash; Developing and applying the data-processing workflow in Jupyter
* Scientific Record-Keeping &mdash; 25% &mdash; Records should include: (a) Target selection criteria starting with listings of available targets and their properties, (b) Conditions of data-taking, (c) Factors during observation that are relevant to data quality and data processing
* Project Report and Presentation &mdash; 25% &mdash; We will jointly produce a project report. If our results are sufficiently significant, our project report will be submitted as a paper to a refereed journal (such as the Journal of the AAVSO or the Astronomical Society of the Pacific). We will also present our results to the Deep Springs community as a standalone presentation or as a lecture in the lecture series that is under discussion by CurCom.
