# Transient Astronomy

*A program of directed study and research aimed at pushing the limits of the Deep Springs Observatory and of observing the behavior of transient targets, particularly supernovae.*

Terms 3-6 of Academic Year 2022-2023, Deep Springs College

Mentor/Supervisor: [Prof. Brian Hill](../index.html)

Student Researchers: Luke Suess (DS 21) and Sofia Mikulasek (DS 22)

## Record of Work

A record of our tasks and progress is being maintained:

* [Record of Work](./record_of_work-term_3.html)

## Syllabus

* [Syllabus](./TransientAstronomySyllabus.pdf) &mdash; A PDF that mirrors what is on this web page

## Overview

This directed study will address the following research questions:

1. In the dark skies and high altitude at the [Deep Springs Observatory](../deep-springs-observatory/index.html), what observational techniques and conditions make us the most sensitive and accurate that we can we be in detecting and estimating the changes in brightness of stars possibly as dim as magnitude 20 with the observatory's relatively modest (250mm) telescope? We fully expect to be able to get to magnitude 19. NB: larger numbers are dimmer in the astronomical magnitude system. Before this directed study even begins, we have become confident that our equipment can do photometry on magnitude 18 stars.
2. What are the best practices in the analysis of the data taken in our observations that again push the brightness limits of our setup?
3. What transient targets are of the most interest given our data-taking and analysis capability? We believe that supernovae identified by the [Zwicky Transient Facility (ZTF)](https://www.ztf.caltech.edu) are within our grasp and that supernovae light curves taken over many nights with our gear will be of sufficient interest to astrophysics researchers that we can contribute our results to refereed publications. Supernovae have various brightnesses with the brightest ones having peak luminosity brighter than magnitude 17 (see the Rochester Astronomy of Science's compendium of [Latest Supernovae](https://www.rochesterastronomy.org/supernova.html)). In the unlikely event that research-quality data on supernovae prove to be beyond what we can get from our setup, we will pursue easier targets (e.g., binary star systems and transiting exoplanets).

These questions are mostly in the realm of experimental technique as our setup is, as we begin this study, only beginning to be proven.

## Schedule and Work Plan

This directed study is a blend of a (1) observational astronomy, (2) data-taking with research ambitions, and (3) developing a data-processing pipeline in Python. This blend fits under the model of &ldquo;Research Experience for Undergraduates (REU),&rdquo; as it is known at many institutions.

To carry these three activities out, we need approximately 7 meetings for theory and organization, 14 meetings for joint observation sessions, and 7 meetings for joint analysis sessions.

These numbers are intentionally aligned with how many analytical and laboratory meetings a one-semester Deep Springs course would have if half of its meetings were analytical and half were laboratory. We will necessarily need to adapt if either the analytical or laboratory work takes an unexpected amount of time, while retaining the total target of approximately the same amount of meetings as a one-semester full-load course.

Because we will be limited by Moon, weather conditions, and our general availability, to maximize the opportunity for joint observation sessions, we are spreading this work over three of the seven-week Deep Springs terms, rather than two, which would be more typical for a full-load one-semester course. Both December and January may have quite a few weeks that are so cold that it is hard to do quality observing (although optimistically they could offer many mild weeks). Therefore the Term 3 weeks before Thanksgiving, and the Terms 4 and 5 weeks starting at the beginning of February are likely to present the best opportunities to gather high-quality images.

### Project Activities

All three of us need to be fully cognizant and responsible for the results that we produce. This means that we will (outside of regular meeting times) be independently doing analyses of the data we have taken. Also, all three of us do not need to be present for all data-taking sessions, so there will be data-taking sessions consisting of just pairs of us taking additional data once the techniques have been established to all three of our satisfaction. A typical data-taking session will run from about 7pm to midnight, which includes time for setup and teardown. Some data-taking sessions will be pre-dawn instead of in the evening (e.g., from about 3am to 7am).

### Phases

Although there is definitely not a hard delineation or progression between (1) establishing technique, (2) using that technique, and (3) analyzing and writing up results, there are nonetheless three identifiable phases.

In the first phase, we are principally establishing our experimental technique and just starting to establish our analytical technique. In the second phase, we are principally using our experimental technique while still improving our analytical technique. In the third phase, we are still getting additional data the now-established experimental technique while polishing our analytical technique, and in parallel with that we are writing up the best of the results that we were able to achieve.
Roughly speaking, these three phases will correspond to our activities in the three terms that we propose to do the work (Terms 3, 4, and 5).

### Analytical Work in Python

Analytical work has frequently been referred to above. In the [Spring 2022 Observational Astronomy course](../observational-astronomy/index.html), this work was done in a relatively pedestrian and user-friendly tool called AstroImageJ. Most professional astronomers do similar analyses in other more versatile environments. Among newer astronomers, Python has become the dominant choice. Established astronomers often use IDL and IRAF. Because Python is becoming dominant as a general-purpose environment and it is free, that will be our choice.

Our analysis will involve establishing a data-processing pipeline in Python which we expect to use (i) [ccdproc](https://ccdproc.readthedocs.io/en/latest/) for image calibration (lights, darks, flats, and biases), (ii) [astroalign](https://astroalign.quatrope.org/en/latest/) for alignment, and (iii) [photutils](https://photutils.readthedocs.io/en/stable/getting_started.html) for aperture-annulus photometry. These (and other scientific) packages are most commonly accessed from Jupyter notebooks. Jupyter is an interactive scripting environment for manipulating data, making plots, and running Python code. We will thoroughly document our Python [development environment](./development_environment.html) choices and procedures.

## Grading / Evaluation

* Observational Work &mdash; 25% &mdash; This will be comprised of observatory setup and teardown work as well as approximately 14 data-taking sessions
* Analytical Work &mdash; 25% &mdash; This will be comprised of data processing using Python packages
* Scientific Record-Keeping &mdash; 25% &mdash; Records should include: (a) Target Selection Criteria, (b) Listings of Available Targets and their properties, (c) Conditions of Data-Taking, (d) Factors in Data-Processing
* Project Report and Presentation &mdash; 25% &mdash; We will jointly produce a project report. If our results are sufficiently significant, our project report will be submitted as a paper to a refereed journal (such as the Journal of the AAVSO or the Astronomical Society of the Pacific). We will also present our results to the Deep Springs community as a standalone presentation or as a lecture in the lecture series that is under discussion by CurCom.
