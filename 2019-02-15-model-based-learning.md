---
id: 1059
title: Model-Based Machine Learning
date: 2019-02-15T23:37:44+05:30
author: admin@sciloo.com
layout: post
guid: https://sciloo.com/?p=1059
permalink: /2019/02/15/model-based-learning/
colormag_page_layout:
  - default_layout
xyz_smap:
  - "1"
categories:
  - research
  - technology
tags:
  - healthcare
  - machine learning
---
ML not equal to data + black box&nbsp;

ML = data + assumptions&nbsp;&nbsp;

**Free Lunch Theorem**&nbsp;

As per free lunch theorem, without assumptions we can’t build anything.&nbsp;We can’t have one generic&nbsp;<g class="gr_ gr\_4 gr-alert gr\_spell gr\_inline\_cards gr\_run\_anim ContextualSpelling ins-del multiReplace" id="4" data-gr-id="4">algo</g>&nbsp;that is applicable for all the problems.&nbsp;&nbsp;

We have&nbsp;**constraints&nbsp;**like&nbsp;&nbsp;

&nbsp; assumptions,&nbsp;&nbsp;

&nbsp; prior knowledge,&nbsp;&nbsp;

&nbsp; domain knowledge&nbsp;

&nbsp;when dealing with problems and without considering these how we can solve a problem.&nbsp;

**Data + prior knowledge**&nbsp;

Detection of a person in frame&nbsp;

In a simple approach, we will need many images with person at different location.&nbsp;

But with this knowledge, we can develop transformations to shift a person in the image and then train the model on these images instead of acquiring those images.&nbsp;

We tend to think about Big data that we can develop weak models and can forget the constraints/assumptions.&nbsp;

There are 2 types of sizes&nbsp;

&nbsp; 1. computation size&nbsp;

&nbsp; 2. statistical size&nbsp;

<div class="wp-block-image">
  <figure class="alignleft is-resized"><img loading="lazy" src="http://sciloo.com/wp-content/uploads/2019/02/image.png" alt="" class="wp-image-1060" width="243" height="198" /></figure>
</div><figure class="wp-block-image is-resized">

<img loading="lazy" src="http://sciloo.com/wp-content/uploads/2019/02/image-1.png" alt="" class="wp-image-1061" width="236" height="195" /> </figure> 



Computationally small but statistical big&nbsp;

Without assumptions, how we can predict a current value for a new voltage value?&nbsp; On the right side, we can take into consideration about V = IR and can be confident that the line is good predictor for future voltage values. This dataset is small in computational size but big in statistical size.&nbsp;<figure class="wp-block-image is-resized">

<img loading="lazy" src="http://sciloo.com/wp-content/uploads/2019/02/image-3.png" alt="" class="wp-image-1063" width="384" height="261" /> </figure> 

Statistically small but computationally big&nbsp;

The above data is computationally big, take a simple example of a <g class="gr_ gr\_5 gr-alert gr\_gramm gr\_inline\_cards gr\_run\_anim Grammar only-ins doubleReplace replaceWithoutSep" id="5" data-gr-id="5">black</g> and white image of 10X10 pixel, all the combinations can yield combinations that might be more than the total number of atoms in the universe.&nbsp;

Unless we make assumptions, it is very difficult to do computation with these big set of images. This above images data can be computationally very large but statistically very small.&nbsp;

**Model based ML**&nbsp;

Instead of getting lost in the sea of algorithms/models/research papers, we should use model-based learning to use data and assumptions to derive ML algorithm.&nbsp;We should work mainly on defining our assumptions about the problem very clearly.&nbsp;&nbsp;<figure class="wp-block-embed-youtube wp-block-embed is-type-video is-provider-youtube wp-embed-aspect-16-9 wp-has-aspect-ratio">

<div class="wp-block-embed__wrapper">
</div></figure> 

Translate your assumptions into a model and that is the core of model-based learning. If our assumptions are sound/strong then we get much more information from the same amount of data.&nbsp;

Can we develop a tool to do it automatically? Can this dream be true?&nbsp;<figure class="wp-block-image is-resized">

<img loading="lazy" src="http://sciloo.com/wp-content/uploads/2019/02/image-4.png" alt="" class="wp-image-1064" width="288" height="235" /> </figure> 

**User & Movies**&nbsp;

Predict the question marks – whether a user like or dislike&nbsp;those movie&nbsp;for which he has not given&nbsp;a&nbsp;answer. 10ks of movies, 10Ms of users.&nbsp;<figure class="wp-block-image is-resized">

<img loading="lazy" src="http://sciloo.com/wp-content/uploads/2019/02/image-2.png" alt="" class="wp-image-1062" width="433" height="331" /> </figure> <figure class="wp-block-image is-resized"><img loading="lazy" src="http://sciloo.com/wp-content/uploads/2019/02/image-5-1024x507.png" alt="" class="wp-image-1065" width="618" height="306" /></figure> 

Based on my like or dislike, ML is suggesting movies closer to green area that I can like for sure and closer to red area for movies that I may not like.&nbsp;

It is learning my behavior and suggesting me titles based on the populations&nbsp;similar to&nbsp;me.&nbsp;

Information (as per information theory by&nbsp;Shanon) is the surprise from data. Just like above movie ML&nbsp;algo&nbsp;suggest me movies closer to green area and I pick then there is a very less surprise in the data and suggestions don’t move big.&nbsp;

But instead of liking the movie, if I dislike it, it is a big surprise for the&nbsp;algo&nbsp;and movies suggestions move big.&nbsp;

**Quantifying uncertainty**&nbsp;

Uncertainty is an essential part of machine learning and it is a modern view of ML.&nbsp;**Bayes theorem**&nbsp;is at the core of it.&nbsp;

BT: P(A/B) = [P(A) * P(B/A)]/P(B)&nbsp;

**Bishop view on Healthcare**&nbsp;<figure class="wp-block-embed-youtube wp-block-embed is-type-video is-provider-youtube wp-embed-aspect-16-9 wp-has-aspect-ratio">

<div class="wp-block-embed__wrapper">
</div></figure> 

It is one of the biggest opportunities but complex also. Personalized healthcare can be a phenomenon suggesting you personalized course of treatment because as an individual each one of us is unique. It is like machine can learn our movies preferences.&nbsp;

&nbsp;This can happen by analyzing the info from other millions of people.&nbsp;&nbsp;

&nbsp; Cloud based tech + ML tech + Domain experts (from Hospitals like clinicians, doctors, radiologists, etc.)&nbsp;

**Trust and privacy in the Data**&nbsp;

Data is encrypted so it is only accessible to those who have keys but It can become vulnerable while being processed. So Microsoft has taken care of processing data in <g class="gr_ gr\_7 gr-alert gr\_gramm gr\_inline\_cards gr\_run\_anim Grammar only-ins replaceWithoutSep" id="7" data-gr-id="7">secure</g> vault kind of infrastructure where data can be <g class="gr_ gr\_10 gr-alert gr\_spell gr\_inline\_cards gr\_run\_anim ContextualSpelling" id="10" data-gr-id="10">access</g> only to people who have keys. It is secure by hardware and software. 

**Factor Graph**<figure class="wp-block-image">

<img src="http://sciloo.com/wp-content/uploads/2019/02/image-18.png" alt="" class="wp-image-1120" /> </figure> 

The probability of getting a circular or triangular cookie depends upon which jar we choose. Round circles on the right sides are &#8211; one random variable for Jar, one random variable for Cookie

These random variables are driven by their respective probability distribution functions (PDFs) denoted as shaded squares.