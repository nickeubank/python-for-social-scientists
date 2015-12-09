
Network Analysis
=============================

Just use `iGraph <http://igraph.org/python>`_. 

If you're doing community detection, make sure to get the `louvain-igraph` module that adds the most cutting edge algorithms to `iGraph`. `You can get it here. <http://www.traag.net/code/>`_

`NetworkX` is the other big network analysis library, but it's *much* slower than `iGraph`. The reason is that `iGraph` is written in C, so it's orders of magnitudes faster than `NetworkX`, which is entirely written in native Python (much, much slower). For small graphs, `NetworkX` is fine, but for moderate sized networks (10,000 nodes or more) you really want to use `iGraph`. 

If you get stuck working with `iGraph`, `the mailing list community <https://lists.nongnu.org/mailman/listinfo/igraph-help>`_ is *amazingly* helpful and supportive. 