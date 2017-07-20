---
layout: post
title: Introduction to Trapezoidal Rule
author: Kapil Chaudhary
excerpt_separator: <!--more-->
tags: [Numerical Method]
---
<div class="isa_info"><h1><i class="fa fa-arrow-right"></i>Introduction:</h1> <br /><p align="center">This is one of the Newton-Cotes Formulae used for evaluating approximate numerical value of a definite integral.</p></div>
<!--more--><div class="divider"></div>
<h2>Why "Trapezoidal" Name ?</h2>
It approximates the region under the graph as a trapezoid.Look at image of  trapezoidal rules in action.
![trapezoidal in action](/alpha/img/IMG_20170720_174523.jpg)
<div class="divider"></div>
<h2>Accuracy : </h2>
This Mehod is pretty accurate for evaluating approximate values of periodic functions over thier period.however it is not much accurate for non-periodic functions.Simple Trapezoidal rule[^1] even fails to integrate Quardratic polynomials so it has degree of precision 1 and  Composite Trapezoidal Rule[^2] fails to integrate a Cubic Polynomial so its degree of precision is 2.
<div class="divider"></div>
<h2> How it Works ? </h2>
<h3>Simple Trapezoidal Rule:</h3>

![simple Trapezoidal rule](/alpha/img/IMG_20170720_181014.jpg)

<h3> Composite Trapezoidal Rule:</h3>
First , We do create partition for [a,b] where a and b are lower and upper limit of integral respectively.
In Regular Grids or Uniform Partition, [a,b] interval is distributed into $$n$$ subintervals of same length[^3].
**In General**, If [a,b] is distributed uniformly into n subintervals. Let $$S_i$$ be $$i^{th}$$ interval with step size(_h_).
$$S_1 = [a , a+h] \\ S_2 = [a+h , a+2h] \\ \vdots \\ S_i = [a+(i-1)h , a+ih] \\ \vdots \\ S_n = [a+(n-1)h , b]$$ 
<center>
$$[a,b] = \bigcup_{i=1}^{n} S_i$$
</center>
It forms a increasing monotonic finite sequence of points.
<center>
$$ a < a+h < a+2h < \cdots < a+nh = b$$
$$a+nh = b \\ h = \frac{b-a}{n}$$</center>

Now, Apply Simple Trapezoidal Rule for each of the subinterval $$S_i$$.

$$\int_{a}^{b} f(x) dx = \sum\limits_{i=1}^{n} [\int_{S_i}{} f(x)dx ]$$

$$\approx \sum\limits_{i=1}^{n} h\left[\frac{f(a+(i-1)h)+f(a+ih)}{2}\right]$$

$$= \frac{h}{2}\left[f(a)+f(b)+2\sum\limits_{i=1}^{n-1}f(a+ih)\right] $$

$$= \frac{(b-a)}{2n}\left[f(a)+f(b)+2\sum\limits_{i=1}^{n-1}f(a+ih)\right] $$ 

as $$h = \frac{b-a}{n}$$<br />
**Example**
Let's take a very simple example , integrating $$f(x)= sin(x)$$ over interval [0,2] by partition into two uniform subinterval (n=2). <br />
**Answer**
![Uniform Grid Composite Trapezoidal Rule integrating sine function over 0 to 2](/alpha/img/IMG_20170720_180952.jpg)

<div class="isa_info">
<b>Note :</b> If we will increase the value of <i>n</i> then partition will  become smaller and smaller and consequently our answer will be more accurate.
<b>"As Smaller Partition , As Accurate Answer"</b></div>

Check this following image
(Source- Wiki) showing how accuracy increase in answer while increasing _n_
![Effect of increasing n in composite Trapezoidal rule](/alpha/img/trapezium2.gif)

<br /><small>**Note:**
However , it is also possible to do partition of [a,b] with irregular length.[^4]
</small>
<h3>Formulae :</h3>
<h3>Simple Trapezoidal Rule -</h3>
<br />Equation(1) :
$$\int_{a}^{b}f(x)dx \approx (b-a)\left[\frac{f(a)+f(b)}{2}\right]$$
<h3>Composite Trapezoidal Rule</h3>
Equation(2) :
$$\int_{a}^{b}f(x)dx \approx \frac{(b-a)}{2n}\left[f(a)+f(b)+2\sum\limits_{k=1}^{n-1}f(a+kh)\right]$$ 

<div class="divider"></div>

### Error Analysis



<div class="divider"></div>
**Source / Credits :** <br />
1.Book (Numerical Methods) By M.K Jain and Co. IIT Delhi.<br />
2.Satyendra K. (My N.M. Teacher)<br />
3.Wikipedia (For few images)




[^1]: Simple Trapezoidal Rule is just a special case of composite Trapezoidal Rule with (n=1), i.e. in simple trapezoidal rule , we don't partition the interval [a,b] into further subintervals.
[^2]: Composite Trapezoidal Rule is much accurate than Simple Trapezoidal Rule.
[^3]: that same length is named as _Step Size_ , denoted by _h_ and is always a positive number.
[^4]: Link to Article [Trapezoidal Rule with non-uniform step size](/non-uniform-step-size-trapezoidal-rule)




