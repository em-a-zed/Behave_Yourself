---
title: "35. Custom Code: Matlab Scripts"
image: 
  path: /assets/images/Custom_code_Matlab_Hero.png
---

<!--- # General concepts --->


The Matlab scripts described here can be found in this Github
Repository: [Matlab
Scripts](https://github.com/em-a-zed/Custom-Tracking-Code/tree/main/Matlab)

### Script to track a tethered fly

This script was written to allow relatively fast tracking of single
*Drosophila melanogaster* adult individuals. The particular application
in which this script was employed entailed a tethered adult fly. The
tethered fly preparation relies on glueing a very thin steel pin (i.e.
minutien pins from [Fine Science](https://www.finescience.com/)) to the
dorsal thorax of the fly. The pin is then suspended in a magnetic field,
allowing it (and the attached fly) to freely rotate around its
longitudinal axis, i.e. as described in (Duistermars and Frye 2008).\
This preparation allows the tethered individual to \"fly\" restricting
its movements exclusively to rotations about the axis defined by the
steel pin (i.e. yaw). Translations in space in any direction are
effectively impeded. The video tracking of the suspended individual
occurs from beneath (i.e. the camera is placed beneath the tethered
fly). The fly is illuminated with infrared light from above, and
patterns are presented to the fly in the same way used to visually
stimulate free-moving individuals in an open arena.

![image-center]({{ site.url }}{{ site.baseurl}}/assets/images/Tethered_Fly.png)

The script is fairly well commented, so that many aspects of the
script's logic can be desumed by the comments alone.\
Briefly:

-   The script initially defines the video source (i.e. the camera).
    This entails having previously loaded into the the Matlab
    environment the appropriate driver for the camera model being used.

-   One of the advantages of the Matlab scripting environment is that it
    allows the programming of relatively complex tasks, while also
    making it possible to define a simple but effective Graphical User
    Interface (GUI) with relatively few lines of code.

-   In the next step, the script defines the opening of a \"file
    selection dialog\", allowing the user to define the name and
    location of the file into which the tracking data will be saved. A
    file with the same name, but different extension will also be
    produced, allowing to save a recording of the video captured by the
    camera. As can be seen from the script, this is optional and depends
    upon whether the user is interested in saving the video information
    or not. Whatever the case, the numeric data pertaining to the video
    tracking will always be saved in a text file (.txt extension).

-   The next section opens a preview window presenting the user with a
    view of what is currently visible to the video camera. At the same
    time a single frame of the visible scene is captured allowing the
    user to define a Region Of Interest (ROI) to define the specific
    region, which will then be targeted by the tracking algorithm.

-   The next section uses the ROI to create a side-to-side copy of the
    same image. One copy is a greyscale representation of the ROI, while
    the other represents a thresholded version (i.e. black and white
    representation), allowing the user to select the threshold grey
    level using a slider control, which will define the distinction
    between what will be represented as black and what will be
    represented as white in the thresholded image. The tracking
    algorithm relies on this representation of the object to track in
    order to optimize the tracking process (i.e. only the black pixels
    will be tracked).

-   The tracking algorithm employs a strategy, based on the
    approximation of the object to be tracked by an ellipsoid. If the
    object to be tracked presents sufficiently distinct anterior and
    posterior ends, the ellipsoid approximation will allow to precisely
    track the anterior and posterior ends via the focal points of the
    ellipsoid (i.e. the front-to-back orientation). Thus the rotations
    of the object about the axis of rotation, can be monitored by
    tracking the rotation of the longitudinal axis of the ellipsoid, as
    well as the movement of the focal points. This is all defined in the
    function *get~ellipse~(Img, direct)*. This approach was described by
    Raphael Candelier and further details can be found here:
    [Candelier](https://raphael.candelier.fr/?blog=Image%20Moments)

-   Now the system is ready to track the tethered fly. The script waits
    for the command (the click of a button by the user) which will start
    the tracking.

-   The tracking can be viewed in real time by plotting a graphical
    representation of the ellipsoid itself, it's longitudinal axis and
    the anterior and posterior ends of the identified object. This is
    done by the function *displayTrackingResults()*.

-   Tracking will continue until the user clicks on the button
    specifying to stop the tracking.

-   The script then proceeds to save all the tracking data into the
    specified file, to close the preview window, turn off the camera and
    terminate the script.
