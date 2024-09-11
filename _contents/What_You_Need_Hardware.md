---
title: "15. What you will (or might) need: Hardware"
image: 
  path: /assets/images/Hardware_Hero.jpg
---

<!--- # General concepts --->


<h3 id="sec:orgcb37a62">Electronics</h3>
<ol>
<li><p><strong>Arduino</strong> <span id="sec:org5619048"
label="sec:org5619048"></span></p>
<p>Arduino electronic boards are open-source hardware platforms designed
for creating digital devices and interactive objects that can sense and
control physical elements. They are popular for their ease of use,
versatility, and wide range of applications in electronics projects.
Here are some key characteristics:</p>
<ol>
<li><p><strong>Microcontroller-Based</strong>: Each Arduino board comes
with a microcontroller (e.g., ATmega328 on the Arduino Uno), which acts
as the brain of the board, executing programmed instructions.</p></li>
<li><p><strong>Digital and Analog I/O Pins</strong>: Arduino boards have
multiple input and output pins that can be used to connect sensors,
LEDs, motors, and other electronic components.</p></li>
<li><p><strong>Programming Environment</strong>: Arduino uses a
simplified version of C/C++ and comes with an integrated development
environment (IDE) that is user-friendly and easy to learn.</p></li>
<li><p><strong>USB Connectivity</strong>: Most boards can be connected
to a computer via USB for programming and power supply.</p></li>
<li><p><strong>Wide Compatibility</strong>: Arduino is compatible with a
vast array of sensors, modules, and shields that extend its
functionality.</p></li>
</ol>
<p>Some typical applications for Arduino boards:</p>
<ul>
<li><p><strong>Prototyping</strong>: Rapid development of electronic
prototypes.</p></li>
<li><p><strong>Education</strong>: Teaching electronics and
programming.</p></li>
<li><p><strong>Robotics</strong>: Controlling robots and automation
systems.</p></li>
<li><p><strong>IoT</strong>: Creating Internet of Things devices that
can communicate over networks.</p></li>
<li><p><strong>DIY Projects</strong>: Building personal projects, such
as home automation systems, wearable technology, and interactive
art.</p></li>
</ul>
<p>Other important points of strength of the Arduino project are:</p>
<ul>
<li><p><strong>Open Source</strong>: The hardware and software are
open-source, allowing for customization and community
contributions.</p></li>
<li><p><strong>Extensive Documentation</strong>: A wealth of tutorials,
forums, and examples are available online.</p></li>
<li><p><strong>Libraries</strong>: Numerous libraries are available to
simplify the use of various sensors and modules.</p></li>
</ul>
<p>This is the link to the Arduino development board, software download
and documentation pages: <a
href="https://store.arduino.cc">Arduino</a></p></li>
<li><p><strong>LED Panels</strong> <span id="sec:org6863123"
label="sec:org6863123"></span></p>
<p>LED-based panels can efficiently be employed to present visual
stimuli to model organisms. In 2008, Michael Reiser and Michael
Dickinson <span class="citation"
data-cites="reiser_modular_2008">(Reiser and Dickinson 2008)</span>
reported the design of an approximately cylindrical modular display
system for insect behavioral neuroscience. Following that report, the
design was further updated, and all the technical details for the
construction of such modular systems were made publicly available
through the author’s Github website <a
href="https://reiserlab.github.io/Modular-LED-Display/">Modular-LED-Display</a>.
The website documents everything required to implement a fully
functional system, including commercial sources for the LED panels, the
electronics, the hardware and the software required to control them. As
of writing, the LED panels used are monochromatic (i.e. green LEDs),
however this also results in very high speed refresh rates (up to 500Hz,
with 256 brightness levels).</p></li>
<li><p><strong>Ultra-Short-Throw Digital Projectors</strong> <span
id="sec:orged2025c" label="sec:orged2025c"></span></p>
<p>UST projectors refer to "Ultra Short Throw" projectors. These are
specialized projectors designed to project large images from a very
short distance to the screen or wall. In general, UST projectors can
project large images(e.g., 250cm, diagonal, or more) from just a few
centimeters away from the screen or the surface on which to project the
image. This is achieved through advanced lens and mirror systems.
Nowdays, such projectors are widely available on the consumer market at
relatively affordable prices, depending on the required quality of the
projected image (i.e. resolution, brightness and contrast). However, the
applications envisaged in the specific context being considered here,
require the projection of high definition, high contrast images, having
sizes in the range of 25cm (diagonal). The type of projectors that have
such characteristics are those designed for applications requiring the
short distance projection of relatively small images which can function
as user interfaces (i.e. touch screen functions on common surfaces, such
as walls or panels of any material, including glass).<br />
Currently we are using projectors from <a
href="https://www.ti.com/">Texas Instruments</a> (Texas Instruments, DLP
LightCrafter™ Display 4710 EVM Gen2).</p></li>
<li><p><strong>Digital Cameras</strong> <span id="sec:org3dca672"
label="sec:org3dca672"></span></p>
<p>When selecting video cameras for video tracking applications, certain
characteristics are particularly desirable to ensure accurate and
efficient tracking performance. Here are some key attributes to
consider:</p>
<ol>
<li><p><strong>High Frame Rate</strong>: High frame rates (60 fps or
higher) are essential for capturing smooth motion, which is crucial for
accurately tracking fast-moving objects.</p></li>
<li><p><strong>High Resolution</strong>: High resolution allows for more
detailed images, which can improve the accuracy of the tracking
system.</p></li>
<li><p><strong>Low Latency</strong>: Low latency ensures that the video
feed is processed in real-time, which is critical for responsive
tracking.</p></li>
<li><p><strong>Global Shutter</strong>: Global shutters capture the
entire frame at once, as opposed to rolling shutters which capture the
frame line by line.</p></li>
<li><p><strong>High Dynamic Range (HDR)</strong>: HDR capability allows
the camera to capture details in both very bright and very dark areas of
the scene.</p></li>
<li><p><strong>Good Low-Light Performance</strong>: Many tracking
applications may occur in low-light or variable lighting
conditions.</p></li>
<li><p><strong>Robust Connectivity</strong>: Fast and reliable data
transfer is essential for high-performance tracking.</p></li>
<li><p><strong>Software and SDK Support</strong>: Comprehensive software
support ensures that the camera can be easily integrated into existing
systems.<br />
</p></li>
</ol>
<p>Example Cameras for Video Tracking:</p>
<ul>
<li><p><strong>FLIR Blackfly S</strong>: Known for high frame rates,
global shutter, and high resolution.</p></li>
<li><p><strong>Basler ace</strong>: Offers a range of resolutions and
frame rates, and is compact and lightweight.</p></li>
<li><p><strong>XIMEA xiQ Series</strong>: Compact design with high frame
rates and low latency, ideal for embedded systems.</p></li>
</ul>
<p>Selecting the right video camera for tracking depends on the specific
requirements of your application, such as the speed of the objects being
tracked, lighting conditions, and integration needs.</p>
<p>Currently in our labs we use two types of digital cameras:</p>
<ul>
<li><p>Chameleon3 USB3 digital cameras by FLIR Systems (formerly Point
Grey Research). This is the link to <a
href="https://www.flir.com/">FLIR</a>.</p></li>
<li><p>Ximea digital cameras. This is the link to <a
href="https://www.ximea.com/">XIMEA</a></p></li>
</ul>
<p>The Chameleon3 USB3 digital cameras, are a line of high-performance,
compact digital cameras designed for a variety of applications including
industrial inspection, scientific imaging, and machine vision. Here are
some key features and details about the Chameleon3 USB3 digital
cameras:</p>
<ol>
<li><p><strong>USB 3.0 Interface</strong>: These cameras utilize the USB
3.0 interface, providing high data transfer rates of up to 5 Gbps, which
allows for faster image capture and transfer.</p></li>
<li><p><strong>High-Quality Sensors</strong>: Chameleon3 cameras are
equipped with high-quality CMOS and CCD sensors from leading
manufacturers like Sony and On Semiconductor, offering resolutions
ranging from VGA to several megapixels.</p></li>
<li><p><strong>Compact and Lightweight Design</strong>: The cameras are
designed to be compact and lightweight, making them suitable for
integration into various systems where space is limited.</p></li>
<li><p><strong>Flexible Configuration</strong>: They come with flexible
configuration options including adjustable frame rates, exposure times,
and gain settings, allowing customization to suit specific application
needs.</p></li>
<li><p><strong>Image Quality</strong>: These cameras provide high image
quality with features like low noise, high dynamic range, and excellent
sensitivity, making them suitable for capturing detailed and accurate
images in various lighting conditions.</p></li>
<li><p><strong>Software and SDK Support</strong>: The Chameleon3 cameras
are supported by FLIR’s FlyCapture software and SDK, which provide
comprehensive tools for camera control, image capture, and image
processing. This makes it easier for developers to integrate the cameras
into their applications.</p></li>
<li><p><strong>Versatility</strong>: These cameras are used in a wide
range of applications including machine vision, robotics, medical
imaging, microscopy, and scientific research due to their reliable
performance and versatility.</p></li>
<li><p><strong>Compatibility</strong>: The cameras are compatible with a
variety of operating systems including Windows, Linux, and macOS,
ensuring broad usability across different platforms.</p></li>
</ol>
<p>The XIMEA MQ013RG-ON is a model from XIMEA’s xiQ series of USB3
Vision cameras, known for their compact size, high performance, and
versatility. Here are some key features and details:<br />
</p>
<ol>
<li><p><strong>Sensor</strong>: The MQ013RG-ON uses the ON Semiconductor
AR0134 CMOS sensor. It is a 1.2-megapixel sensor with a resolution of
1280 x 960 pixels. The sensor size is 1/3 inch, which is a standard size
for many industrial and scientific imaging applications.</p></li>
<li><p><strong>Frame Rate</strong>: The camera supports a high frame
rate of up to 60 frames per second (fps) at full resolution. This makes
it suitable for applications requiring fast image capture, such as
high-speed industrial inspection or real-time monitoring.</p></li>
<li><p><strong>Interface</strong>: The camera features a USB 3.0
interface, providing high data transfer rates up to 5 Gbps. USB 3.0
ensures fast and reliable data transmission, making it ideal for
high-resolution and high-speed imaging applications.</p></li>
<li><p><strong>Compact Design</strong>: The MQ013RG-ON is known for its
extremely compact and lightweight design. The small form factor (26.4 mm
x 26.4 mm x 21.6 mm) makes it easy to integrate into tight spaces or
portable systems.</p></li>
<li><p><strong>Low Power Consumption</strong>: The camera is designed to
operate with low power consumption, which is beneficial for portable and
embedded systems where power efficiency is crucial.</p></li>
<li><p><strong>Global Shutter</strong>: The camera is equipped with a
global shutter, which captures the entire image at once, eliminating
motion artifacts and distortions. This is particularly important for
capturing fast-moving objects accurately.</p></li>
<li><p><strong>Image Quality</strong>: The MQ013RG-ON offers good image
quality with low noise and high sensitivity, making it suitable for
various lighting conditions. It also supports multiple image enhancement
features such as gain control, exposure control, and white
balance.</p></li>
<li><p><strong>Software Support</strong>: XIMEA provides comprehensive
software support, including drivers and SDKs for major operating systems
like Windows, Linux, and macOS. The xiAPI SDK facilitates easy camera
integration and control, and supports various programming
languages.<br />
</p></li>
</ol>
<p>The Basler ace line of digital cameras is a popular series of
industrial cameras known for their high performance, reliability, and
versatility in various applications. Basler, a German company, is
well-regarded in the machine vision and digital imaging industry. Here
are some key features and aspects of the Basler ace cameras:</p>
<ol>
<li><p><strong>Resolution and Frame Rate</strong>: The Basler ace
cameras come in a wide range of resolutions, from VGA to several
megapixels, and can achieve high frame rates suitable for fast-moving
applications.</p></li>
<li><p><strong>Sensor Options</strong>: These cameras use high-quality
CMOS and CCD sensors from leading manufacturers like Sony, ON
Semiconductor, and others. The choice of sensors allows for excellent
image quality, sensitivity, and dynamic range.</p></li>
<li><p><strong>Compact Design</strong>: The cameras are designed to be
compact and lightweight, making them easy to integrate into various
systems and applications where space is a constraint.</p></li>
<li><p><strong>Interfaces</strong>: Basler ace cameras support multiple
interface standards, including GigE (Gigabit Ethernet), USB 3.0, and
Camera Link, offering flexibility in connectivity and data transfer
speeds.</p></li>
<li><p><strong>Image Processing</strong>: They come with advanced image
processing features like color correction, gamma correction, and
debayering, which can be performed on the camera, reducing the load on
the host system.</p></li>
<li><p><strong>Software Support</strong>: Basler provides the Pylon
Camera Software Suite, which includes drivers, SDKs, and tools for easy
integration and development. The suite supports multiple platforms and
programming languages.</p></li>
<li><p><strong>Industrial Standards</strong>: The cameras comply with
industry standards like GenICam and GigE Vision, ensuring compatibility
and ease of use with a wide range of third-party software and
systems.</p></li>
<li><p>This is the link to the Basler website: <a
href="https://www.baslerweb.com/en/">Basler</a></p></li>
</ol></li>
<li><p><strong>LabJack</strong> <span id="sec:orgb4af236"
label="sec:orgb4af236"></span></p>
<p>LabJack produces high speed, relatively low cost USB Data Acquisition
(DAQ) interfaces to aid in the construction of computer-based
instrumentation. A LabJack DAQ allows the acquisition of readings from
various sensors/transducers, and the control of different
outputs/actuators. These DAQs are compatible with various
scripting/programming languages, including Python and Matlab. We have
been successfully employing the U series of these DAQs in our labs for
some time. This is the link to the LabJack website: <a
href="https://labjack.com/">LabJack</a></p></li>
</ol>
<h3 id="sec:orgba881e4">Optomechanics, optics and illumination</h3>
<p>Much of what might be needed in assembling a tracking setup entails
the use of mounts and breadboards, in order to fix the components in
place as well as to provide holders for video cameras and for
illumination devices, as well as raised stages for the arena(s) and
digital projection apparatus. In our labs we often refer to Thorlabs as
a source for such material.</p>
<ol>
<li><p><strong>Thorlabs</strong> <span id="sec:orgdd98142"
label="sec:orgdd98142"></span> provides a wide range of hardware
specifically designed for photonics, optics, and related fields. Here’s
an overview of some of the types of hardware they offer:</p>
<ol>
<li><p><strong>Mounting Components</strong>:</p>
<ul>
<li><p><strong>Lens Mounts</strong>: Fixed and adjustable mounts for
lenses of various sizes.</p></li>
<li><p><strong>Mirror Mounts</strong>: Precision mounts for mirrors,
including kinematic and gimbal mounts.</p></li>
</ul></li>
<li><p><strong>Translation and Rotation Stages</strong>:</p>
<ul>
<li><p><strong>Linear Stages</strong>: Manual and motorized stages for
precise linear positioning.</p></li>
<li><p><strong>Rotation Stages</strong>: For angular positioning of
components.</p></li>
<li><p><strong>XY and XYZ Stages</strong>: Multi-axis stages for complex
positioning needs.</p></li>
</ul></li>
<li><p><strong>Optical Tables and Breadboards</strong>:</p>
<ul>
<li><p><strong>Optical Tables</strong>: Vibration-isolated tables for
stable experimental setups.</p></li>
<li><p><strong>Breadboards</strong>: Smaller, portable alternatives for
mounting optical components.</p></li>
</ul></li>
<li><p><strong>Positioning and Adjustment Tools</strong>:</p>
<ul>
<li><p><strong>Micrometers and Actuators</strong>: Precision tools for
fine adjustments.</p></li>
<li><p><strong>Goniometers</strong>: For precise angular
adjustments.</p></li>
</ul></li>
<li><p><strong>Mirrors</strong>:</p>
<ul>
<li><p><strong>Flat Mirrors</strong>: For beam steering and
alignment.</p></li>
<li><p><strong>Curved Mirrors</strong>: For focusing and collimation
applications.</p></li>
</ul></li>
<li><p><strong>Filters</strong>:</p>
<ul>
<li><p><strong>Bandpass Filters</strong>: For specific wavelength
transmission.</p></li>
<li><p><strong>Neutral Density Filters</strong>: For attenuating light
intensity.</p></li>
</ul></li>
<li><p><strong>LEDs</strong>:</p>
<ul>
<li><p><strong>High-Power LEDs</strong>: For bright illumination in
various wavelengths.</p></li>
</ul></li>
</ol>
<p>This is the link to Thorlabs website: <a
href="https://www.thorlabs.com/">Thorlabs</a></p>
<p>Furthermore for optical components, in particular optical filters
(i.e. longpass IR filters), we have made use of components from Edmund
Optics. This company is also a supplier of optomechanics
material.</p></li>
<li><p><strong>Edmund Optics</strong> <span id="sec:orgf5bdff3"
label="sec:orgf5bdff3"></span> is a provider of optical and imaging
components and systems, supplying high-quality optical and optomechanics
components, including lenses, mirrors, filters.</p>
<ol>
<li><p><strong>Optical Components</strong>:</p>
<ul>
<li><p><strong>Lenses</strong>: A wide variety of lenses including
spherical, aspherical, cylindrical, and gradient index lenses.</p></li>
<li><p><strong>Mirrors</strong>: Flat, concave, and convex mirrors with
various coatings for different applications.</p></li>
<li><p><strong>Filters</strong>: Optical filters including bandpass,
longpass, shortpass, and neutral density filters.</p></li>
<li><p><strong>Prisms and Beamsplitters</strong>: Devices for beam
manipulation and splitting, including beam combiners and dichroic
beamsplitters.</p></li>
</ul></li>
<li><p><strong>Imaging and Machine Vision</strong>:</p>
<ul>
<li><p><strong>Imaging Lenses</strong>: High-performance lenses for
cameras and imaging systems.</p></li>
<li><p><strong>Cameras</strong>: Industrial cameras for machine vision,
scientific imaging, and more.</p></li>
<li><p><strong>Illumination</strong>: Light sources and illumination
systems for imaging and vision applications.</p></li>
</ul></li>
<li><p><strong>Optomechanics</strong>:</p>
<ul>
<li><p><strong>Mounts and Holders</strong>: Lens mounts, mirror mounts,
and other holders for optical components.</p></li>
<li><p><strong>Positioning Systems</strong>: Translation stages,
rotation stages, and more for precise positioning of optical
elements.</p></li>
<li><p><strong>Optical Tables and Breadboards</strong>: Stable platforms
for setting up optical experiments and systems.</p></li>
</ul></li>
</ol>
<p>This is the link to the Edmund Optics website: <a
href="https://www.edmundoptics.com/">Edmund Optics</a></p></li>
</ol>
<h3 id="sec:org46764a4">Arenas</h3>
<p>The design and construction of arenas suitable for containing the
animals in a defined space during tracking (perhaps in the presence of
visual stimulation of the individuals) requires the consideration of
some key aspects such as:<br />
</p>
<ul>
<li><p>the material used to construct the arena should be transparent,
in particular the top, which is the part through which the video camera
will be recording the behaviour of the enclosed animals;</p></li>
<li><p>the shape of the arena should be considered carefully, according
to the intentions of the experimenter. In particular, circular shaped
arenas are generally used in order to avoid having corners into which
the animals may tend to find "refuge", which may result in the animals
remaining immobile for most of the experiment time. On the other hand,
circular open spaces may be a source of stress, in particular for single
animals, and this should be kept in due consideration. In this respect,
throughout the years, many other geometries for arenas used to study
particular aspects of <em>Drosophila melanogaster</em> behaviour have
been proposed (see for example, <span class="citation"
data-cites="soibam_modeling_2012">(Soibam et al. 2012)</span> or <span
class="citation" data-cites="tom_mekdara_novel_2012">(Tom Mekdara et al.
2012)</span>).</p></li>
<li><p>In the case of experiments involving insects, such as Drosophila,
the height of the enclosing arena (i.e. floor to ceiling) requires a
careful design in order to restrict the vertical motion of the flies by
not allowing them to fly, but only walk. Also the height should decline
towards the edges of the arena, so that the flies can only adopt an
upright standing position throughout the arena, as described in the
paper by Simon et al. <span class="citation"
data-cites="simon_new_2010">(Simon and Dickinson 2010)</span>.<br />
</p></li>
</ul>
<ol>
<li><p><strong>Construction of fruit fly arenas</strong> <span
id="sec:org2a1a1df" label="sec:org2a1a1df"></span> In our lab we employ
circular arenas of varying diameters, according to the type of
experimental setup employed (i.e. single animal <em>vs</em> multiple
animals) <span class="citation" data-cites="meda_searching_2020">(Meda
et al. 2020)</span>, <span class="citation"
data-cites="meda_heuristic_2022">(Meda et al. 2022)</span>. Such arenas
are made from transparent (or semi-transparent) colourless 3D-printed
resin. The design of the arenas can be done in many ways. One of these
is to employ technical drawing software, such as Inkscape, to produce a
vectorialized profile of the circular arena (i.e. a side view plane)
which can then be "spun" virtually around it’s center to produce a 3D
solid of revolution using software, such as OpenSCAD, which allows to
export the design as a file representing the 3D structure in a format
which can be used to instruct a 3D printer to produce the solid object
represented in the diagram using the desired material (such as
transparent resin). A possible workflow for the design of a circular
arena with the characteristics described in <span class="citation"
data-cites="simon_new_2010">(Simon and Dickinson 2010)</span> would
be:</p>
<ol>
<li><p>Generate the 2D profile by plotting the mathematical function
which describes the profile using an R script (i.e. see the section on
<em>Custom code : R scripts</em>).</p></li>
<li><p>Export the plotted profile image from RStudio as an "svg" type
file. Make sure to choose the option to <strong>not</strong> conserve
the aspect ratio, otherwise the true size of the object will not be
maintained.</p></li>
<li><p>Open the "svg" file with Inkscape.</p></li>
<li><p>Ungroup the imported object to isolate it from the background
which is also imported with the original "svg" image.</p></li>
<li><p>Delete the underlying background and keep the object.</p></li>
<li><p>Put the Inkscape grid into "mm" mode.</p></li>
<li><p>Use the "node tool" and identify the nodes at the extremities of
each of the segments which make up the profile. Select one adjacent node
on either side of adjacent segments and click the "join selected nodes"
button in the toolbar. There are various instructional videos online
showing this procedure.<br />
The profile generated using R, is made up of segments defined by the
"pieces" of the function. The junctions are not apparent in the graph,
but Inkscape will detect these as discontinuities between the segments.
This is why they need to be joined in Inkscape, before submitting the
profile to OpenSCAD in order to produce the 3D solid of revolution. If
you do not do this, the solid produced in OpenSCAD will have very small
holes in it at the points of junction between the profile
segments.<br />
</p></li>
<li><p>Finally, select all the segments and use the "Paths" menu to
combine all the paths into one.</p></li>
<li><p>Now use the "Fill and stroke" menu to make the lines of the
desired thickness (usually would be 1.5-2.0 mm)</p></li>
<li><p>Select the object and move the object to (0,0) coordinates
(Inkscape has 0,0 coordinates in the top lef hand corner, it is better
to move the object to the bottom left hand corner, as OpenSCAD then
reads that as being the (0,0) position in it’s own reference framework.
In Inkscape, on an A4 sheet of paper in portrait mode, this would be at
[0, 292] (not [0, 297], because the object has a size of 5mm, if the
line thickness chosen is 1.5mm and the floor-to-ceiling height of the
arena is 3.5mm).</p></li>
<li><p>Check the size of the object to make sure the dimensions of the
object are as you want them to be (i.e. the radius, thickness, and max.
ceiling height. Correct them if necessary).</p></li>
<li><p>Save the Inkscape object as an "svg" file.</p></li>
<li><p>Open the "svg" file using OpenSCAD. To open the "svg" file open a
"New Document" in OpenSCAD, then use the OpenSCAD console to issue an
"import()" command.</p></li>
<li><p>Translate the position of the object to have the X coordinates at
zero (Actually, for technical reasons, it is better to place the object
at 3D coordinates (x=0.0001, y=0, z=0).</p></li>
<li><p>Use the "<code>rotate_extrude</code>" command to make a 3D
object. Check the figure below representing an example of an arena
produced with the above procedure: the commands described at points 13,
14 and 15, should be issued in the reverse order (i.e. in OpenSCAD,
transformations of a defined object are prepended to (i.e. given before)
the generation of the object. In the figure, the OpenSCAD console is
visible on the left of the 3D object and it shows the commands in the
order in which they should be issued.</p>
<div class="center">
<p><img src="{{ site.url }}{{ 
	site.baseurl}}/assets/images/OpenSCAD_60mm_Arena.png" alt="image" /></p>
</div></li>
<li><p>Save the 3D object as an "stl" file.</p></li>
<li><p>Send to 3D printing service to be printed in the material of
choice. Generally this would be transparent resin.</p></li>
</ol></li>
</ol>
	
