---
layout: post
title: conformal mappings and angle between curves
---

## Path :

Let G be a region containing points A and B,
a 'PATH' from point A to point B , is a continuous function ($\gamma$) defined as

$$\gamma : [a,b] @>>> \mathcal{G}$$

such that $\gamma(a) = A$ , 
$\gamma(b) = B $

### Examples of paths

### Smooth and Piecewise Smooth Paths :

Let $\gamma$ be a path from A to B ; $\gamma(a) =A$ and 
$\gamma(b) =B$ , we say $\gamma$ is a smooth path from A to B iff 
$\gamma(t)$ is differentiable at each point $t \in (a,b)$

If $\gamma(t)$ fails to be differentiable at certain points ($k_1,k_2, \cdots , k_n$) between $(a,b)$ then we say $\gamma$ is piecewise smooth path.

We'll be using term 'curve' for smooth or piecewise smooth paths.

## Angle between smooth curves

Let $\gamma_1,\gamma_2$ be two smooth paths through point $z_0$ (i.e. $\gamma_1 (t_1)= \gamma_2 (t_2) =z_0$ ).
Then , Angle between curves $\gamma_1$ and $\gamma_2$ at point $z_0$ is given by :

$$ \bbox[yellow,5px,border:2px solid red] {\theta = arg[{\gamma_1}'(t_1)] - arg[{\gamma_2}'(t_2)] }$$

## Composition of analytic function over a smooth path is again a smooth path ?

Yes, Composition of analytic function over a smooth path is again a smooth path.

<b>Proof :</b> 

So we need to show $f\circ\gamma$ is analytic.

## How to calculate angle b/w new paths formed by composition of an analytic function over old paths ?



## Conformal Map :

A mapping that preserves angle between curves.
That is if $\theta$ is angle b/w two smooth paths $\gamma_1$ and $\gamma_2$ passing through $z_0$ then angle ($\theta$) will remain unchanged b/w new paths obtained by composition of a conformal map over $\gamma_1$ and $\gamma_2$ .
if $f$ be conformal map , then between paths $\sigma_1 = f\circ\gamma_1$ and $\sigma_2 = f \circ \gamma_2$ through point $f(z_0)$is same as $\gamma_1$ and $\gamma_2$ through $z_0$

## Analytic Map is Conformal map and conformal map is analytic map.