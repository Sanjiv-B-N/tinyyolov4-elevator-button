# tinyyolov4-elevator-button
## Check Pre-requisites
<p> Before following along on this tutorial refer to this page to check if you have set up your Jetson Nano properly. If not this will lead to a lot of errors in the future steps of this turorial:<br><br>
  https://github.com/Sanjiv-B-N/jetson-nano-setup 
  <br></p>
## Install Darknet
<p> we need darkent to run tinyYOLOv4 on the Jetson Nano. Run the following  on the command line: <br><br>
  git clone https://github.com/AlexeyAB/darknet.git<br>
  cd darknet<br>
  sudo nano Makefile<br><br></p>
  
  <p> Now the makefile opens. Make the following changes to the make:<br><br>
  GPU=1<br>
  CUDNN=1<br>
  OPENCV=1<br><br>
  
  After that save the Makefile and run the following command to install darknet:<br><br>
  make<br><br>
  </p>
  
## Now install weitghts and config file of the retrained tinyYOLOv4

<p> We have trained the tinyYOLOv4 on the Elevator button dataset. I have uploaded the config file and the retrained weights in this github. Download them and place them in your darknet directory. Now run this command to have object detection on the Jetson Nano! run this on the commandline in th darkenet directory:<br><br>
  ./darknet detect cfg/yolov3.cfg yolov3.weights data/image.jpg<br><br>
  
  Here on this line add the correct paths to the weigths the config file and test image and then you'll get the output!</p>
  
  
  
  
  
  
