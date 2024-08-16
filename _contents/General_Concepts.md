---
title: "05. General concepts"
image: 
  path: /assets/images/Gears.jpg
---

<!--- NEED TO THANK FOR GRAPHIC CONTENT --->
<!--- https://pixabay.com/illustrations/search/circuit%20boards/ --->

<!--- # General concepts --->

## The problem

-   If you are reading this, then you are likely interested in
    video-tracking of animals for behavioural studies.

-   This guide is an attempt to provide indications on how to approach
    this problem starting from the basics. As the title implies, the
    idea is to provide suggestions on how to implement everything that
    is required on a Do It Yourself basis, both from the hardware as
    well as from the software points of vew.

-   Granted, there are commercial solutions available. Some of these
    deal with all the aspects of animal tracking in the laboratory,
    offering a complete package which includes the required hardware as
    well as the software (i.e. [Noldus](https://www.noldus.com/)).
    Others, such as [ANY-maze](https://www.any-maze.com/), proved the
    tracking software. In both cases the software is conceived to handle
    all aspects of the tracking process, such as data acquisition and
    storage, experiment design, statistical data analysis and reporting
    of results. This paper reports a comparison of the performance of
    the two systems (Lim et al. 2023).

-   I will deal with the subject matter mainly referring to behavioural
    experimentation in the lab involving *Drosophila melanogaster* as
    the model organism. However, most of what will be exposed can be
    adapted to other laboratory model organisms with relative ease.


## The solutions

-   At the most basic level what will be needed is:
    1.  a transparent enclosure (arena) into which to place the
        animal(s) to be tracked;
    2.  a digital video camera with which to capture the movements of
        the subjects;
    3.  a computer to which the camera will be attached and which will
        run the software being used to capture the video footage
        and/or perform the real time tracking.

-   Some further considerations which could be made are related, for
    example, to the type of lighting to use during the video
    recording/tracking. Typically you would need to adequately
    illuminate the scene using some form of "normal" visible white
    light. While this may be fine for just tracking animals in a
    visually unchanging environment, this may not be a good solution
    when the video recording/tracking is performed while providing
    the subject with visual stimuli (i.e. the visual environment
    surrounding the subject is not static). In this case, the visual
    stimuli will also be "seen" by the camera and by the tracking
    software and this will cause interferences with the tracking
    process. One solution is to illuminate the scene with infra-red
    light and to equip the video camera with a long pass Infra Red
    (IR) filter. This guarantees that the video camera will only be
    able to "see" the animals (illuminated by the IR light) and not
    the visual stimuli (which should be restricted to the visibile
    part of the light spectrum).


### Further considerations on lighting

Since correct lighting is a key issue in this context, it is worth
considering the possibility of housing the arena, camera and the
UST projector (if one is being used to provide visual stimuli to
the experimental animals) in a light-proof enclosure. There are
many ways in which this can be constructed, with materials ranging
from plywood to aluminium and black acrylic (i.e. the latter, as
described here: [MARGO](https://github.com/de-Bivort-Lab/margo)).

