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

RFID works based on the modulation of a reflected signal at a tag’s resonant frequency ($$𝑓_{𝑟𝑒𝑠}$$). The transmission strength and resonant frequency of RFIDs are also affected by the (inductive) coupling coefficient, k, and the Quality factor, Q, which depends on their basic electrical parameters such as resistance, capacitance, and inductance. Thus tuning is done by adjusting the capacitance (C), or the inductance, (L) according to the formulae for resonant frequency and quality factor:

$$f_{res} = \frac{1}{2 \pi \sqrt{LC} } ; \qquad 𝑄 = \frac{1}{𝑅}\sqrt\frac{𝐿}{𝐶} $$

This property is exploited to introduce various sensing modalities into the antenna. A change in the physical property is transduced into a change in the sensor’s resistance or capacitance. Together with the antenna, this change is reflected as a change in transmission power and frequency.

## Sensing Prototypes

<div class="post_container">
      <div class="flex-item-pic">
        <img src="/GodwinPonraj/assets/Fig_RFID_sensors.jpg" width = "100%" height = "100%">
      </div>
      <div class="flex-item-text" align="justify" style="padding-right:0px">
        Four sensor prototypes were made, designed to respond to different mechanical stimuli - a capacitance-based tactile sensor, an inductance based compression sensor, an extension sensor and a bend sensor. The fabricated capacitive sensor prototype has a parallel plate design, where both the conductive plates lie on a single plane, and an out-of-plane capacitive coupling occurs between them via the common dielectric medium. 
      </div>
</div>

When a normal force is applied the dielectric medium is deformed, disrupting the electric field distribution and capacitive coupling between the conductive traces. The compression sensor consists of a circular spiral antenna with cuts introduced between each turn. This kirigami-inspired design allows the spiral to expand in a direction normal to its surface. As the pyramid is compressed, the vertical distance between the individual antenna loops decreases, increasing the coil trace’s mutual inductance, which changes the antenna’s resonant frequency. The extension sensor design uses a round tag with spiral antenna design and a long strip extention at the end. The straight conductor was folded in alternative mountain and valley folds to form the sensing element. Similarly, a bend sensor was fabricated using a squareslinky kirigami design as the basis. An L-shaped substrate is folded over itself in alternating mountain and valley folds.

<div class="post_container">
      <div class="flex-item-text" align="justify" style="padding-left:0px">
        Capacitive tactile sensors can be used as contact identification devices or force limiting devices in robotic applications. Due to the PET substrate's flexible nature, the sensors can be designed to be compliant with the robot’s morphology. Advanced tactile sensor applications such as closed-loop control for robotic object grasping tasks, object orientation estimation and slip estimation. It could also be made wireless by integrating simple antenna coil trace designs and functional sensor traces.
      </div>
  <div class="flex-item-pic">
        <video width="100%" height= "100%" controls>
          <source src="/GodwinPonraj/assets/Vid_RFID_sensing.mp4" type="video/mp4">
          Your browser does not support mp4 video tag.
        </video>
      </div>
</div>
The compression sensors have the potential to be used to identify specific user interactions. This kirigami-based device can be used as a multi-step input device, where the user can change the intensity or rate of control. For example, the speed of rotation of a motor or the flow rate in a pneumatic pump can be controlled by changing the sensor’s compression level. The device could also be used in contact identification like the tactile sensors. The extension and bend sensors can be used to sense and monitor robotic and industrial mechanisms such as a slider crank mechanism or a revolute joint movement. 

<br>

<div style="padding:10px; border-bottom: 1px solid lightgray; border-left: 5px solid darkgray;">
<u>Related Publication:</u><br>
<b><i>G. Ponraj</i></b>, W. L. Yeo, K. S. Kumar, M. S. Kalairaj, C. J. Cai and H. Ren, "Chip-Less Wireless Sensing of Kirigami Structural Morphing Under Various Mechanical Stimuli Using Home-Based Ink-Jet Printable Materials," 2021 IEEE International Conference on Robotics and Automation (ICRA), Xi'an, China, 2021, pp. 11400-11407, <a href="https://ieeexplore.ieee.org/document/9561945">doi: 10.1109/ICRA48506.2021.9561945</a>.
</div>
