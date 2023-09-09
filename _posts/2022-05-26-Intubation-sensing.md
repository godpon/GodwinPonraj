---
title:  "Chip-Less Wireless Sensing of Endotracheal Intubation"
mathjax: true
layout: post
categories: media
contribution: Lead Contributer ( <i>Conceptualization</i> | <i>Design</i> | <i>Experimentation</i> | <i>Characterization</i> | <i>Writing</i> )
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
        <img src="/GodwinPonraj/assets/Fig_ETtube_sch.jpg" height = "100%">
      </div>
      <div class="flex-item-text" align="justify" style="padding-right:0px">
        Endotracheal intubation is a common medical practice for patients requiring upper airway management. An important parameter while performing intubation is the depth of insertion of the tube. However, most current solutions rely on vision-based feedback for successfully performing remote intubation. We propose a novel application of chip-less RF sensing technology to identify the intubation tube from the exterior and serve as an additional feedback modality, independent of the visual aid.
      </div>
</div>

<!--more-->
We used printable silver conductive ink to fabricate flexible RF antennas to be deployed on the Endotracheal (ET) intubation tubes. An interrogating antenna, connected to a network analyzer, placed on top of the neck can identify the RF antenna inside the trachea during intubation in real-time. A prototype design was developed and tested with various wireless channel mediums (air, water, phantom models, and duck neck). Seven human subjects were involved in another experiment that used human fingers as a wireless medium between the antennas. Experimental results show that the proposed method can identify the presence of ET tubes by registering a significant change in the return loss magnitude (2.21 dB in phantom model and an average of 1.16 dB in human experiments) across all the mediums. The proposed sensing solution can be used as a viable feedback parameter for robotic control systems that aim to automate intubation with or without visual feedback.

The proposed sensing scheme consists of a reading side and a sensing side. In the sensing side the antenna is mounted on to the ET tube behind the inflatable balloon. Whereas in the reading antenna is fixed at a desired location on the throat region externally. The reading antenna is connected to a Vector Network Analyzer (VNA) which is in turn connected to a PC.
The VNA generates a stimulus signal and monitors the reflected power level. When in vicinity, the sensing antenna absorbs varying levels of power across the frequency spectrum.
The frequency at which the antenna absorbs maximum power from the signal, is known as the resonant frequency.
The objective here is to identify the resonant frequency and track the return loss level. 
Maximum return loss occurs when the distance between the two antennas is minimum that is during concentric alignment of the sensing and transmitting antennas.

<div class="post_container">
      <div class="flex-item-pic">
        <video width="100%" height= "100%" controls>
          <source src="/GodwinPonraj/assets/Vid_ETtube_sensing.mp4" type="video/mp4">
          Your browser does not support mp4 video tag.
        </video>
      </div>
      <div class="flex-item-text" align="justify" style="padding-right:0px">
        Video shows the proposed sensing scheme in a human phantom model. The return loss at resonant frequency marked by the red circle changes and peaks whenever the sensing antenna is the closest to the reading antenna.
      </div>
</div>
<br>
<div style="padding:10px; border-bottom: 1px solid lightgray; border-left: 5px solid darkgray;">
<u>Related Publication:</u><br>
<b><i>G. Ponraj</i></b>, C. Cai, and H. Ren, “Chip-Less Real-time Wireless Sensing of Endotracheal Intubation Tubes by Printing and Mounting Conformable Antenna Tag,” in IEEE Robotics and Automation Letters, vol. 7, no. 2, pp. 2369-2376, April 2022, <a href = "https://ieeexplore.ieee.org/document/9676421/">doi: 10.1109/LRA.2022.3141664</a>.
</div>
