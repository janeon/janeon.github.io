---
layout: post
title: Star-clustering
author: Jane Hsieh
date: '2018-05-16 14:35:23 +0530'
category: projects
summary: C++, shell scripting, gnuplot, SIMBAD
thumbnail: posts/kc_plot_1.png
---

This project uses the k-means algorithm and the elbow method to identify potential star and galaxy clusters.

It first queries for astronomical data (star / galaxy coordinates) from the <a href="https://simbad.u-strasbg.fr/simbad/sim-fid">SIMBAD</a> database

Bash shell scripting used to
<ul>
<li> clean resultant data </li>
</ul>

C++ used to
<ul>
<li> convert coordinates from RA and Dec (right ascension and declination) to x-y coordinates for 2D plotting </li>
<li> use the elbow method (by running the clustering over a range of k values) to find the optimal number of clusters</li>
<li> running k-means (where k is determined on the previous step) on the data and plotting it with <a href="http://www.gnuplot.info/">gnuplot</a></li>
</ul>




Checkout our project source code on <a href="https://github.com/janeon/k-clustering_project">Github</a>!

Some resultant plots:
<div>
<img src="/assets/img/posts/kc_plot_1.png" style="width:50%; float: left;">
<img src="/assets/img/posts/kc_plot_2.png" style="width:47%; float: left; padding-top: 0.95em">
</div>
