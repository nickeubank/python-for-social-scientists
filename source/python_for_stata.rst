
Note to Stata Users
============================

Welcome Stata users! 

There's good news and bad news for you Stata users (of whom I am definitely one -- I spent 6 years working exclusively in Stata). The goods news is that you have no bad habits developed from R, and you're about to enter a world of phenomenal flexibility and power. 

The main thing to keep in mind during your transition to Python is that there will be things in Python that will frustrate you. The beauty of Stata is that it does one thing, and one thing only: manipulate tabular data-sets. As a result of this narrow focus, Stata is able to develop a very clean, simple, intuitive syntax for that specific application. 

The advantage Python has over Stata is that is can do all sorts of things Stata never could -- network analysis, geo-spatial analysis, web-scraping, text analysis, etc. But the downside is that a side-effect of this flexibility is that Python syntax will feel more cumbersome. That's just a compromise you'll have to decide you can live with if you want to work with Python -- sorry!


Sense of Perspective
^^^^^^^^^^^^^^^^^^^^

Everything you know from Stata is inside a single DataFrame object in Python. Think of it as "zooming out". 


Macros
^^^^^^^^^^^^^

If you're someone who is used to working with macros (using the `local` or `global` commands) -- either directly or in for-loops -- you have both an advantage and disadvantage moving into Python. On the plus side, you've been introduced to the idea of generalizing your code, which is great. But on the negative, you've gotten used to a way of using variables that's pretty unique to Stata. 

In Stata, macros work by replacing part of a command before that command is executed. For example, if I write::

   local controls "age age2 education"
   reg income gender `controls'

Then what happens is, before running the second line of that code, it replace `\`controls\'` with the string "age age2 education", then executes the code (`reg income gender age age2 education`). In other words, the macro evaluation happens before the command is passed to Stata. 

Unfortunately, almost no other programming language works this way. You'll see quickly how variables work in Python, but just don't be surprised when you find your intuition from macros failing you. 