---
layout: post
title: Introduction to Trapezoidal Rule
author: Kapil Chaudhary
excerpt_separator: <!--more-->
tags: [Numerical Method]
---
<p>This is one of the Newton-Cotes Formulae used for evaluating approximate numerical value of a definite integral.</p>
<!--more-->
<h2>Why "Trapezoidal" Name ? :</h2>
It approximates the region under the graph as a trapezoid.Look at following two images of simple and composite trapezoidal rules in action -
<img src="http://sirkapil.github.io/img/trapezoidal rule/220px-Trapezoidal_rule_illustration.png"><img src="https://sirkapil.github.io/img/trapezoidal%20rule/Composite_trapezoidal_rule_illustration.svg.png">
<h2>Accuracy : </h2><br />
This Mehod is pretty accurate for evaluating approximate values of periodic functions over thier period.
however it is not much accurate for non-periodic functions.Simple Trapezoidal rule even fails to integrate Quardratic polynomials so it has degree of precision 1 and A Composite Trapezoidal Rule fails to integrate a Cubic Polynomial so its degree of precision is 2.
<h2> How it Works ? </h2>
First , We do create partition for [a,b] where a and b are lower and upper limit of integral respectively.
In Regular Grids or Uniform Partition, [a,b] interval is distributed into N subintervals of same length (Named as Step size and denoted by 'h')
In General , If [a,b] is distribuited uniformly into n subintervals, Then
<center>$$ a < a+h < a+2h < \cdots < a+nh = b$$
$$a+nh = b $$ $$h = \frac{b-a}{n}$$</center>
<br /><small>However it is also possible to do partition of [a,b] with irregular lengths , in such case Formulae for Trapezoidal rule is different (i'll post about it too in another aricle whenever it will be ready, a link to that article will be pasted here)
</small>
<h2>Formulae :</h2>
<h3>Simple Trapezoidal Rule -</h3>
<br />
$$\int_{a}^{b}f(x)dx \approx (b-a)\left[\frac{f(a)+f(b)}{2}\right]$$<br /><br />
<h3>Composite Trapezoidal Rule -</h3>
$$\int_{a}^{b}f(x)dx \approx$$ $$(b-a)\left[\frac{f(a)+f(b)+2\sum_{k=1}^{n-1}f(a+kh)}{2n}\right]$$ where $$h = \frac{b-a}{n}$$
