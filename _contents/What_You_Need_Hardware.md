---
title: "15. What you will (or might) need: Hardware"
image: 
  path: /assets/images/Hardware_Hero.jpg
---

<!--- # General concepts --->


## Electronics

1.  <span class="underline">Arduino</span>

      
    Arduino electronic boards are open-source hardware platforms designed
    for creating digital devices and interactive objects that can sense
    and control physical elements. They are popular for their ease of use,
    versatility, and wide range of applications in electronics
    projects. Here are some key characteristics:
    
    1.  **Microcontroller-Based**: Each Arduino board comes with a
        microcontroller (e.g., ATmega328 on the Arduino Uno), which acts as
        the brain of the board, executing programmed instructions.
    2.  **Digital and Analog I/O Pins**: Arduino boards have multiple input
        and output pins that can be used to connect sensors, LEDs, motors,
        and other electronic components.
    3.  **Programming Environment**: Arduino uses a simplified version of
        C/C++ and comes with an integrated development environment (IDE)
        that is user-friendly and easy to learn.
    4.  **USB Connectivity**: Most boards can be connected to a computer
        via USB for programming and power supply.
    5.  **Wide Compatibility**: Arduino is compatible with a vast array of
        sensors, modules, and shields that extend its functionality.
    
    Some typical applications for Arduino boards:
    
    -   **Prototyping**: Rapid development of electronic prototypes.
    -   **Education**: Teaching electronics and programming.
    -   **Robotics**: Controlling robots and automation systems.
    -   **IoT**: Creating Internet of Things devices that can communicate
        over networks.
    -   **DIY Projects**: Building personal projects, such as home
        automation systems, wearable technology, and interactive art.
    
    Other important points of strength of the Arduino project are:
    
    -   **Open Source**: The hardware and software are open-source, allowing
        for customization and community contributions.
    -   **Extensive Documentation**: A wealth of tutorials, forums, and
        examples are available online.
    -   **Libraries**: Numerous libraries are available to simplify the use
        of various sensors and modules.
    
      
    This is the link to the Arduino development
         board, software download and documentation pages: [Arduino](https://store.arduino.cc)

2.  <span class="underline">LED Panels</span>

      
    LED-based panels can efficiently be employed to present visual
    stimuli to model organisms. In 2008, Michael Reiser and Michael
    Dickinson (\cite{reiser_modular_2008}) reported the design of an
    approximately cylindrical modular display system for insect
    behavioral neuroscience. Following that report, the design was
    further updated, and all the technical details for the
    construction of such modular systems were made publicly available
    through the author's Github website [Modular-LED-Display](https://reiserlab.github.io/Modular-LED-Display/). The
    website documents everything required to implement a fully
    functional system, including commercial sources for the LED
    panels, the electronics, the hardware and the software required
    to control them. As of writing, the LED panels used are
    monochromatic (i.e. green LEDs), however this also results in
    very high speed refresh rates (up to 500Hz, with 256 brightness
    levels).

3.  <span class="underline">Ultra-Short-Throw Digital Projectors</span>

      
    UST projectors refer to "Ultra Short Throw" projectors. These are
    specialized projectors designed to project large images from a
    very short distance to the screen or wall. In general, UST
    projectors can project large images(e.g., 250cm, diagonal, or
    more) from just a few centimeters away from the screen or the
    surface on which to project the image. This is achieved through
    advanced lens and mirror systems. Nowdays, such projectors are
    widely available on the consumer market at relatively affordable
    prices, depending on the required quality of the projected image
    (i.e. resolution, brightness and contrast). However, the
    applications envisaged in the specific context being considered
    here, require the projection of high definition, high contrast
    images, having sizes in the range of 25cm (diagonal). The type of
    projectors that have such characteristics are those designed for
    applications requiring the short distance projection of
    relatively small images which can function as user interfaces
    (i.e. touch screen functions on common surfaces, such as walls or
    panels of any material, including glass).  
    Currently we are using projectors from [Texas Instruments](https://www.ti.com/) (Texas
    Instruments, DLP LightCrafter™ Display 4710 EVM Gen2).

4.  <span class="underline">Digital Cameras</span>

      
    When selecting video cameras for video tracking applications,
    certain characteristics are particularly desirable to ensure
    accurate and efficient tracking performance. Here are some key
    attributes to consider:
    
    1.  **High Frame Rate**: High frame rates (60 fps or higher) are
        essential for capturing smooth motion, which is crucial for
        accurately tracking fast-moving objects.
    
    2.  **High Resolution**: High resolution allows for more detailed images,
        which can improve the accuracy of the tracking system.
    
    3.  **Low Latency**: Low latency ensures that the video feed is processed
        in real-time, which is critical for responsive tracking.
    
    4.  **Global Shutter**: Global shutters capture the entire frame at once,
        as opposed to rolling shutters which capture the frame line by
        line.
    
    5.  **High Dynamic Range (HDR)**: HDR capability allows the camera to
        capture details in both very bright and very dark areas of the
        scene.
    
    6.  **Good Low-Light Performance**: Many tracking applications may occur
        in low-light or variable lighting conditions.
    
    7.  **Robust Connectivity**: Fast and reliable data transfer is essential
        for high-performance tracking.
    
    8.  **Software and SDK Support**: Comprehensive software support ensures
        that the camera can be easily integrated into existing systems.
    
    Example Cameras for Video Tracking:
    
    -   **FLIR Blackfly S**: Known for high frame rates, global shutter, and
        high resolution.
    -   **Basler ace**: Offers a range of resolutions and frame rates, and
        is compact and lightweight.
    -   **XIMEA xiQ Series**: Compact design with high frame rates and low
        latency, ideal for embedded systems.
    
    <br />  
    Selecting the right video camera for tracking depends on the specific requirements of your application, such as the speed of the objects being tracked, lighting conditions, and integration needs.
    
    Currently in our labs we use two types of digital cameras:
    
    -   Chameleon3 USB3 digital cameras by FLIR Systems (formerly Point Grey Research). This is the link to [FLIR](https://www.flir.com/).
    -   Ximea digital cameras. This is the link to [XIMEA](https://www.ximea.com/)   

	<br />
	The Chameleon3 USB3 digital cameras, are a line of high-performance, compact digital cameras designed for a variety of applications including industrial inspection, scientific imaging, and machine vision. Here are some key features and details about the Chameleon3 USB3 digital cameras:   
    
    1.  **USB 3.0 Interface**: These cameras utilize the USB 3.0 interface,
        providing high data transfer rates of up to 5 Gbps, which allows
        for faster image capture and transfer.
    
    2.  **High-Quality Sensors**: Chameleon3 cameras are equipped with
        high-quality CMOS and CCD sensors from leading manufacturers like
        Sony and On Semiconductor, offering resolutions ranging from VGA to
        several megapixels.
    
    3.  **Compact and Lightweight Design**: The cameras are designed to be
        compact and lightweight, making them suitable for integration into
        various systems where space is limited.
    
    4.  **Flexible Configuration**: They come with flexible configuration
        options including adjustable frame rates, exposure times, and gain
        settings, allowing customization to suit specific application
        needs.
    
    5.  **Image Quality**: These cameras provide high image quality with
        features like low noise, high dynamic range, and excellent
        sensitivity, making them suitable for capturing detailed and
        accurate images in various lighting conditions.
    
    6.  **Software and SDK Support**: The Chameleon3 cameras are supported
        by FLIR's FlyCapture software and SDK, which provide comprehensive
        tools for camera control, image capture, and image processing. This
        makes it easier for developers to integrate the cameras into their
        applications.
    
    7.  **Versatility**: These cameras are used in a wide range of
        applications including machine vision, robotics, medical imaging,
        microscopy, and scientific research due to their reliable
        performance and versatility.
    
    8.  **Compatibility**: The cameras are compatible with a variety of
        operating systems including Windows, Linux, and macOS, ensuring
        broad usability across different platforms.
    
      
    The XIMEA MQ013RG-ON is a model from XIMEA’s xiQ series of USB3 Vision
    cameras, known for their compact size, high performance, and
    versatility. Here are some key features and details:  
    
    1.  **Sensor**: The MQ013RG-ON uses the ON Semiconductor AR0134 CMOS
        sensor. It is a 1.2-megapixel sensor with a resolution of 1280 x
        960 pixels. The sensor size is 1/3 inch, which is a standard size
        for many industrial and scientific imaging applications.
    
    2.  **Frame Rate**: The camera supports a high frame rate of up to 60
        frames per second (fps) at full resolution. This makes it suitable
        for applications requiring fast image capture, such as high-speed
        industrial inspection or real-time monitoring.
    
    3.  **Interface**: The camera features a USB 3.0 interface, providing
        high data transfer rates up to 5 Gbps. USB 3.0 ensures fast and
        reliable data transmission, making it ideal for high-resolution and
        high-speed imaging applications.
    
    4.  **Compact Design**: The MQ013RG-ON is known for its extremely compact
        and lightweight design. The small form factor (26.4 mm x 26.4 mm x
        21.6 mm) makes it easy to integrate into tight spaces or portable
        systems.
    
    5.  **Low Power Consumption**: The camera is designed to operate with low
        power consumption, which is beneficial for portable and embedded
        systems where power efficiency is crucial.
    
    6.  **Global Shutter**: The camera is equipped with a global shutter,
        which captures the entire image at once, eliminating motion
        artifacts and distortions.
        -   This is particularly important for capturing fast-moving objects
            accurately.
    
    7.  **Image Quality**: The MQ013RG-ON offers good image quality with low
        noise and high sensitivity, making it suitable for various lighting
        conditions. It also supports multiple image enhancement features
        such as gain control, exposure control, and white balance.
    
    8.  **Software Support**: XIMEA provides comprehensive software support,
        including drivers and SDKs for major operating systems like
        Windows, Linux, and macOS. The xiAPI SDK facilitates easy camera
        integration and control, and supports various programming
        languages.  <br />
		<br />
		    
    In addition to the above, the Basler ace line of digital cameras is a popular series of industrial cameras known for their high performance, reliability, and versatility in various applications. Basler, a German company, is well-regarded in the machine vision and digital imaging industry. Here are some key features and aspects of the Basler ace
    cameras:
    
    1.  **Resolution and Frame Rate**: The Basler ace cameras come in a
        wide range of resolutions, from VGA to several megapixels, and can
        achieve high frame rates suitable for fast-moving applications.
    
    2.  **Sensor Options**: These cameras use high-quality CMOS and CCD
        sensors from leading manufacturers like Sony, ON Semiconductor, and
        others. The choice of sensors allows for excellent image quality,
        sensitivity, and dynamic range.
    
    3.  **Compact Design**: The cameras are designed to be compact and
        lightweight, making them easy to integrate into various systems and
        applications where space is a constraint.
    
    4.  **Interfaces**: Basler ace cameras support multiple interface
        standards, including GigE (Gigabit Ethernet), USB 3.0, and Camera
        Link, offering flexibility in connectivity and data transfer
        speeds.
    
    5.  **Image Processing**: They come with advanced image processing
        features like color correction, gamma correction, and debayering,
        which can be performed on the camera, reducing the load on the host
        system.
    
    6.  **Software Support**: Basler provides the Pylon Camera Software
        Suite, which includes drivers, SDKs, and tools for easy integration
        and development. The suite supports multiple platforms and
        programming languages.
    
    7.  **Industrial Standards**: The cameras comply with industry
        standards like GenICam and GigE Vision, ensuring compatibility and
        ease of use with a wide range of third-party software and systems.
    
    8.  This is the link to the Basler website: [Basler](https://www.baslerweb.com/en/)

## Optomechanics, optics and illumination

Much of what might be needed in assembling a tracking setup entails the use of mounts and breadboards, in order to fix the components in place as well as to provide holders for video
cameras and for illumination devices, as well as raised stages for the arena(s) and digital projection apparatus. In our labs we often refer to Thorlabs as a source for such material.

1.  **Thorlabs** provides a wide range of hardware specifically designed for
    photonics, optics, and related fields. Here's an overview of some
    of the types of hardware they offer:
    
    1.  **Mounting Components**:
        -   **Lens Mounts**: Fixed and adjustable mounts for lenses of
            various sizes.
        -   **Mirror Mounts**: Precision mounts for mirrors, including
            kinematic and gimbal mounts.
    
    2.  **Translation and Rotation Stages**:
        -   **Linear Stages**: Manual and motorized stages for precise linear
            positioning.
        -   **Rotation Stages**: For angular positioning of components.
        -   **XY and XYZ Stages**: Multi-axis stages for complex positioning
            needs.
    
    3.  **Optical Tables and Breadboards**:
        -   **Optical Tables**: Vibration-isolated tables for stable
            experimental setups.
        -   **Breadboards**: Smaller, portable alternatives for mounting
            optical components.
    
    4.  **Positioning and Adjustment Tools**:
        -   **Micrometers and Actuators**: Precision tools for fine
            adjustments.
        -   **Goniometers**: For precise angular adjustments.
    
    5.  **Mirrors**:
        -   **Flat Mirrors**: For beam steering and alignment.
        -   **Curved Mirrors**: For focusing and collimation applications.
    
    6.  **Filters**:
        -   **Bandpass Filters**: For specific wavelength transmission.
        -   **Neutral Density Filters**: For attenuating light intensity.
    
    7.  **LEDs**:
        -   **High-Power LEDs**: For bright illumination in various
            wavelengths.
    
    This is the link to Thorlabs website: [Thorlabs](https://www.thorlabs.com/)
    
    Furthermore for optical components, in particular optical filters
    (i.e. longpass IR filters), we have made use of components from Edmund
    Optics. This company is also a supplier of optomechanics material.

2.  **Edmund Optics** is a provider of optical and imaging components and systems,
    supplying high-quality optical and optomechanics components, including
    lenses, mirrors, filters.
    
    1.  **Optical Components**:
        -   **Lenses**: A wide variety of lenses including spherical,
            aspherical, cylindrical, and gradient index lenses.
        -   **Mirrors**: Flat, concave, and convex mirrors with various
            coatings for different applications.
        -   **Filters**: Optical filters including bandpass, longpass,
            shortpass, and neutral density filters.
        -   **Prisms and Beamsplitters**: Devices for beam manipulation and
            splitting, including beam combiners and dichroic beamsplitters.
    
    2.  **Imaging and Machine Vision**:
        -   **Imaging Lenses**: High-performance lenses for cameras and
            imaging systems.
        -   **Cameras**: Industrial cameras for machine vision, scientific
            imaging, and more.
        -   **Illumination**: Light sources and illumination systems for
            imaging and vision applications.
    
    3.  **Optomechanics**:
        -   **Mounts and Holders**: Lens mounts, mirror mounts, and other
            holders for optical components.
        -   **Positioning Systems**: Translation stages, rotation stages, and
            more for precise positioning of optical elements.
        -   **Optical Tables and Breadboards**: Stable platforms for setting
            up optical experiments and systems.
    
    This is the link to Edmund Optics website: [Edmund Optics](https://www.edmundoptics.com/)

### Arenas

The design and construction of arenas suitable for containing the
animals in a defined space during tracking (perhaps in the
presence of visual stimulation of the individuals) requires the
consideration of some key aspects such as:  

-   the material used to construct the arena should be transparent,
    in particular the top, which is the part through which the video
    camera will be recording the behaviour of the enclosed animals;
-   the shape of the arena should be considered carefully, according
    to the intentions of the experimenter. In particular, circular
    shaped arenas are generally used in order to avoid having
    corners into which the animals may tend to find "refuge", which
    may result in the animals remaining immobile for most of the
    experiment time. On the other hand, circular open spaces may be
    a source of stress, in particular for single animals, and this
    should be kept in due consideration. In this respect, throughout
    the years, many other geometries for arenas used to study
    particular aspects of *Drosophila melanogaster* behaviour have
    been proposed (see for example, \cite{soibam_modeling_2012} or
    \cite{tom_mekdara_novel_2012}).
-   In the case of experiments involving insects, such as
    Drosophila, the height of the enclosing arena (i.e. floor to
    ceiling) requires a careful design in order to restrict the
    vertical motion of the flies by not allowing them to fly, but
    only walk. Also the height should decline towards the edges of
    the arena, so that the flies can only adopt an upright standing
    position throughout the arena, as described in the paper by
    Simon et al. (\cite{simon_new_2010}).

1.  <span class="underline">Construction of fruit fly arenas</span>

    In our lab we employ circular arenas of varying diameters,
    according to the type of experimental setup employed (i.e. single
    animal *vs* multiple animals)(\cite{meda_searching_2020},
    \cite{meda_heuristic_2022}). Such arenas are made from
    transparent (or semi-transparent) colourless 3D-printed resin.
    The design of the arenas can be done in many ways. One of these
    is to employ technical drawing software, such as Inkscape, to
    produce a vectorialized profile of the circular arena (i.e. a
    side view plane) which can then be "spun" virtually around it's
    center to produce a 3D solid of revolution using software, such
    as OpenSCAD, which allows to export the design as a file
    representing the 3D structure in a format which can be used to
    instruct a 3D printer to produce the solid object represented in
    the diagram using the desired material (such as transparent
    resin).
    A possible workflow for the design of a circular arena with the
    characteristics described in \cite{simon_new_2010} would be:
    
    1.  Generate the 2D profile by plotting the mathematical function
        which describes the profile using an R script (i.e. using
        RStudio).
    2.  Export the plotted profile image from RStudio as an "svg" type
        file. Make sure to choose the option to **not** conserve the
        aspect ratio, otherwise the true size of the object will not
        be maintained.
    3.  Open the "svg" file with Inkscape.
    4.  Ungroup the imported object to isolate it from the background
        which is also imported with the original "svg" image.
    5.  Delete the underlying background and keep the object.
    6.  Put the Inkscape grid into "mm" mode.
    7.  Use the "node tool" and identify the nodes at the extremities
        of each of the segments which make up the profile. Select one
        adjacent node on either side of adjacent segments and click
        the "join selected nodes" button in the toolbar. There are
        various instructional videos online showing this procedure.
    8.  Finally, select all the segments and use the "Paths" menu to
        combine all the paths into one.
    9.  Now use the "Fill and stroke" menu to make the lines of the
        desired thickness (usually would be 1.5-2.0 mm)
    10. Select the object and move the object to (0,0) coordinates
        (Inkscape has 0,0 coordinates in the top lef hand corner, it
        is better to move the object to the bottom left hand corner,
        as OpenSCAD then reads that as being the (0,0) position in
        it's own reference framework. In Inkscape, on an A4 sheet of
        paper in portrait mode, this would be at [0, 292] (not [0,
        297], because the object has a size of 5mm, if the line
        thickness chosen is 1.5mm and the floor-to-ceiling height of
        the arena is 3.5mm).
    11. Check the size of the object to make sure the dimensions of
        the object are as you want them to be (i.e. the radius,
        thickness, and max. ceiling height. Correct them if
        necessary).
    12. Save the Inkscape object as an "svg" file.
    13. Open the "svg" file using OpenSCAD. To open the "svg" file
        open a "New Document" in OpenSCAD, then use the OpenSCAD
        console to issue an "import()" command.
    14. Translate the position of the object to have the X
        coordinates at zero (Actually, for technical reasons, it is
        better to place the object at 3D coordinates (x=0.0001, y=0, z=0).
    15. Use the "`rotate_extrude`" command to make a 3D object. Check
        the figure below representing an example of an arena produced
        with the above procedure: the commands described at points
        13, 14 and 15, should be issued in the reverse order (i.e. in
        OpenSCAD, transformations of a defined object are prepended
        to (i.e. given before) the generation of the object. In the
        figure, the OpenSCAD console is visible on the left of the 3D
        object and it shows the commands in the order in which they
        should be issued.
		![image-center]({{ site.url }}{{ site.baseurl}}/assets/images/OpenSCAD_60mm_Arena.png)
    16. Save the 3D object as an "stl" file.
    17. Send to 3D printing service to be printed in the material of
        choice. Generally this would be transparent resin.