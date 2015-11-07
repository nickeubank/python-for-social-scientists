
Python Intro for R Users!
=========================

Here's some python for R user advice!

Key Concepts: References
========================

Before you dive into general-purpose tutorials on Python syntax, there's one large conceptual change you should be aware of coming from R. 

Say you make a new vector as follows:

``my.list <- list(1,2,3)``

In R, there's no difference between a variable (like ``my.list``) and the object (the list 1, 2, 3) associated with it. But this is actually a slight of hand used by R to hide something fundamental about how computers work, and it does not happen in Python.

In Python, when you create an object like a `list`, Python puts that list somewhere in memory, kind of like you might put something big on a shelf somewhere in a warehouse. The variable associated with that `list` (``my.list``) is not the same as that list -- it actually just stores the location on the shelves where you placed that list. 

The reason this matters is that it's possible for multiple variables to be pointed at the same item on a shelf, which means if you do something to one variable, it changes the item on the shelf, and so if you call the other variable that points to that item on a shelf, you will find the change affected both items. For example:

.. ipython:: python

    # Make a new list
    x = ['Adriane', 'and', 'Nick', 'got', 'engaged!']
    # Make new var Y, and assign it x. In R this would make a copy. 
    y = x 
    # Add to the end of the string
    x.append(" no, seriously guys. We're engaged. Not kidding.")
    # We see this new addition is now at end of x
    x
   
    # But look! It's also at the end of y! 
    # That's because they both point at the same list on the shelf. 
    y
   

Weird, right?
