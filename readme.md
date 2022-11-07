# Object Detection in Unmanned Aerial Vehicle Camera Stream Using Deep Neural Network
This work represents another way of using the detection and subsequent analysis of objects from Unmanned Aerial Vehicle (UAV) perspective. The whole system uses one camera, which is suitably positioned on the UAV to capture the scene. Image processing and subsequent object detection using the YOLOv4 convolutional neural network model. The YOLO model was trained on our own dataset. This training set was created specifically for UAV applications. The result of this work is a learned YOLO neural network model designed for UAVs with regard to the used training set.

<p float="center">
  <img src="https://drive.google.com/uc?id=1boxg0Mui2vfPdvQ_nGBF9sQa2gANmjEf" width="200" />
  <img src="https://drive.google.com/uc?id=1t_ioAAK7zLW0CU5xHoStTeEDxtuqg4ho" width="200" />
  <img src="https://drive.google.com/uc?id=1g191w6fDrlVKNChyWkfXK1rAKW5MwzmH" width="200" />
  <img src="https://drive.google.com/uc?id=1f4B0i1wBc1Jk9wVEzQsfuSR-7piq0iwv" width="200" />
</p>

<b>The dataset, scripts and other files used in this work can be found at:</b></br>
https://drive.google.com/drive/folders/1pCiBqvItr4K8-zJZ3WTG0lvnNh--s22S?usp=sharing

<b>To start training neural network model YOLOv4 with framework darknet:</b></br>
<code>sudo path/to/darknet detector train "coco.data" "yolov4-obj.cfg" "yolov4.conv.137" -dont_show -mjpeg_port 8090 -map</code>

<b>To start testing inference of learned neural network model YOLOv4:</b></br>
<code>python3 opencv_yolov4_inference_test.py --video=./video/cars.mp4</code>

<b>Model training results:</b>
<p float="center">
  <img src="https://drive.google.com/uc?id=1dp1jt9ALL_nuU_jnZwyNFSQzIr7gsMcd" width="450" />
</p>

<p float="center">
  <img src="https://drive.google.com/uc?id=1rSnwwOM7-kvNuHolyzvFvrJOlRvSQqER" width="650" />
</p>
