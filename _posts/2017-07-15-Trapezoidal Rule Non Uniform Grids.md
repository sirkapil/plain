---
layout: post
title: Trapezoidal Rule for non-uniform grid
author: Kapil Chaudhary
tag: [Numerical Method, Newton Cotes Rule]
excerpt_separator: <!--more-->
---
	
	
	
<p align="center">We have already discussed about<u><b><a href="/Trapezoidal-Rule.html"> Trapezoidal Rule for uniform grids .</a></u></b></p>
<p> Now Let's discuss about non-uniform panels! 
<!--more-->
What will be our approximate numerical integral value if interval [a,b] is partitioned in such a way that each sub-interval is of non-uniform length ?
Like [0,1] is partitioned in this following format :</p><br />
<p align="center">$[0,\frac{1}{3}] \cup [\frac{1}{3},\frac{1}{2}] \cup [\frac{1}{2},1]$</p><br />
<p align="center">
   Notice that each sub-interval is of different length
   .We'll be naming length of $i^{th}$ subinterval as $h_i$
   as in above example of partition of [0,1] , we have 
   $h_1 =\frac{1}{3}$
   $h_2 =\frac{1}{6}$
   $h_3 =\frac{1}{2}$
</p> 
    