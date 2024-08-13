---
title: "40. Custom Code: Python Scripts"
image: 
  path: /assets/images/Custom_code_Python_Hero.png
---

<!--- # General concepts --->


The Python scripts described here can be found in this Github
Repository: [Python
Scripts](https://github.com/em-a-zed/Custom-Tracking-Code/tree/main/Python)

### Some tips for Python users

Python is an open source, cross-platform and relatively easy programming
language to learn and use.

-   An excellent place to start if you have little or even no previous
    experience with Python is this: [Real
    Python](https://realpython.com/), or also this: [The Hitchiker's
    Guide to Python](https://docs.python-guide.org/)

-   You can download the latest Python version for your operating system
    here: [Python](https://www.python.org/). However, before downloading
    and installing a Python version for your operating system, read the
    rest of this.

-   The typical Python working environment consists in the Python
    \"engine\" itself as well as a number of functional additions
    (libraries and packages, i.e. such as [Numpy](https://numpy.org/)
    and [Scipy](https://scipy.org/)) which expand the basic capabilities
    of Python. This can be the source of a relatively common problem: a
    specific piece of software written in Python, may have been written
    using a specific release (version) of Python at a certain point in
    time. That piece of software may also rely on a set of add on
    libraries and/or packages that were tailored to run under the
    specific release of Python used when the software was originally
    written. So, in a nutshell, every piece of software will generally
    run using the release of Python which was used to write it (with the
    same versions of libraries and add on packages which were compatible
    with that specific release of Python).

-   In essence, what happens is that, as computer operating systems (OS)
    evolve, so do the versions of Python that best take advantage of the
    features of these new OS, although new OS generally show a rather
    good backward compatibility with older versions of Python. The newer
    releases of Python may also see changes in some aspects of the
    functionality of the Python language itself. So, what might happen,
    some time after having written a certain piece of software based on
    Python, is that the software loses compatibility with the newer
    versions of Python. The newer versions of Python may also lose some
    compatibility with the libraries and add on packages originally used
    to develop the software and these libraries and packages may in turn
    show changes to accomodate this.

-   Fortunately, this is generally not an unsurmountable issue.
    Different releases of Python can be present (and be used) on the
    same machine. The only problem this raises is that of keeing things
    \"in order\", i.e. keeping the software developed using specific
    versions of Python, separate from other software developed with
    different versions of Python. In addition, each piece of software
    will not only make reference to a specific version of Python, but
    also to the specific versions of the associated libraries and add on
    packages. All of this can be dealt with by using Package Managers.
    Package managers allow the user to generate isolated environments on
    a computer's hard disk (i.e special kinds of directories) within
    which only a specific release of Python and the associated libraries
    and add on packages is used.

-   There are distributions of Python available which are already
    pre-packaged into a user-friendly bundle (i.e. they contain the
    Python programming language itself as well as a certain number of
    packages, libraries and tools).

-   One such distribution is [Anaconda](https://www.anaconda.com/),
    which provides an easy-to-use platform for data science and machine
    learning. It comes with a number of pre-installed packages and tools
    typically employed by programmers working in these fields. Anaconda
    also has a package manager that makes it easy to install and manage
    dependencies and packages. This is the wiki page about Anaconda
    ("Anaconda (Python Distribution)" 2024).

-   Anaconda provides the Conda package management tool that can install
    packages provided by Anaconda on their own
    [Repository](https://repo.anaconda.com/repository). This is a very
    popular repository, especially for data scientists, simplifying the
    creation and management of environments and the installation of
    packages in them. One drawback compared to manual package management
    is that the package selection is more limited.

-   To manage things manually you will need to:

    a.  Use a manager to download and set different Python versions.\
        **Pyenv** is a just such a tool. With it, it is possible to
        install several Python versions; set or change the global(i.e.
        default) Python version in your computer; set or change a Python
        version locally for a specific project.

    b.  Use the Python package manager **pip**. This tool allows to
        install the libraries and add on packages which may be required
        for a specific project. If you have activated a new virtual
        environment, the use of *pip* within the environment (i.e.
        dedicated directory) will install the add on packages only in
        the virtual environment/directory. The advantage of this is that
        all the other environments remain untouched and also the global
        environment remains untouched.

    c.  Use the Python tool **venv**, (or you can also use a similar
        tool called **virtualenv**) which allows the definition and
        activation of virtual environments.

For further details on the preceding 3 points see, for example, also:
[The Hitchikers Guide to
Python](https://docs.python-guide.org/starting/installation/)
<br />

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