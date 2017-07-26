---
layout: post
title: Sepreted Sets & Disjoint Sets
tags: [point set topology]
excerpt_separator: <!--more-->
author: Kapil Chaudhary
---
In this post,We shall discuss about an important topic of <a href="/tags#point+set+topology">point set topology</a> that is
Seperated Sets and Disjoint Sets. <!--more-->
<br />

<h1>Definitions :</h1>
<div class="divider"></div>
<div class="box2">
<p><b>Disjoint Sets</b>: <br />Let $A$ and $B$ be two non-empty sets, We say $A$ and $B$ are disjoint if
<br /><center>$$ A \cap B = \phi$$
</center>
</p></div>
i.e. both sets must have no common point. if both have any point common , we say sets are "_joint sets_".<br />
**Examples :**

|  $A$      |  $B$     | $A \cap B$ |   Joint/Disjoint |
|-----------|:--------:|:-----------:|-----------------:|
| $[0,1]$   | $(1,2)$  | $\phi$   | Disjoint       |
| $[0,1]$   | $[1,2)$  | ${1}$   | Joint set touching at point 1     |
| $[0,1]$   | $(1,2)$  | $\phi$   | Disjoint       |
| $[0,1]$   | $(-1,2)$  | $[0,1]$   | Joint $       |
| $(a,b]$   | $(c,b]$  | $A$ if $a<c \\ B$ if $a>c$  | joint       |



<div class="box2">
<p><b>Seperated Sets</b>: <br />Let $A$ and $B$ be two non-empty sets,We say sets $A$ and $B$ are seperated if following two conditions holds :<br />
<center>$$ A \cap \overline{B} = \phi$$ 
$$ \overline{A} \cap B = \phi$$
</center></p>
</div>

