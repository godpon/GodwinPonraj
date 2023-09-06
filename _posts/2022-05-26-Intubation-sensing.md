---
title:  "Chip-Less Wireless Sensing of Endotracheal Intubation"
mathjax: true
layout: post
categories: media
---
<style>
  .post_container {
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: space-between;
  flex-wrap: wrap;
}

.flex-item-text {
  flex: 38%;
/*  background-color: darkred;
  color: white; */
  border: 1px solid red;
/*   padding: 5px; */
  padding-top: 0px;
  padding-bottom: 0px;
  justify-content: space-around;
}

/* Main column */
.flex-item-pic {
  flex: 58%;
/*  background-color: darkblue;
  color: white; */
  border: 1px solid blue;
  padding: 5px;
  align-content: space-around;
}
/* Responsive layout - makes a one column layout instead of a two-column layout */
/*@media (max-width: 800px) {
  .flex-item-right, .flex-item-left {
    flex: 100%;
  }*/

@media (max-width: 800px) {
  .post_container {
    flex-direction: column;
  }
}

.text {
  padding-right: 20px;
}
</style>

<div class="post_container">
      <div class="flex-item-pic">
        <img src="/GodwinPonraj/assets/Fig_ETtube_sch.jpg" width = "100%" height = "100%">
      </div>
      <div class="flex-item-text" align="justify">
        Endotrachealintubation is a common medical practice for patients requiring upper airway management. An important parameter while performing intubation is the depth of insertion of the tube. However, most current solutions rely on vision-based feedback for successfully performing remote intubation. We propose a novel application of chip-less RF sensing technology to identify the intubation tube from the exterior and serve as an additional feedback modality, independent of the visual aid.
      </div>
</div>


We used printable silver conductive ink to fabricate flexible RF antennas to be deployed on the Endotracheal (ET) intubation tubes. An interrogating antenna, connected to a network analyzer, placed on top of the neck can identify the RF antenna inside the trachea during intubation in real-time. A prototype design was developed and tested with various wireless channel mediums (air, water, phantom models, and duck neck). Seven human subjects were involved in another experiment that used human fingers as a wireless medium between the antennas. Experimental results show that the proposed method can identify the presence of ET tubes by registering a significant change in the return loss magnitude (2.21 dB in phantom model and an average of 1.16 dB in human experiments) across all the mediums. The proposed sensing solution can be used as a viable feedback parameter for robotic control systems that aim to automate intubation with or without visual feedback.

<div style="background-color: Gainsboro; color: black; padding:10px;">
<u>Related Publication:</u><br>
<b><i>G. Ponraj</i></b>, C. Cai, and H. Ren, “Chip-Less Real-time Wireless Sensing of Endotracheal Intubation Tubes by Printing and Mounting Conformable Antenna Tag,” in IEEE Robotics and Automation Letters, vol. 7, no. 2, pp. 2369-2376, April 2022, <a href = "https://ieeexplore.ieee.org/document/9676421/">doi: 10.1109/LRA.2022.3141664</a>.
</div>
