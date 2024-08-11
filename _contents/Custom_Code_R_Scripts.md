---
title: "30. Custom Code: R Scripts"
image: 
  path: /assets/images/Custom_code_R_Hero.png
---


<!--- # General concepts --->

The R scripts described here can be found in this Github Repository:
[R_Scripts](https://github.com/em-a-zed/Custom-Tracking-Code/tree/main/R)
### Script to generate circular arena profile

The following is an R script which defines a function (called
\"Arena\"). The function is based upon the piece function as defined in
(Simon and Dickinson 2010). The function will generate the profile of an
arena (actually half of an arena) having a floor-to-ceiling height of
3.5mm and a radius of 30mm. The generated profile is made up of segments
defined by the \"pieces\" of the function. The junctions are not
apparent in the graph, but Inkscape will detect these as discontinuities
between the segments. This is why they need to be joined in Inkscape,
before submitting the profile to OpenSCAD in order to produce the 3D
solid of revolution. If you do not do this, the solid produced in
OpenSCAD will have very small holes in it at the points of junction
between the profile segments.

      Arena <- function(h=3.5,  radius=30){
      h <- 3.5 ##millimeters (height of arena from floor to ceiling)

      ####WITH THIS DESIGN THE ARENA CANNOT HAVE A RADIUS
      ####LESS THAN 30 mm....
      radius <- 30 ## arena radius in millimeters
      #################

      theta <- 11*pi/180  ## slope of vertical wall of arena 
      ##11 degrees converted to radians 
      I = h*pi/(4*tan(theta))
      Xmax <- h/(2*tan(theta)) + I

      #Straw commented on typos in the orginal  equations!
      # x = h/(2*tan(theta)) + I

      x <- seq(0, 2*I, 0.1)

      x1 <- x[which(x>=0 & x<=I)]
      y1 <- h*(1-cos((pi*x1)/(2*I)))/2

      ##For i<x<=Xmax
      x2 <- x[which(x>=I & x<=Xmax)]
      y2 <- tan(theta)*(x2-I) + (h/2)

      plot(x1, y1, type='n', xlim=c(0, radius), ylim=c(0, radius + 10),
           axes=FALSE, xlab="", ylab="")

      segments(0, 0, (radius-Xmax), 0, lwd=3)

      lines(x1+radius-Xmax, y1, lwd=3)

      lines(x2+radius-Xmax, y2, lwd=3)

      #Upright segment at the edge of the arena
      segments(radius, tan(theta)*(Xmax-I) + (h/2), radius, 0, lwd=3)

      mtext(paste("radius=", radius, " ", "h=", h))
    }