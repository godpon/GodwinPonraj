---
title:  "Kirigami Bracelet to measure Skin Impedance & Classify Hand Gestures"
mathjax: true
layout: post
categories: media
contribution: Lead Contributer ( <i>Conceptualisation</i> | <i>Software</i> | <i>Validation</i> | <i>Supervision</i> | <i>Writing</i> )
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
        <img src="/GodwinPonraj/assets/Fig_Kiri_bracelet.jpg" width = "100%" height = "100%">
      </div>
      <div class="flex-item-text" align="justify" style="padding-right:0px">
        Wearable devices are gaining recognition for their use as a biosensor platform. Electrical impedance tomography (EIT) is one of the sensing techniques that utilizes wearable sensors as its primary data acquisition system. It measures the impedance or resistance at the peripheral (skin) level and calculates the conductivity distribution. Howvever, modern-day EIT devices are still costly and bulky. We propose a novel low-cost kirigami-based wearable device that has soft PEDOT: PSS electrodes for sensing skin impedances.
      </div>
</div>

<!--more-->
Simulation results show that the proposed kirigami structure for the bracelet has a large deformation during actuation while experiencing relatively lower stress. The paper also presents a comparative study on a few machine learning algorithms to classify hand gestures, based on the measured skin impedance. The best classification accuracy (91.49%) was observed from the quadratic support vector machine (SVM) algorithm with 48 principal components.

<div style="border-left: 5px solid darkgray; padding:10px;">
<u>Related Publication:</u><br>
<b><i>G. Ponraj</i></b>, X. Z. Wang, K. S. Kumar, and H. Ren, “Comparative Study of Machine Learning Algorithms to Classify Hand Gestures from Deployable and Breathable Kirigami-Based Electrical Impedance Bracelet,” Multimodal Technol. Interact. 2020, vol. 4, no. 3, p. 47, Aug. 2020, <a href="https://www.mdpi.com/791780">doi: 10.3390/MTI4030047</a>.
</div>
