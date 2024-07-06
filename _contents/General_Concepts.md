---
title: ""
image: 
  path: /assets/images/Gears.jpg
---

# General concepts

## The problem

-   If you are reading this, then you are likely interested in
    video-tracking of animals for behavioural studies.

-   This guide is an attempt to provide indications on how to
    approach this problem starting from the basics. As the title
    implies, the idea is to provide suggestions on how to implement
    everything that is required on a Do It Yourself basis, both from
    the hardware as well as from the software points of vew.

-   Although this may seem a difficult undertaking, in reality it is
    relatively simple. All that is required is some programming
    experience as well as a basic knowledge of electronics.

-   I will deal with the subject matter mainly referring to
    behavioural experimentation in the lab involving *Drosophila
    melanogaster* as the model organism. However, most of what will
    be exposed can be adapted to other laboratory model organisms
    with relative ease.


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

