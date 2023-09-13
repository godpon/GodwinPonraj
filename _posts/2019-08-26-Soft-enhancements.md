---
title:  "Active Contact Enhancements & Piezoresistive Tactile Array for Robotic Grippers"
mathjax: true
layout: post
categories: media
contribution: Lead Contributer ( <i>Conceptualization</i> | <i>Design</i> | <i>Methodology</i> | <i>Experimentation</i> | <i>Investigation</i> | <i>Writing</i> )
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
<!--
<div align="right" style="margin-top: 0px; padding-top: 0px;">
  Contribution: Lead (Conceptualisation | Design | Experimentation | Characterisation | Writing)
</div>
-->
<div class="post_container">
      <div class="flex-item-pic">
        <img src="/GodwinPonraj/assets/Fig_Soft_enhans.jpg" height = "100%">
      </div>
      <div class="flex-item-text" align="justify" style="padding-right:0px">
<!--         In any interaction of the robot with its surroundings, it is important to establish proper contact with the object to ensure complete control over its manipulation.   -->
        The sense of touch and perception play a vital role to close the feedback loop of contact modulations. This work discusses the design and development of a novel hybrid sensorized soft-matter structure which has active contact modulation capabilities to ensure better and firm contact in rigid robotic grippers. An integrated multi-taxel piezoresistive tactile sensor which can confer to both rigid and soft surfaces easily was developed as a feedback device.
      </div>
</div>

<!--more-->
The proposed soft enhancement was developed for a rigid tendon driven modular gripper. The gripper has five fingers like a Human hand and each finger has two links and one degree of freedom (DOF). The soft layers are made of a soft yet strong and stretchable material-EcoFlex<sup>TM</sup> 00-30 (Smooth-On, Inc). The soft layers comprise alternative inflation and suction modules which can be pneumatically actuated by vacuum pumps controlling their positive and negative pressure respectively. The suction module is used to enhance the grip and the inflation module is used for increasing the contact area between the hand and the object. 

A 4x4 multi-taxel tactile sensor was custom designed and fabricated to go along with the proposed soft enhancement. It comprises a piezoresistive fabric layer sandwiched between two conductive layers.The conductive layers are realized using flexible PCBs with copper traces. Each layer has four traces of width 2 mm each separated by 1 mm gap. The top and bottom conductive layers are arranged orthogonally to each other such that each overlapping region forms a single tactile sensing element (taxel) of dimension 2 mm x 2 mm. The electrical equivalent of a single taxel is a variable resistor. When an external force is applied to the taxel, the resistance of the piezoresistive fabric decreases at that point which will be reflected across the corresponding conductive traces. 

To demonstrate the superiority of the soft enhancement structure, the robotic gripper was tested in an object handling experiment. The gripper was controlled via the servo motors attached to the tendons. The task is to pick up an egg from a foam tray and place it back in another location. A rigid gripper without soft enhancement structure will fail at this task, because of the smooth curvature and slippery nature of the egg's surface. The rigid hand surface is not able to provide the necessary friction to hold the egg firmly. One can arguably try to increase the grip force from the gripper. However, the egg being a delicate object will break easily from excessive force.

<div class="post_container">
      <div class="flex-item-pic">
        <video width="100%" height= "100%" controls>
          <source src="/GodwinPonraj/assets/Vid_Egg_handling.mp4" type="video/mp4">
          Your browser does not support mp4 video.
        </video>
      </div>
      <div class="flex-item-text" align="justify" style="padding-right:0px">
        The same task was repeated by the same gripper after equipping the thumb and the index fingers with the proposed soft enhancement structures. Once the hand makes firm contact with the egg, the suction module is actuated to increase the grip strength by creating a vacuum between the hand and the egg. The embedded tactile sensor was used to monitor the force exerted during the grip. 
      </div>
</div>

Due to the presence of soft layers, the gripper was able to handle delicate slippery surface of the egg with a firm grip without transmitting the full force from the rigid hand beneath.

<div style="padding:10px; border-bottom: 1px solid lightgray; border-left: 5px solid darkgray;">
<u>Related Publications:</u><br>
<ol>
<li><b><i>G. Ponraj</i></b>, A. V. Prituja, C. Li, A. Bamotra, G. Zhu, K. Senthil Kumar, N. V. Thakor, A. B. Soares, and H. Ren, “Active contact enhancements with stretchable soft layers and piezoresistive tactile array for robotic grippers∗,” in IEEE International Conference on Automation Science and Engineering, 2019, vol. 2019-Augus, pp. 1808–1813, <a href="https://doi.org/10.1109/COASE.2019.8842882">doi: 10.1109/COASE.2019.8842882</a>.</li>

<li><b><i>G. Ponraj</i></b>, A. V. Prituja, C. Li, G. Zhu, N. V. Thakor, and H. Ren, “Pinch grasp and suction for delicate object manipulations using modular anthropomorphic robotic gripper with soft layer enhancements,” Robotics, vol. 8, no. 3, p. 67, Aug. 2019, <a href="https://www.mdpi.com/2218-6581/8/3/67">doi: 10.3390/robotics8030067</a>.</li>
</ol>
</div>
