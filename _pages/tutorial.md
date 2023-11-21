---
layout: page
permalink: /book/
title: book
nav: true
nav_order: 4
cv_pdf: example_pdf.pdf
---
Computational Imaging through Atmospheric Turbulence: get a [physical copy](https://www.barnesandnoble.com/w/computational-imaging-through-atmospheric-turbulence-stanley-h-chan/1143986968) or a draft PDF [here](https://nchimitt.github.io/assets/pdf/CI_atm_turb_book.pdf) for free!


<img src="/assets/img/book.webp" width="25%" height="25%" class="float-right" />


Since the seminal work of Andrey Kolmogorov in the early 1940’s, imaging through atmospheric turbulence has grown from a pure scientific pursuit to an important subject across a multitude of civilian, space-mission, and national security applications. Fueled by the recent advancement of deep learning, the field is further experiencing a new wave of momentum. However, for these deep learning methods to perform well, new efforts are needed to build faster and more accurate computational models while at the same time maximizing the performance of image reconstruction.


The book is written primarily for image processing engineers, computer vision scientists, and engineering students who are interested in the field of atmospheric turbulence, statistical optics, and image processing. The book can be used as a graduate text, or advanced topic classes for undergraduates.


Below you'll find brief summaries for each chapter.

---
**Chapter 1**

The first chapter discusses basic principles of the book: what is turbulence, how does it manifest in imaging over long distances, and what are the main roadblocks holding back current restoration methods? 

---
**Chapter 2**

The basics of Fourier optics are presented in this chapter. Here, we're aimed at getting the main results of Fourier optics conveyed in a (relatively) short amount of space. First, light should be modeled as a wave. This is critical for understanding how light is degraded by the turbulent atmosphere and how it affects an image. Furthermore, how does light move from one place to another if it is indeed a wave; are there any approximations we can make? This leads us to introduce Fresnel and Fraunhofer diffraction. Finally, we discuss point spread functions (PSFs) and related topics along with spatially varying linear systems.

---
**Chapter 3**

This chapter contains the classical description and models for atmospheric turbulence, which we adopt the model of turbulence being a random field. We then are quick to introduce the structure function -- a unique property of the turbulence literature. One will not find an autocovariance function written anywhere, instead, one must use structure functions. We then move towards using a layered model for turbulence to arrive at the effects the turbulence has on the phase of a wave which propagates through it. Finally, we discuss the most precise framework for simulating wave propagation through turbulence: split-step propagation. 

---
**Chapter 4**

The last chapter covered the more classical description of turbulence, while this chapter discusses a perspective that we take in thinking about turbulence. The foundations of these ideas date back to the 1970's when David Fried and Robert Noll considered a basis representation to describe the effects that a wave experiences by turbulence. The model we discuss here takes this and applies more modern considerations to it. We use some learning-based tricks, properties of random number generation, and a few additional considerations to develop a simulator which is 1000 times faster than split-step propagation (although this number varies, it is a reasonable estimation). At the core of this is representing a spatially varying impulse response as a sum of invariant responses and a learning-based trick known as the phase-to-space (P2S) transform. The P2S transform gives us a lot of useful properties for inverse problems: it's a neural network!


---
**Chapter 5**

This chapter concludes the book with discussing inverse problems and how a simulator can be used to aid in reconstruction. We talk about various aspects of the inverse problem: how should the forward operator be formulated in an approximate way, how can better data help us restore, and what properties are unique to turbulence that we need to consider? We present various topics such as lucky imaging, optical flow, and multi-vs-single-frame restoration methods.