---
title:  "Sensor Fusion of Leap Motion Controller and Flex Sensors for Human Finger Tracking"
mathjax: true
layout: post
categories: media
contribution: Lead Contributer ( <i>Conceptualization</i> | <i>Algorithm</i> | <i>Software</i> | <i>Experimentation</i> | <i>Writing</i> )
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
        <img src="/GodwinPonraj/assets/Fig_Sensor_fusion.jpg" height = "100%">
      </div>
      <div class="flex-item-text" align="justify" style="padding-right:0px">
        A novel strategy for tracking the fingertips of a human hand by combining two distinct sensors - Leap motion controller (vision based tracking) and Flex sensors (non-vision based tracking). We describe the theory and implementation of a sensor fusion algorithm using Kalman filter, and present the experimental results that shows the proposed method having an edge in minimizing the effects of occlusion in a visual based tracking method. Increased accuracy and reliable finger-tip tracking was achieved with <5% error.
      </div>
</div>

<!--more-->
Tracking the position, orientation, and articulation of human hands has a variety of applications including gesture recognition, robotics, medicine and health care, design and manufacturing, and art and entertainment across multiple domains. Out of the various tracking methods, vision-based tracking is an efficient and widely used method. Several devices have been developed by researchers and engineers to track objects using vision. The leap motion (LM) controller is one such device. However, visual tracking is an equally complex and challenging task due to several factors like higher dimensional data from hand motion, higher speed of operation, and self-occlusion. The proposed method in this work has proven to mitigate the self-occlusion and improve the accuracy of leap motion tracking by augmenting it with a non-vision based sensor attached to a glove.

Leap Motion controller (_Leap motion Inc._) is a motion sensor specifically designed to track human hands. It uses two infrared cameras (sensors) and three infrared LEDs. The sensors have about 150 degrees field of view and an effective range of approximately 0.03 to 0.06 meters above the device. The major drawback of Leap motion controller is the problem of self-occlusion. One hand covering another, movements of the fingers when the hand is upside down or sideways when multiple fingers curl or come together are some cases where the problem of self-occlusion occurs. 

Flex sensors are analog input devices whose resistance changes when they are bent by external force. They can be used to detect the flexion/extension of a Human finger by mounting them above the fingers. In this work, three flex sensors were stitched along the outer-dorsal surface of a glove, one each for the thumb, index and middle fingers. This method is relatively cheaper than other glove based tracking methods using accelerometers or mechanical attachments, and was sufficient to provide the basic data to support the implementation of the proposed sensor fusion technique together with the vision data from the leap motion controller. The position and velocity vectors from the leap motion controller and the position estimate from the flex sensors based on the kinematic model of the human hand, were taken as the outputs of a state-space model of a linear time-invariant system. Applying kalman filter to this state space model, the a-posteriori covariance estimation will generate the position vectors by combining data from both the leap motion controller and the flex sensor glove. 

To analyze the effectiveness of the proposed method, finger tip positions of index, middle and thumb fingers during selected hand postures were measured both from LM alone and from the sensor fusion method. The postures were selected so that the problem of self-occlusion is evident during LM tracking. Initially, the posture was kept facing the LM and later, the hand was re-oriented to face away from the LM. Error was calculated as percentage deviation with respect to the ground truth measured by the electromagnetic trackers. Figure below shows the comparison of root mean square (RMS) errors of the proposed sensor fusion method with those of LM alone for one of the finger postures (parallel extension). 

<div class="post_container">
      <div class="flex-item-pic">
        <img src="/GodwinPonraj/assets/Fig_par_ext.jpg" height = "100%">
      </div>
      <div class="flex-item-text" align="justify" style="padding-right:0px">
        The Parallel extension denotes the extension of the thumb in parallel to the other four fingers. The thumb lies in a position between abduction and adduction. When the orientation is reversed, the thumb is entirely occluded by the palm. The proposed method is able to reduce the error percentage of thumb position to <2%. A slight improvement in position of the other two fingers can also be observed. 
      </div>
</div>

The proposed sensor fusion method has been proved to reduce the error in occluded scenarios thus increasing the overall accuracy and reliability of the device. It can be used in applications that require remote control of robotic manipulators accurately. A sample was demonstrated using a soft robotic actuators. Future work can be done to extend this method to incorporate joint angle and orientation data of each bone from the LM and with the help of multiple flex sensors to further reduce the error percentage.

<div style="padding:10px; border-bottom: 1px solid lightgray; border-left: 5px solid darkgray;">
<u>Related Publications:</u><br>
<b><i>G. Ponraj</i></b> and H. Ren, “Sensor Fusion of Leap Motion Controller and Flex Sensors Using Kalman Filter for Human Finger Tracking,” IEEE Sens. J., vol. 18, no. 5, pp. 2042–2049, Mar. 2018, <a href="http://ieeexplore.ieee.org/document/8248750/">doi: 10.1109/JSEN.2018.2790801</a>.
</div>
