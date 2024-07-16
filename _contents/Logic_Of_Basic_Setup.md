---
title: "The logic of the basic experimental setups"
image: 
  path: /assets/images/Gears.jpg
---

<!--- # The logic of the basic experimental setups --->

There are two basic scenarios which normally present themselves:


## Tracking of freely moving animals in the absence of specific visual stimulation

In this context, there are different possibilities:

-   1. Single animal in a single arena
-   2. Multiple animals in a single arena
-   3. Multiple animals, each in a single arena  
      
    Given that tracking of the animals occurs in the absence of visual
    stimulation, it follows that illumination of the arenas need not be
    done with infrared light. Consequently video recording of the
    behaviour of the animal(s) can be performed with ordinary optics
    (i.e. no special light filters are required). Illumination is best
    done from beneath the arena, while the video camera records the
    backlit scene from above.  In the first case, the software of choice
    for tracking could be MARGO, if one is interested in live-tracking
    of the animal. If on the other hand, live-tracking is not important,
    then Ctrax can be used for offline tracking.  
      
    In the case of multiple animals, if one is interested in maintaining
    the identity of the individuals distinct throughout the tracking
    process, then Ctrax would be the tracking software of choice, albeit
    that the tracking can only be performed offline. If, on the other
    hand, it is not important to keep the identity of the animals
    separate during the tracking, i.e. in the case one is only
    interested in knowing the total amount of movement (the total or the
    average distance travelled collectively by all the animals) during
    the tracking period, then the MARGO package can be used to perform
    live-tracking of the multiple animals.


## Tracking of freely moving animals in the presence of specific visual stimulation

In this context it is more customary to track animals under one of
the following two conditions:

-   1. Single animal in a single arena
-   2. Multiple animals, each in a single arena  
      
    In this case, the reason why the condition with "multiple animals in
    a single arena" is not considered is that in this type of setup the
    individuals are under the influence of one another, since they share
    the same arena. This would introduce a source of (possibly unwanted)
    disturbance, in particlar if the objective of the setup is to
    evaluate the response of the animals specifically to the visual
    stimuli.  
      
    In both cases, the software of choice for tracking is MARGO,
    especially if one is interested in live-tracking of the
    individuals. Ctrax could also be used in these cases, albeit the
    tracking can only be performed offline.  
      
    Within the context of tracking animals subjected to specific visual
    stimulation, we can consider two different experimental
    paradigms. Open-loop or closed-loop visual stimulation.


### Open-loop conditions

Under open-loop conditions, the animals are subjected to visual
stimuli, which can be provided by computer-controlled Light
Emitting Diode (LED) panels or by Ultra Short Throw (UST)
projector(s). In open-loop conditions, the tracked behavioural
response of the animals has no effect on the visual stimuli.


### Closed-loop conditions

Under closed-loop conditions the animals are subjected to visual
stimuli, which can be provided by computer-controlled LED panels
or by UST projector(s). In this case the tracked behavioural
response of the animals can affect the visual stimuli: The way in
which the behavioural response of the animals affects the visual
stimuli is determined by programming the software which controls
the visual stimuli to respond in predetermined ways to specific
behavioural parameters. The behavioural parameters are obtained
through live-tracking of the animal's movements.
