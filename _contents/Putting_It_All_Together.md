---
title: "25. Putting it all together"
image: 
  path: /assets/images/Puzzle_Hero.jpg
---

<!--- # General concepts --->

# The following are a couple of schematized tracking setups
In the first case the setup consists in a cylindrical LED panel enclosure at the bottom of which there is a circular 3D-printed transparent-resin arena with a transparent glass top. The arena is illuminated from beneath with an array of Infrared LEDs, while the tracked individual (in this case a fly) is video-recorded using a digital camera equipped with a longpass IR filter. Visual stimulation of the individual occurs via programmed patterns transmitted by the computer software to the arrays of LEDs.

<br />
<br />
![image-center]({{ site.url }}{{ site.baseurl}}/assets/images/Tracking-Setup-LED.jpg)
<br />
<br />
In the second case the setup consists in a cylindrical frosted (sanded) plexiglass enclosure at the bottom of which there is a circular 3D-printed transparent-resin arena with a transparent glass top. The arena is illuminated from beneath with an array of Infrared LEDs, while the tracked individual (in this case a fly) is video-recorded using a digital camera equipped with a longpass IR filter. Visual stimulation of the individual occurs via programmed patterns transmitted in a coordinated way by the computer software to the pair of UST projectors which project onto opposite sides of the curved surface of the frosted plexiglass cylinder.

<br />
![image-center]({{ site.url }}{{ site.baseurl}}/assets/images/Tracking-Setup-UST.png)

<br />
# Placing and connecting the components

In general, components of setups, such as those described in the
preceding section, should be ideally placed in a light-tight enclosure
or in a dark room in order to ensure that the animals do not receive any
undesired visual signals. This is true both for conditions which
envisage visual stimulation (via LED panels or via projectors) as well
as for experimental conditions which do not contemplate any specific
visual stimulation.\
Apart from this, the required components should ideally be placed on a
relatively stable (possibly vibration free) surface/bench. Often,
alluminium black breadboard surfaces (i.e. see the section dealing with
*optomechanics*) can be extremely useful because they provide handy ways
with which to sturdily fix camera and/or projector holders, through the
use of alluminium posts and clamps. For a very basic example of this see
the figure below:

![image-center]({{ site.url }}{{ 
	site.baseurl}}/assets/images/My_Apparatus_Edit.png)

The figure shows a wide field view of the whole setup. The UST projector
is circled in red, while the video camera above the
frosted-surface-plexiglass cylinder is circled in green. These two parts
are shown as enlargements in the following two figures.\
The first image shows the UST projector placed upon a metal plate, which
is fixed, through small mounting posts screwed onto a large alluminium
breadboard base.

![image-center]({{ site.url }}{{ 
	site.baseurl}}/assets/images/Projector_Only.png)


The second image shows the frosted-surface-plexiglass cylinder, with
above it the videocamera connected to an \"overhead camera platform\"
(from [Glidegear](https://glidegear.net/)). The plexiglass cylinder sits
on top of a custom made transparent plexiglass \"table\" and surrounds a
circular arena (not visible) which also sits on the plexiglass platform.
Immediately below the plexiglass platform is a glass mirror placed at a
45 degree angle with respect to the horizontal. The mirror reflects
infrared light upward through the plexiglass table to the video camera
above. Thge IR light is projected from a circular array of IR LEDs,
placed to the right of the image (in front of the mirror), and fixed to
a mini alluminium breadboard with a specific holder.

![image-center]({{ site.url }}{{ 
	site.baseurl}}/assets/images/Plex_Cylin&Camera.png)


The breadboards, posts, IR LED array and LED array holder are all from
[Thorlabs](https://www.thorlabs.com/).

<br />
# Two computers: separating visual stimulation from tracking

In some circumstances it may be desirable to control the visual
stimulation apparatus (i.e. UST projector(s)) and the tracking of the
experimental animal(s) separately (i.e. by using a separate computer for
each task). This may become necessary to improve the performance of the
two tasks, especially in terms of the speed of the tracking.\
In our experience, a situation of this type occurred when performing the
tracking of a single animal using a Matlab script (for an example see
the *Code: Matlab Scripts* section), while the visual stimulation was
being performed under the control of a Python script using the Psychopy
library (for an example see the *Code: Python Scripts* section). This
turned out to be a problematic situation for a single computer to
handle, leading to a very noticeable slowing down of the tracking. In
this case we resorted to running the two scripts on separate computers.
We thus adopted a \"quick and dirty\" solution to the problem. The two
computers were connected by way of two
[Arduino](https://www.arduino.cc/) boards, leveraging on the fact that
there are Arduino libraries available both for Matlab and for Python.
Such libraries allow a computer to communicate with the Arduino board
through a USB connection, using a serial communication protocol.
Communication between the Arduino boards is established by wiring the
two boards via a single digital I/O pin on each board. The state of the
connected Arduino digital pins can be controlled directly from the
Python and/or Matlab scripts. This allows to send discrete signals from
one script to the other, permitting the synchronization of tasks between
the two computers. Indeed, in this case, all that was needed was to have
the possibility of sending signals between the two computers in order to
synchronize the tracking with the visual stimulation, in particular in
closed-loop situations. The logic of this process implies that the
\"sender\" computer sends a signal to a specified digital I/O pin on the
Arduino board to which it is connected via USB, while the \"receiving\"
computer continues polling the equivalent digital I/O pin on the Arduino
board to which it is connected via USB for a received signal. Probably
the best model of Arduino boards for this application would be the
*Mega* model, since this model has a slightly greater processing power,
resulting in faster processing speed (so that there should be very
little delay in the communication between the two computers).\
With this type of connection, it is very important that the two Arduino
boards share a common ground connection in order to guarantee that each
board can correctly interpret an incoming signal as being significantly
above the threshold to be interpreted as a positive signal.\
The same kind of approach could be adopted using
[ESP32](https://www.espressif.com/) boards (see the Post on ESP32)
instead of the Arduino Mega boards. In this case, it would also be
possible to take advantage of the extensive wireless communication
possibilities offered by these boards, instead of hardwiring the two
boards together.

<br />
# Controlling external devices

The need to employ Arduino, ESP32 or similar boards most often arises
when it becomes necessary to interface the tracking and/or visual
stimulation scripts to allow them to also control external devices. For
example, in the case of *Drosophila melanogaster* strains genetically
manipulated to allow the optogenetic activation of specifically
engineered genes, it may become necessary to allow for the temporally
controlled activation/inactivation of such genes during an experiment
(as described for example in (Meda et al. 2020)). This would require the
automatic switching on and off of specifically designed narrow bandwidth
emitting LEDs. Such a task can be easily implemented by using Arduino
technology. The Arduino board is connected to the controlling computer
via USB, and the optogenetic LEDs circuit can be connected to one of the
digital I/O pins of the Arduino, which in turn can be addressed directly
from the tracking/visual stimulation script(s), by means of the specific
commands made available through the Python and/or Matlab Arduino
libraries.\
It is possible to perform the same task using a
[LabJack](https://labjack.com/) interface, since such interfaces also
have dedicated libraries which work with Matlab and Python. The LabJack
family of interfaces are more expensive than Arduino or ESP32 boards,
but they allow for high frequency communication through their GPIO pins,
while perhaps also being a little more user friendly to handle.
