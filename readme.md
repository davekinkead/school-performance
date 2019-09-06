---
title: What do student results tell us about school performance?
author: Dave Kinkead
email: d.kinkead@uq.edu.au
status: abstract
license: CC BY SA
---

## Abstract 

> Measuring school performance has become an important activity within our education systems.  Today, most developed countries have some metric to rank and compare schools --- Adequate Yearly Progress (AYP) of No Child Left Behind (NCLB), Progress 8 scores, National Assessment Program - Literacy and Numeracy (NAPLAN), Trends in International Mathematics and Science Study (TIMSS), and the Programme for International Student Assessment (PISA).

> Yet these measures are only substitutes for what we are really interested in --- how much do schools influence student achievement. Because we can't measure the causal impact of schooling on student achievement directly, we can't know what impact schools have with any certainty.  Instead, we must _infer_ the causal impact of schooling on student achievement by way of proxy measures such as standardised student test scores which presents us with a significant epistemic challenge. 

> This paper introduces a novel approach to computer simulation to argue that the presence of choice or selectivity within a school system undermines measures of school performance based on student acheivement.  In it, I develop a simple model in order to investigate the robustness of the inference from student achievement to school performance.  I then demonstrate how the introduction of school choice or selectivity leads to a complete failure of the inference mechanism.

> My claim is simple --- _if an inference is unreliable in an ideal setting, then it will certainly be unreliable in a non-ideal one_.  By eliminating measurement errors and abstracting away confounders, computer simulation allows us to create the ideal conditions from which to assess the quality of this inference.  Thus, if the conditions in this model are present in the real world, then we should be very sceptical inferring anything about school performance from student achievement.

## Installation

You can run your own simulation by cloning this repo and building from source ...

    $ git clone git@github.com:davekinkead/school-performance.git
    $ npm install
    $ make paper

In the `paper.coffee.md` file, you can edit the parameters of each simulation, eg ...


    relative_2 = { 
      schools: [{impact: -0.25}, {impact: -0.5}],
      selectivity: 0.5
    }