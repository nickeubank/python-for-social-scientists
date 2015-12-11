
3. Pandas
=============================

Python itself does not include vectors, matrices, or dataframes as fundamental data types. As Python became an increasingly popular language, however, it was quickly realized that this was a major short-coming, and new libraries were created that added these data-types (and did so in a very, very high performance manner) to Python.

The original library that added vectors and matrices to Python was called `numpy`. But `numpy`, while very powerful, was a no-frills library. You couldn't do things like mix data-types, label your columns, etc.. To remedy this shortcoming a new library was created -- built on top of `numpy` -- that added all the nice features we've come to expect from modern languages: `pandas`. 


Advice
^^^^^^^^^^^

Many things about `pandas` will seem familiar to users of other languages like Matlab, R, or Stata, and most differences are relatively obvious. However, there are two things I think most tutorials under-emphasize I want to alert you to: 

* **Indices:** Most languages (like R, Matlab, and Stata) organize data based on it's order. In R, for example, if you `cbind` two vectors, they attached to one another based on the order of rows. 

In `pandas`, every row of a DataFrame has a name (an index label), and most things in `pandas` are designed to keep careful track of those index labels, and where possible to make sure that when different objects are combined, they are always `aligned` according to those indices. 

* **Changes:** As of late 2015, `pandas` was in version 0.18. Until Version 1, `pandas` developers are likely to feel relatively free to make changes to some core functions in `pandas` to improve the language. For example, in mid-2015, the `sort` function was changed to help make the behavior more intuitive. 

So you're aware of changes, I strongly recommend subscribing to the `pydata Google Group Mailing List <https://groups.google.com/forum/#!forum/pydata>`_ so when updates to `pandas` come out you'll be alerted and get a summary of changes. 

Tutorials
^^^^^^^^^^^

`Intro to Pandas (Greg Reda) <http://www.gregreda.com/2013/10/26/intro-to-pandas-data-structures/>`_
---------------------------------------------------------------------------------------------------------------------------------

**Format:** Text / iPython Notebooks

**Summary:** A really nice, text-based tutorial. Very good for basics. 

`Pandas from the Ground Up (Brandon Rhodes) <https://www.youtube.com/watch?v=5JnMutdy6Fw>`_
---------------------------------------------------------------------------------------------------------------------------------

**Format:** Video, with linked iPython notebooks

**Summary:** One of two very good video introductions to `pandas` (the other is the Jonathan Rocher video below). I suggest watching a little of both of these and picking the one that suits your learning style. This tutorial is a little more "let's learn the principles of Pandas in the abstract then apply them", while the Rocher tutorial is a little more "let's learn as we do", but mix principles and examples well depending on your learning style. 

`Make sure you download the associated materials here, not from the link in the video! <https://github.com/brandon-rhodes/pycon-pandas-tutorial>`_

`Analyzing and Manipulating Data with Pandas (Jonathan Rocher) <https://www.youtube.com/watch?v=0CFFTJUZ2dc>`_
---------------------------------------------------------------------------------------------------------------------------------

**Format:** Video, with linked iPython notebooks

**Summary:** The second very good video introductions to `pandas`. Again, I suggest watching a little of both of these and picking the one that suits your learning style.

`Make sure you download the associated materials here! <https://github.com/jonathanrocher/pandas_tutorial>`_

`Learn Pandas <https://bitbucket.org/hrojas/learn-pandas>`_
---------------------------------------------------------------------------------------------------------------------------------

**Format:** Text / iPython Notebooks

**Summary:** Nice. A little dense, and a little more focused on getting users going than teaching basic organizing principles, but if you want to get to useable code fast, a good option. 

