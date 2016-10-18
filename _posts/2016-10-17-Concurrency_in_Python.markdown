---
layout: post
title:  Exploring concurrency in Python
date:   2016-10-17 22:27:30 -0700
categories: Python, Programming, Concurrency, Parallelism
theme: minima
---

This tutorial will cover some aspects of concurrency in Python. This is intended for beginners, but advanced users may find a few useful bits and pieces. It can be best followed by trying it out. So, fire up your favorite editor and follow along!

Let me begin by distinguishing between concurrency and parallelism as it can easily be confused.
Concurrency: Running programs or units of computation simultaneously but one at a given time
Parallelism: Running computations simultaneously at the same time. Parallelism is concurrent but not vice-versa.

In Python concurrency can be accomplished using multithreading, while parallelism, using multiprocessing. This is in part due to the nature of the GIL (Global interpreter Lock) that prevents threads from running all at the same time.
However, each process in Python, is an interpreter in itself and would each have its own GIL. Processes therefore, run in parallel, while threads within it, run concurrently.

There are various libraries in Python for multithreading and multiprocessing, but for the scope of this tutorial, we restrict it to exploring packages that are part of the standard library.

To spice things up a bit, let's attempt to solve the following problem:

Read data from 

{% highlight python %}
# Required imports
import multithreading
import multiprocessing

{% endhighlight %}

Check out the [Jekyll docs][jekyll-docs] for more info on how to get the most out of Jekyll. File all bugs/feature requests at [Jekyll’s GitHub repo][jekyll-gh]. If you have questions, you can ask them on [Jekyll Talk][jekyll-talk].

[jekyll-docs]: http://jekyllrb.com/docs/home
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-talk]: https://talk.jekyllrb.com/
