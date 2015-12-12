
Plotting
=====================

The low-level library for making figures in Python is called `matplotlib`. It's very powerful, but also a little *too* low-level for most social science uses, so it's probably not your best bet. Instead, most people use either `seaborn`, or `ggplot` (meant to duplicate syntax and functionality of `ggplot` in R).

ggplot
^^^^^^^^^^^^^^^^^^^^^

If you're accustomed to using `ggplot` in R, then good news: the folks at yhat have duplicated it's functionality in Python! 

* `ggplot Overview <http://ggplot.yhathq.com/how-it-works.html>`_
* `Installation <http://ggplot.yhathq.com/install.html>`_

seaborn
^^^^^^^^^^^^^^^^^^^^^

The other very popular library for plotting is called `seaborn`. It's build on top of `matplotlib`, and basically allows you to make common statistical plots more easily. If you come from stata, think of `seaborn` as your `twoway`; if you come from `R`, it's your `ggplot`. 

* `Main page <http://stanford.edu/~mwaskom/software/seaborn/>`_
* `Gallery of example plots (with the code that made them) <http://stanford.edu/~mwaskom/software/seaborn/examples/index.html>`_
* `Introduction to seaborn <http://stanford.edu/~mwaskom/software/seaborn/introduction.html>`_
* `Tutorial <https://stanford.edu/~mwaskom/software/seaborn/tutorial/distributions.html>`_. (Note this is not the default tutorial on the `seaborn` site, but another one that's hidden away I actually much prefer!)

At the time of this is being written, `seaborn` did not come with Anaconda by default, but can be easily added by typing `conda install seaborn` in your terminal window.

