
1. Setting Up Python
==============================



Installing Python
^^^^^^^^^^^^^^^^^

First, we want to download the Anaconda Python distribution. The Anaconda distribution is not the only way to get python -- indeed, there's a good chance a version of Python is already installed on your computer -- but the Anaconda installation does a number of very nice things:

* A clean installation of the latest version of Python
* Installation of a large number of add-on libraries that are commonly used in scientific computing (this is what the type of work social scientists do is called)
* Installation of a "package manager" -- a tool for installing new packages in the future and updating already installed packages. [#pip]_

To install the Anaconda distribution, just go to the `Anaconda download page <https://www.continuum.io/downloads>`_ and pick the appropriate installer. **Make sure to get an installer for Python 3.x, not 2.x**! [#2v3]_


Running Python
^^^^^^^^^^^^^^

Once you have python, you have to decide how to interact with it. Anaconda includes a "Launcher" app that offers several options (which you can find in the "anaconda" folder, though there's probably a shortcut on your desktop after installation), but I would suggest using the program Spyder to work with Python -- it's probably the most familiar interface to Stata and R users, as it is analogous to Stata / RStudio. 



.. [#pip] If you know what pip is, Anaconda is similar to pip, but with the added ability of being able to not just load python modules, but also compile the C or C++ code that underlies some fancier libraries. 
.. [#2v3] In 2000, Python 3 was first released. Python 3 fixed a lot of things people disliked about Python, but in the process it made some changes that meant code written in Python 2 would not work any more. To ease the transition to Python 3, both Python 2 and Python 3 have been supported for several years so people could keep running their Python 2 until they finished the transition. Almost everything is now in Python 3, so since you don't have any old code to worry about, you want Python 3.