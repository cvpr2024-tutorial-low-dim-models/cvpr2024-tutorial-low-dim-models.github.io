---
layout: default
twitter_card:
  type: summary_large_image
---

{% include title.html %}

## Overview

Over the past decade, the advent of machine learning and large-scale computing
has immeasurably changed the ways we process, interpret, and predict with data
in imaging and computer vision. The "traditional" approach to algorithm
design, based around parametric models for specific structures of signals and
measurements---say sparse and low-rank models---and the associated optimization
toolkit, is now significantly enriched with data-driven learning-based
techniques, where large-scale networks are pre-trained and then adapted to a
variety of specific tasks. Nevertheless, the successes of both modern
data-driven and classic model-based paradigms rely crucially on correctly
identifying the low-dimensional structures present in real-world data, to the
extent that we see the roles of learning and compression of data processing
algorithms---whether explicit or implicit, as with deep networks---as
inextricably linked.

As such, this tutorial provides a timely tutorial that
uniquely bridges low-dimensional models with deep learning in imaging and
vision. This tutorial will show how:

1. Low-dimensional models and principles provide a valuable lens for
   formulating problems and understanding the behavior of modern deep models in
   imaging and computer vision; and how
2. Ideas from low-dimensional models can provide valuable guidance for
   designing new parameter efficient, robust, and interpretable deep learning
   models for computer vision problems in practice.

We will begin by introducing
fundamental low-dimensional models (e.g., basic sparse and low-rank models)
with motivating computer vision applications.
Based on these developments, we
will discuss strong conceptual, algorithmic, and theoretical connections
between low-dimensional structures and deep models, providing new perspectives
to understand state-of-the-art deep models in terms of learned representations,
generalizability, and transferability.
Finally, we will demonstrate that these
connections can lead to new principles for designing deep networks learning
low-dimensional structures in computer vision, with both clear interpretability
and practical benefits.
We will conclude with a **panel discussion** with expert researchers from academia
and industry on what role low-dimensional models can and should play in our
current age of opaque large language models and foundation models for computer
vision.

## Speakers

<div style="clear: both; display: flex; flex-wrap: wrap; justify-content:
  space-evenly; ">

{% assign orgs = site.organizers %}
{% for organizer in orgs %}
{{ organizer }}
{% endfor %}

</div>

## Panelists

<div style="clear: both; display: flex; flex-wrap: wrap; justify-content:
  space-evenly; ">

{% assign pans = site.panelists %}
{% for panelist in pans %}
{{ panelist }}
{% endfor %}

</div>

## Schedule

This tentative schedule will be updated when the full CVPR schedule is
announced.

<table>
<colgroup>
<col width="69%" />
<col width="17%" />
<col width="14%" />
</colgroup>
<thead>
<tr>
<th>Lecture</th>
<th>Speaker</th>
<th>Time (PT)</th>
</tr>
</thead>
<tbody>
<tr>
<td class="title" colspan="3" markdown="span">
**Session 1:** Principles of Basic Low-Dimensional Models
</td>
</tr>
<tr>
<td>
Introduction to Basic Low-Dimensional Models
<br>
<a class="abstract btn btn-sm z-depth-0" role="button" style="color:#959396;">(Lecture Abstract)</a>
<br>
<div class="abstract hidden">
<p>
The first part will introduce fundamental properties and results for sensing, processing, analyzing, and learning low-dimensional structures from high-dimensional data. We will first discuss classical low-dimensional models, such as sparse coding and low-rank matrix sensing, and motivate these models by applications in computer vision. Based on convex relaxation, we will characterize the conditions, in terms of sample/data complexity, under which the learning problems of recovering such low-dimensional structures become tractable and can be solved efficiently, with guaranteed correctness or accuracy.
</p>
</div>
</td>
<td markdown="span">
  <a href="https://people.eecs.berkeley.edu/~yima/">Yi Ma</a>
</td>
<td markdown="span">
9:00-10:00
</td>
</tr>
<tr>
<td>
Introduction to Low-Dimensional Models in Deep Learning
<br>
<a class="abstract btn btn-sm z-depth-0" role="button" style="color:#959396;">(Lecture Abstract)</a>
<br>
<div class="abstract hidden">
<p>
Next, we delve into the core principles of low-dimensional models within
various neural network architectures. Specifically, we will introduce
<em>unrolled optimization</em> as a design principle for interpretable deep
networks. As a simple special case, we will examine several unrolled
optimization algorithms for sparse coding, and show that they exhibit striking
similarities to current deep network architectures. These unrolled networks are
white-box and interpretable <em>ab initio</em>.
</p>
</div>
</td>
<td markdown="span">
  <a href="https://sites.google.com/view/yuqianzhang">Yuqian Zhang</a>
</td>
<td markdown="span">
10:00-11:00
</td>
</tr>
<tr>
<td class="title" colspan="3" markdown="span">
**Session 2:** Understanding Low-Dimensional Representations & Learning in Deep Networks
</td>
</tr>
<tr>
<td>
Understanding Low-Dimensional Representation via Neural Collapse
<br>
<a class="abstract btn btn-sm z-depth-0" role="button" style="color:#959396;">(Lecture Abstract)</a>
<br>
<div class="abstract hidden">
<p>
The session focuses on the strong conceptual connections between low-dimensional structures and deep models in terms of learned representation. We start with the introduction of an intriguing Neural Collapse phenomenon in the last-layer representation and its universality in deep network, and lays out the mathematical foundations of understanding its cause by studying its optimization landscapes. We then generalize and explain this phenomenon and its implications under data imbalancedness. Furthermore, we demonstrate the practical algorithmic implications of Neural Collapse on training deep neural networks.
</p>
</div>
</td>
<td markdown="span">
  <a href="https://cse.osu.edu/people/zhu.3440">Zhihui Zhu</a>
</td>
<td markdown="span">
11:15-12:15
</td>
</tr>
<tr>
<td>
Invariant Low-Dimensional Subspaces of Learning Dynamics
<br>
<a class="abstract btn btn-sm z-depth-0" role="button" style="color:#959396;">(Lecture Abstract)</a>
<br>
<div class="abstract hidden">
<p>
Second, we show that low-dimensional structures also emerge in training dynamics of deep networks. Specifically, we show that the evolution of gradient descent only affects a minimal portion of singular vector spaces across all weight matrices. The analysis enables us to considerably improve training efficiency by taking advantage of the low-dimensional structure in learning dynamics. We can construct smaller, equivalent deep linear networks without sacrificing the benefits associated with the wider counterparts. Moreover, it allows us to better understand deep representation learning by elucidating the progressive feature compression and discrimination from shallow to deep layers.
</p>
</div>
</td>
<td markdown="span">
  <a href="https://qingqu.engin.umich.edu/">Qing Qu</a>
</td>
<td markdown="span">
13:30-14:30
</td>
</tr>
<tr>
<td class="title" colspan="3" markdown="span">
**Session 3:** Designing Deep Networks for Pursuing Low-Dimensional Structures
</td>
</tr>
<tr>
<td>
ReduNet: A White-box Deep Network from the Principle of Maximizing Rate Reduction
<br>
<a class="abstract btn btn-sm z-depth-0" role="button" style="color:#959396;">(Lecture Abstract)</a>
<br>
<div class="abstract hidden">
<p>
In this part, we will focus on the special yet highly useful case of learning
the data distribution and transforming it to an <em>linear discriminative
representation</em> (LDR). We will discuss the information theoretic and
statistical principles behind such a representation, and design a loss
function, called the <em>coding rate reduction</em>, which is optimized at such
a representation. By unrolling the gradient ascent on the coding rate
reduction, we will construct a deep network architecture, called the ReduNet,
where each operator in the network has a mathematically precise (hence
white-box and interpretable) function in the transformation of the data
distribution towards an LDR. Also, the ReduNet may be constructed layer-wise in
a forward-propagation manner, that is, without <em>any</em> back-propagation
required.
</p>
</div>
</td>
<td markdown="span">
  <a href="https://people.eecs.berkeley.edu/~yima/">Yi Ma</a>
</td>
<td markdown="span">
14:45-15:45
</td>
</tr>
<tr>
<td>
White-Box Transformers via Sparse Rate Reduction
<br>
<a class="abstract btn btn-sm z-depth-0" role="button" style="color:#959396;">(Lecture Abstract)</a>
<br>
<div class="abstract hidden">
<p>
In the final part, we demonstrate how combining sparse coding and rate
reduction yields "sparse linear discriminative representations" using an
objective called sparse rate reduction. We develop CRATE, a deep network
architecture, by unrolling the optimization of this objective and
parameterizing feature distribution in each layer. CRATE's operators are
mathematically interpretable, with each layer representing an optimization
step, making the network a transparent "white box". Although CRATE's design
significantly differs from ReduNet, both aim for a similar goal, showcasing the
versatility of the unrolled optimization approach. Remarkably, CRATE closely
resembles the transformer architecture, suggesting that the interpretability
gains from such networks might also improve our understanding of current,
practical deep architectures.
</p>
</div>
</td>
<td markdown="span">
  <a href="https://sdbuchanan.com">Sam Buchanan</a>
</td>
<td markdown="span">
15:45-16:45
</td>
</tr>
<tr>
<td class="title" colspan="2" markdown="span">
**Session 4:** Panel Discussion
</td>
<td markdown="span">
17:00-18:00
</td>
</tr>
</tbody>
</table>

## Materials

Slides and recordings will be posted here after the event.
