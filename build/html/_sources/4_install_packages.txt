
4. Installing Packages
==========================

There are three tools for adding modules to your python installation: `conda`, `anaconda`, and `pip`.

`pip` is the oldest tool, and works for most things. `conda` is the newest, and is great because it can handle libraries that `pip` struggles with (libraries that require compilation, as many scientific libraries do) and is curated and managed by the Continuum Analytics. And finally, anaconda.org is a user-contributed version of `conda` -- same engine, but the specific packages are managed by users on Anaconda.org, so results aren't quite as well guaranteed, but many things are available that aren't on `conda`. You access it by typing `conda -c` instead of `conda`/

**An important note:** Unlike in R or Stata, you don't download and install Python libraries from inside Python. Instead, you invoke `pip`, `conda`, or `anaconda` from the "command line" -- a text-based interface for your operating system. The command line is found in the `terminal` application (on a mac) or `PowerShell` application (on Windows), and you may also hear it referred to as `bash`. The command line may seem scary, but you literally just need to open `terminal` (on a mac, it's in Applications/Utilities) or PowerShell and type `conda install [library]` or `pip install [library]`.

Generally, I would attempt to load libraries as follows:

* Try `conda install [library]` 
* Try `pip install [library]`
* Use `conda -c install [library]`

Here are tutorials for each:

* `conda and anaconda <http://conda.pydata.org/docs/using/pkgs.html>`_ (ignore all the stuff about "environments" -- not relevant at this stage!)
* `pip <http://python-packaging-user-guide.readthedocs.org/en/latest/installing/#use-pip-for-installing>`_ Note pip is included in the Anaconda distribution, so you can ignore all the stuff about setting up pip in the guide above the "Use pip for installing" entry, and you don't need to worry about anything below "Upgrading packages".


