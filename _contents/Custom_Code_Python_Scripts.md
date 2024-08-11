---
title: "40. Custom Code: Python Scripts"
image: 
  path: /assets/images/Custom_code_Python_Hero.png
---

<!--- # General concepts --->


The Python scripts described here can be found in this Github
Repository: [Python
Scripts](https://github.com/em-a-zed/Custom-Tracking-Code/tree/main/Python)

### Script to track a freely moving individual

Although this script is relatively basic, it is nonetheless a fully
functional version of a tracker which can easily live-track a single,
freely moving individual. In it's simplicity the script allows to easily
understand how the various parts of the program work. It is also fairly
well commented, so this should further facilitate the comprehension of
its logic.\
The script allows to monitor the tracked individual live, as well as
optionally allowing the plotting of tracking data (also live).
Furthermore the script also implements the *Pyschopy* library, allowing
the user to define the type of visual pattern to present to the tracked
individual (on a separate window and/or screen). In addition, the
projected pattern(s) are programmed to respond, in closed-loop form, to
specific movements of the tracked individual.\
Finally, the script also uses the *Pandas* library to allow the
organization of the collected tracking data as a dataframe, which
greatly facilitates saving the collected data into a text file, which
can then be easily accessed and analyzed using Python scripts,
spreadsheet software, R scripts etc.\
As in the case of the Matlab script for tracking a single tethered
individual (see the Matlab code section), this tracking algorithm also
employs a strategy, based on the approximation of the object to be
tracked by an ellipsoid. In this case, the movements of the object can
be monitored by tracking the center of mass of the ellipse as well as
the rotations of the longitudinal axis of the ellipse in order to obtain
information on the object's instantantaneous orientation. This approach
was described by Raphael Candelier and further details can be found
here: [Candelier](https://raphael.candelier.fr/?blog=Image%20Moments).\
The algorithm to perform this type of tracking was provided by Raphael
Candelier in the form of a Matlab script, which I then \"translated\"
into Python language.
