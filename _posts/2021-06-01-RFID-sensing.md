---
title:  "Chip-Less Wireless Sensing with Kirigami using Ink-Jet Printable Materials"
mathjax: true
layout: post
categories: media
contribution: Lead Contributer ( <i>Conceptualization</i> | <i>Fabrication</i> | <i>Characterization</i> | <i>Writing</i> )
---
<style>
  .post_container {
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: space-between;
  flex-wrap: wrap;
}

/* Set padding-left or padding-right equal to 0 in main code */
.flex-item-text {
  flex: 35%;
/*   border: 1px solid blue; */
  padding-left:1em;
  padding-right:1em;
  justify-content: space-around;
}

.flex-item-pic {
  flex: 58%;
/*   border: 1px solid blue; */
  padding: 5px;
  align-content: space-around;
}

/* Responsive layout - makes a one column layout instead of a two-column layout */
@media (max-width: 800px) {
  .post_container {
    flex-direction: column;
  }
  .flex-item-text{
    padding: 0px;
  }
  .flex-item-pic{
    max-width: 90%;
  }
}

</style>

<div class="post_container">
      <div class="flex-item-pic">
        <img src="/GodwinPonraj/assets/Fig_RFID_printing.jpg" width = "100%" height = "100%">
      </div>
      <div class="flex-item-text" align="justify" style="padding-right:0px">
        The feasibility of using chip-based RFID designs as wireless sensor tags open a wide range of application possibilities in the field of robotics. However, multi-step lithography manufacturing and/or MEMS techniques are often required for the industrial-grade fabrication of such sensors. In this paper, we present a simple, home-based, two-step fabrication process to produce chipless RF-based wireless sensors.
      </div>
</div>

<!--more-->
We use an office-based inkjet printer to produce the antenna traces using silver conductive ink. Kirigami-inspired designs are used to produce four sensors responsive to various mechanical stimuli commonly used for DIY robotic projects (contact, compression, extension, and bend). We demonstrate sensing and wireless transmission of the detected mechanical stimuli through the proposed chipless sensor tags with reliable consistency. The tags can be replicated quickly with the inkjet-printing method. This paper also contains analyses on the effects of varying the dimensions and electrical parameters of the tags. The developed antennas in this work can be used as wireless mechano-responsive sensors for robotic applications.

RFID works based on the modulation of a reflected signal at a tag’s resonant frequency ($$𝑓_{𝑟𝑒𝑠}$$). This tuning is done by adjusting the capacitance (C), or the inductance, (L) according to the resonant frequency formula:

<math>
$𝑓_{𝑟𝑒𝑠} = <mfrac>
  1
  2{\pi}<sqrt>𝐿𝐶</sqrt>}$
</mfrac>
</math>

$$f_{res} = \frac{1}{2 \pi \sqrt{LC} }$$

The transmission strength and resonant frequency of RFIDs are affected by the (inductive) coupling coefficient, k, and the Quality factor, Q, which depends on their basic electrical parameters such as resistance, capacitance, and inductance.
$$𝑄 = \frac{1}{𝑅}\sqrt\frac{𝐿}{𝐶}$$
This property is exploited to introduce various sensing modalities into the antenna. A change in the physical property is transduced into a change in the sensor’s resistance or capacitance. When connected to an antenna, this change is reflected as a change in transmission power and frequency

## MathJax

$$ e^{i\theta}=\cos(\theta)+i\sin(\theta) $$

$$ \frac{\mathrm{d}}{\mathrm{d}t} \left ( \frac{\partial L}{\partial \dot{q}} \right ) = \frac{\partial L}{\partial q} $$

$$ i\hbar\frac{\partial}{\partial t} \Psi(\mathbf{r},t) = \left [ \frac{-\hbar^2}{2\mu}\nabla^2 + V(\mathbf{r},t)\right ] \Psi(\mathbf{r},t) $$

<div style="padding:10px; border-bottom: 1px solid lightgray; border-left: 5px solid darkgray;">
<u>Related Publication:</u><br>
<b><i>G. Ponraj</i></b>, W. L. Yeo, K. S. Kumar, M. S. Kalairaj, C. J. Cai and H. Ren, "Chip-Less Wireless Sensing of Kirigami Structural Morphing Under Various Mechanical Stimuli Using Home-Based Ink-Jet Printable Materials," 2021 IEEE International Conference on Robotics and Automation (ICRA), Xi'an, China, 2021, pp. 11400-11407, <a href="https://ieeexplore.ieee.org/document/9561945">doi: 10.1109/ICRA48506.2021.9561945</a>.
</div>
