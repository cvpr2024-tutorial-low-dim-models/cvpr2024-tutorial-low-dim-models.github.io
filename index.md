---
layout: default
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
<td markdown="span">
Introduction to Basic Low-Dimensional Models
</td>
<td markdown="span">
  <a href="https://people.eecs.berkeley.edu/~yima/">Yi Ma</a>
</td>
<td markdown="span">
9:00-10:00
</td>
</tr>
<tr>
<td markdown="span">
Introduction to Low-Dimensional Models in Deep Learning
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
<td markdown="span">
Understanding Low-Dimensional Representation via Neural Collapse
</td>
<td markdown="span">
  <a href="https://cse.osu.edu/people/zhu.3440">Zhihui Zhu</a>
</td>
<td markdown="span">
11:15-12:15
</td>
</tr>
<tr>
<td markdown="span">
Invariant Low-Dimensional Subspaces of Learning Dynamics
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
<td markdown="span">
ReduNet: A White-box Deep Network from the Principle of Maximizing Rate Reduction
</td>
<td markdown="span">
  <a href="https://people.eecs.berkeley.edu/~yima/">Yi Ma</a>
</td>
<td markdown="span">
14:45-15:45
</td>
</tr>
<tr>
<td markdown="span">
White-Box Transformers via Sparse Rate Reduction
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
