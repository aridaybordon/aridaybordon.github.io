---
layout:     post
title:      "Predicting chaotic systems (Part 1): Solving the EOM for a double pendulum."
date:       2022-04-12 18:38:00 +0000
tags:       physics
---

## **Introduction**
The double pendulum is one of the most fascinating physical system due to its extremely simplicity and chaotic behaviour. It is a simple system because it consist on two pendulum attached to each other and chaotic because it is extremely sensible to initial conditions. In this post, lagrangian formulation of classical mechanics will be used to obtain the equations of motions (EOM) of the system and a numerical method will be proposed to solve them.

## **Solving the EOM**
A double pendulum is completely described by two degrees of freedom that we will take as the angle of each pendulum with respect the vertical axis, $\theta_1 \text{ and } \theta_2$. In addition, there exist four more free parameters, the mass and the lenght of each pendulum, $m_1\text{, }m_2\text{, }l_1\text{, }l_2$.

With these definitions, we can work up both the total kinetic $T$ and potential energy $V$ of the system.

$$T = \sum_{i=1}^2 \frac{1}{2} m_i v_i^2 = \frac{1}{2} \Big( m_1 l_1 \dot{\theta}_1$$