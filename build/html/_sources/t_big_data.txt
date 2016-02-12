
Big Data / Parallelization
=============================

What *Is* Big Data?
^^^^^^^^^^^^^^^^^^^^
Excellent question! The truth is the term has a different meaning to different people. Within Political Science, for example, the term is often used for any project that studies correlations in relatively large datasets. On this site, however, we will use a more precise and practical definition of two types of *big data*: 

* **Big Data**: data that is too big to load and work with entirely in RAM
    + hundreds of gigabytes of data to a few terabytes of data
* **Very Big Data**: data that is too big to load and work with entirely in RAM, and also too big to store on a single computer's hard drive.
    + peta-bytes of data

Note this distinction is my own -- when you go into the world, you will find big data sometimes means using unusually large datasets, sometimes means data that doesn't fit into ram, and sometimes means data that won't fit on a single computer's harddrive. 

Further, also note that programs very often make copies of data when you work, so if your data just barely fits into RAM (say your data is 7gb and you have 10gb of RAM), then you may be working with *Big Data*!

Why this definition? When your computer is manipulating data (defining variables, running regressions, etc), what its actually doing is grabbing a little bit of data from storage, moving it to the processor, doing math with it, and then putting it back in storage. 

To simplify somewhat, we can think of your computer as having two forms of storage -- RAM (sometimes called main memory), and your harddrive. But these two forms of memory are ''very, very different.'' Your computer can grab data from RAM 100,000 times faster it can grab data on the harddrive. Because of this, your computer is much happier (and performs faster) when it's able to keep all the data you're working with in RAM. Indeed, if you're moving data back and forth to your harddrive, it's almost certainly the biggest bottleneck -- doing actual computations is almost instantaneous compared to moving data back and forth to your harddrive on modern computers. 

With that in mind, if you can't keep all your data in RAM, you have to use special tools that minimize the amount of time your computer spends going back and forth to the harddrive for data. 


Big Data Tools
^^^^^^^^^^^^^^^

Easy to work with, but somewhat limited: `dask`
------------------------------------------------

`Dask` is a new tool written for working with data that doesn't fit into memory (and parallelizing operations) for Python. It was written to basically work just like `pandas`, so it's quite easy to get started using. The only catch is that it only supports a certain number of functions at this point, so it will do a lot, but not everything.

* `Dask Overview <https://www.youtube.com/watch?v=1kkFZ4P-XHg>`_
* `Long Tutorial <https://www.youtube.com/watch?v=ieW3G7ZzRZ0>`_

Dask is probably best for *big data*, but I'm not sure it can really handle *very big data* (data you can't put on one computer's harddrive). The authors aim to fix that, but I'm not sure the system is there yet. 

More involved, but more powerful: `pyspark`
---------------------------------------------

`Spark` is like the second generation of a platform called Hadoop for working with data across lots and lots of software. `pyspark` is a great tool for manipulating `spark` using python. `spark` is *very* powerful, but it's not a tool created for Python users, it's an entire computing system you'll have to learn about to use. 

Though there are attempts to make `PySpark` easier for `pandas` users to use, like `Sparkling Pandas` (`tutorial here <https://www.youtube.com/watch?v=borv_KMI9Ac>`_)

Unlike `Dask`, `Spark` and `PySpark` were built not just for *big data* (data that doesn't fit in RAM), but specifically for *very big data* (data that won't even fit on a single computer's hard drive). So if you have *very big data*, this is probably the way to go. 


