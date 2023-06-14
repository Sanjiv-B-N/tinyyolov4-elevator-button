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
  
  
  
  
  
  
