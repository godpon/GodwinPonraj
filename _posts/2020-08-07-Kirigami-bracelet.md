---
title:  "Kirigami Bracelet to measure Skin Impedance & Classify Hand Gestures"
mathjax: true
layout: post
categories: media
contribution: Lead Contributer ( <i>Conceptualization</i> | <i>Software</i> | <i>Validation</i> | <i>Supervision</i> | <i>Writing</i> )
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

<div class="post_container">
      <div class="flex-item-text" align="justify" style="padding-left:0px">
        The kirigami patterns considered were to realize a “<emph>popping-up</emph>” effect, where a central platform is raised from the base when an extension force is applied along its longitudinal axis. The design was simulated in SolidWorks to understand their stress–strain relationship. The prototype was fabricated using an A4 size paper with eight of the flat platform kirigami structures along its length. The electrodes are made up of PEDOTS: PSS — a flexible, stretchable, and conductive polymer with high ductility. 
      </div>
      <div class="flex-item-pic">
        <img src="/GodwinPonraj/assets/Fig_Kiri_bracelet_solidworks.jpg" width = "100%" height = "100%">
      </div>
</div>

The device is wrapped around the forearm, such that all eight electrodes contact the skin. The data acquisition system consists of a galvanic skin response (GSR) sensor, two 8-channel analog multiplexers, and an Arduino controller. The GSR sensor is used to measure the skin conductivity between two points. The conductivity is measured between all possible combinations of the eight electrodes by the help of two multiplexers each for a lead from the GSR sensor. The resultant 64 data points constitute a single data frame. The dataset collected from each gesture is fed into different machine learning algorithms to compare their performance in classifying the various hand gestures.

<div style="padding:10px; border-bottom: 1px solid lightgray; border-left: 5px solid darkgray;">
<u>Related Publication:</u><br>
<b><i>G. Ponraj</i></b>, X. Z. Wang, K. S. Kumar, and H. Ren, “Comparative Study of Machine Learning Algorithms to Classify Hand Gestures from Deployable and Breathable Kirigami-Based Electrical Impedance Bracelet,” Multimodal Technol. Interact. 2020, vol. 4, no. 3, p. 47, Aug. 2020, <a href="https://www.mdpi.com/791780">doi: 10.3390/MTI4030047</a>.
</div>
