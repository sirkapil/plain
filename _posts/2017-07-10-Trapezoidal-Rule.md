---
layout: post
title: Introduction to Trapezoidal Rule
author: Kapil Chaudhary
excerpt_separator: <!--more-->
tags: [Numerical Method]
---
<div class="isa_info"><b>Introduction:</b> <br />This is one of the Newton-Cotes Formulae used for evaluating approximate numerical value of a definite integral.</div>
<!--more--><div class="divider"></div>
<h2>Why "Trapezoidal" Name ?</h2>
It approximates the region under the graph as a trapezoid.Look at following two images of simple and composite trapezoidal rules in action -equation[^1.1] , equation[^1.2]
<div class="divider"></div>
<h2>Accuracy : </h2>
This Mehod is pretty accurate for evaluating approximate values of periodic functions over thier period.however it is not much accurate for non-periodic functions.Simple Trapezoidal rule[^1] even fails to integrate Quardratic polynomials so it has degree of precision 1 and  Composite Trapezoidal Rule[^2] fails to integrate a Cubic Polynomial so its degree of precision is 2.
<div class="divider"></div>
<h2> How it Works ? </h2>
First , We do create partition for [a,b] where a and b are lower and upper limit of integral respectively.
In Regular Grids or Uniform Partition, [a,b] interval is distributed into N subintervals of same length (Named as Step size and denoted by 'h')
In General , If [a,b] is distribuited uniformly into n subintervals, Then
<center>$$ a < a+h < a+2h < \cdots < a+nh = b$$
$$a+nh = b $$ $$h = \frac{b-a}{n}$$</center>
<br /><small>However it is also possible to do partition of [a,b] with irregular lengths , in such case Formulae for Trapezoidal rule is different[^3]
</small>
<h3>Formulae :</h3>
<h3>Simple Trapezoidal Rule -</h3>
<br />[^1.1]:
$$\int_{a}^{b}f(x)dx \approx (b-a)\left[\frac{f(a)+f(b)}{2}\right]$$
<h3>Composite Trapezoidal Rule</h3> 
[^1.2]:
$$\int_{a}^{b}f(x)dx \approx \frac{h}{2}\left[f(a)+f(b)+2\sum_{k=1}^{n-1}f(a+kh)\right]$$



[^1]: Simple Trapezoidal Rule
[^2]: Composite Trapezoidal Rule
[^3]: Link to [Trapezoidal Rule Nonuniform grids](/non-uniform-grid)


