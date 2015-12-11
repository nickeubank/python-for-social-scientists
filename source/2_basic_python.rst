
2. Basic Python
==========================

This site provides a number of links to recommended introduction to Python tutorials (no reason to re-invent the wheel by trying to write a new one!). These different tutorials each have their own strengths and weaknesses, and readers are encouraged to shop around a little. 

Words of Advice
^^^^^^^^^^^^^^^^^^^^^
Before that list, however, some guidance:

Manage your expectations
-------------------------

Python is very user friendly, but it does ask that you invest a little in learning the fundamentals of the language before you jump into applications. Languages like R and Stata were explicitly designed to have you up and running almost immediately, but accomplishing this affected how the languages could be written. Python requires a little training, but pays you back for that investment down the road.

Prioritize
------------

Because Python is a general purpose language, it has many features that definitely won't be relevant for you immediately, and may never be relevant. Many tutorials, for example, were written by people in silicon valley who write apps for phones, and emphasize the skills they use. Here's an overview of the things I think are critical to know immediately, important to learn soon, and things you may never need to know:

Need immediately:

* Data types: integers, floats, strings, booleans, lists, dictionaries, and sets (tuples are kinda optional)
* Defining functions
* Writing loops
* Understanding mutable versus immutable data types
* Methods for manipulating strings
* Importing third party modules

Things you'll want to know at some point, but not necessary immediately:

* Debugging
* File input / output (most libraries you'll use have tools to simplify this for you)

Don't need:

* Defining or writing classes
* Understanding Exceptions


If you try one of these and find my annotations inaccurate, please `send me a note <mailto:nickeubank+pss@gmail.com>`_ letting me know and I'll update my advice!

One last note: in the Python world, the type of work you will probably be doing is called "scientific computing", so if you're trying to find tailored resources, that's a great search term!

Python and iPython
-------------------

At its core, Python has a simple, text-based interactive interface. However, there is also a program called `iPython` many people use when working interactively with Python. `iPython` is just a little program that sits between the user and Python itself that adds a few bells and whistles to make it a little easier to work with. What `iPython` can do is not really important here; what is important is that you not be surprised if you find different tutorials working with slightly different interfaces. (If you see a tutorial with something called `Jupyter` notebooks, that's basically a special document that runs `iPython`).

You can tell if someone is using Python or `iPython` by looking at the prompt on the screen. Python always has a simple three arrow icon (`>>>`). iPython has a more colorful interface that looks like this:

.. ipython:: python

   print('hello!')


Tutorials
^^^^^^^^^^^

`Python 3 Essentials <http://www.lynda.com/Python-3-tutorials/essential-training/62226-2.html>`_ from Lynda.com
-----------------------------------------------------------------------------------------------------------------
**Pre-requisites:** Some experience in another language like R or Java. If you've used for-loops and defined your own functions in another language, you're probably fine. 

**The Good:** A really incredibly clear instructor and carefully designed class. Some assumed familiarity with programming, but not a lot. Lynda.com also offers ability to speed-up playback for sections that feel familiar or straightforward. Topics are carefully organized and indexed if you need to jump around. Includes a "Quick Start" section. 

**The Bad:** May not be free. Lynda.com tutorials are great because it's a paid service, and sadly you sometimes get what you pay for. However, many universities (Yale, Stanford, etc.) have subscriptions, so check with your institution to see if you can get free access. You can also get a 10 day free trial, or pay $30 for a month. If you're unsure, try the "Quick Start" section, which is public. 

**Recommended Sections:** I would recommend proceeding as follows:

* Section 1
* Section 2 up to "Reusing code and data with a class"
* If you installed Python using the setup recommended here, skip section 3. 
* Do Sections 4 - 8, 11, 13, 14, and the first two parts of Section 17

**Optional Sections**: Not immediately needed, but potentially quite useful:

* Section 9

**Other Notes:** About a decade ago Python began a transition from version 2 to version 3 (for reasons that aren't worth getting into, this was a somewhat controversial move, but it's basically done at this point). This was published in part to help with that transition, so if you hear digressions about how Python 3 is different from Python 2, that's why. 


`Python for You and Me <http://pymbook.readthedocs.org/en/latest/>`_
----------------------------------------------------------------------

**Pre-requisites:** If you've done any programming in another language, you should be set. Maybe *just* a little too much assumed knowledge for someone who has never programmed, but I could be wrong on that (I'm very intolerant of assumed knowledge in teaching...). 

**The Good:** If you don't like video tutorials, this is a great choice. Clearly written, moves slowly and incrementally. 

**The Bad:** No explicit exercises to work through. 

**Recommended Sections:** I would recommend proceeding as follows:

* Everything up to but not including "File Handling"
* Modules

**Optional Sections:** Not crucial, but potentially quite helpful: 

* PEP8 Guidelines


**Other Notes:** 


`Automate the Boring Stuff <https://automatetheboringstuff.com/>`_
-------------------------------------------------------------------
**Pre-requisites:** None! Though the name is a little weird, it seems like a great resource for social scientists. 

**The Good:** Seems like a great introduction with essentially no assumed knowledge! The holy grail for absolute beginners. Also includes lectures (links to youtube at top of each section) for those who like it.

**The Bad:** The narrative voice is fun but a little verbose (kinda like this site), so it could feel a little slow for people with more background. 

**Recommended Section:**

* Chapters 0-6

**Optional Sections:** Not crucial, but potentially quite helpful: 

* Chapter 7, Chapter 10




.. `Dive Into Python <http://www.diveinto.org/python3/>`_
.. -----------------------------------------------------------------
.. 
.. Good, but moves relatively quickly for beginners. 
.. 
.. 
.. 
.. `Python the Guide <http://docs.python-guide.org/en/latest/intro/learning/>`_
.. -----------------------------------------------------------------------------
.. A guide to tutorials! 
.. 
.. 
.. 
.. 
.. `Learn Python the Hard Way <http://learnpythonthehardway.org/>`_
.. -----------------------------------------------------------------
.. A very popular and free resource for learning Python. 
.. 
.. **The Bad:** The tutorial is written for Python 2, and the author goes out of his way to say "A programmer may try to get you to install Python 3 and learn that. Say, "When all of the Python code on your computer is Python 3, then I'll try to learn it." That should keep them busy for about 10 years. I repeat, do not use Python 3." The problem is that that decade has basically passed, and all scientific computing software is basically now made the transition to Python 3. 
.. 
.. **Other Notes:** 
