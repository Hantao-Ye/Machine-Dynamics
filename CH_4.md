# Lecture_4

[TOC]

## Introduction

A **cam** is a specially shaped piece of metal arranged to move a follower in a controls fashion.

A **follower** is a link or linkage train that is

### Benefits of Cams

- Function Generation
- A degenerate form of a pure **fourbar linkage (oscillation)** or **fourbar slider-crank (translation)**
- Effective link length could **change** during the motion
- Easier to generate output function than a linkage
- More expensive to make than a linkage

## 8.1 Cam Terminology

### Classifications of Cam-follower Systems

#### Type of Follower Motion

- translating
  <div align = center><img src ="./assets/CH_4_Figure_2.png"></div>
- rotating
  <div align = center><img src ="./assets/CH_4_Figure_1.png"></div>

#### Type of Cam

- radial cam _(the figures above are all radical cams)_

  open radical cams are also called plate cams
- axial cam

  also called a face cam if open(force closed) and a cylindrical or barrel cam if grooved or ribbed(formed-closed)
  <div align = center><img src ="./assets/CH_4_Figure_5.png"></div>

- three-dimensional cam
  <div align =center><img src ="./assets/CH_4_Figure_6.png"></div>

#### Type of Joint Closure

- force-closed

  requires **an external force** be applied to the joint in order to keep cam and follower physically in contact

  <div align = center><img src ="./assets/CH_4_Figure_1.png"></div>
  <div align = center><img src ="./assets/CH_4_Figure_2.png"></div>

- form closed

  **closes the joint by geometry**

  <div align = center><img src = "./assets/CH_4_Figure_3.png"></div>

#### Type of Follower

- curved (mushroom)
- flat
- rolling
- sliding
  <div align = center><img src ="./assets/CH_4_Figure_4.png"></div>

#### Type of Motion Constraints

- critical extreme position

  - end points of motion are critical
  - path between endpoints is not critical

- critical path motion
  - the path between endpoints is critical
  - displacements, velocities, etc. may be specified
  - endpoints usually also critical
#### Type of Cam Motion Programs

- rise-fall
- rise-fall-dwell
- rise-dwell-fall-dwell

_dwell_: at zero displacement for 90 degrees (low dwell)

## 8.2 S V A J Diagrams

$$
\theta = \omega t
$$

<div align =center><img src = "./assets/CH_4_Figure_7.png"></div>

## 8.3 Double-Dwell Cam Design Choosing S V A J Functions

### The Fundamental Law of Cam Design

**Thw cam function must be continuous through the first and second derivatives of displacement across the entire interval**

_The jerk function must be finite across the entire interval_

### Simple Harmonic Motion (SHM)

$$
\begin{aligned}
    s &= \frac{h}{2}[1-\cos{(\pi \frac{\theta}{\beta})}]\\[2ex]
    v &= \frac{\pi}{\beta}\frac{h}{2}\sin{(\pi \frac{\theta}{\beta})}\\[2ex]
    a &= \frac{\pi^2}{\beta^2}\frac{h}{2}\cos{(\pi\frac{\theta}{\beta})}\\[2ex]
    j &= -\frac{\pi^3}{\beta^3}\frac{h}{2}\sin{(\pi\frac{\theta}{\beta})}
\end{aligned}
$$

<div align = right><img height = 400 src = "./assets/CH_4_Figure_8.png"></div>

- Acceleration discontinuous
- Jerk is infinite

### Cycloidal Displacement

$$
\begin{aligned}
  s &= \frac{h}{\beta}\theta - \frac{h}{2\pi}\sin{(\frac{2\pi\theta}{\beta})}\\[2ex]
  v &= \frac{h}{\beta}(1-\cos(\frac{2\pi\theta}{\beta}))\\[2ex]
  a &= \frac{2\pi h}{\beta^2}\sin(\frac{2\pi \theta}{\beta})\\[2ex]
  j &= \frac{h(2\pi)^2}{\beta^3}\cos(\frac{2\pi \theta}{\beta})
\end{aligned}
$$

<div align = right><img height = 400 src = "./assets/CH_4_Figure_9.png"></div>

- valid cam design
- acceleration and velocity are higher than other functions
- one may seek to cut off the acceleration

### Combined Functions

cut a sine wave into three pieced and recombine them with a square wave

<div align = center><img src = "./assets/CH_4_Figure_10.png"></div>

- lowest magnitude of peak acceleration of standard cam functions

### Polynomial Functions

