# Aplikace modelu neuronové sítě YOLO pro detekci a sledování objektů z perspektivy UAV
Tato práce představuje další způsob využití detekce a následné analýzy objektů z pohledu bezpilotních letounů (UAV). Celý systém využívá jednu kameru, která je vhodně umístěna na UAV pro zachycení scény. Zpracování obrazu a následná detekce objektů pomocí modelu konvoluční neuronové sítě YOLOv4. Model YOLO byl natrénován na naší vlastní datové sadě. Tato tréninková sada byla vytvořena speciálně pro aplikace UAV. Výsledkem této práce je naučený model neuronové sítě YOLO určený pro UAV s ohledem na použitou trénovací sadu.

<p float="center">
  <img src="https://drive.google.com/uc?id=1boxg0Mui2vfPdvQ_nGBF9sQa2gANmjEf" width="200" />
  <img src="https://drive.google.com/uc?id=1t_ioAAK7zLW0CU5xHoStTeEDxtuqg4ho" width="200" />
  <img src="https://drive.google.com/uc?id=1g191w6fDrlVKNChyWkfXK1rAKW5MwzmH" width="200" />
  <img src="https://drive.google.com/uc?id=1f4B0i1wBc1Jk9wVEzQsfuSR-7piq0iwv" width="200" />
</p>

<b>Datovou sadu, skripty a další soubory použité v této práci lze nalézt na:</b></br>
https://drive.google.com/drive/folders/1pCiBqvItr4K8-zJZ3WTG0lvnNh--s22S?usp=sharing

<b>Trénovat model neuronové sítě YOLOv4 s frameworkem darknet lze:</b></br>
<code>sudo path/to/darknet detector train "coco.data" "yolov4-obj.cfg" "yolov4.conv.137" -dont_show -mjpeg_port 8090 -map</code>

<b>Testovat natrénovaný model neuronové sítě YOLOv4 s frameworkem darknet lze:</b></br>
<code>python3 opencv_yolov4_inference_test.py --video=./video/cars.mp4</code>

<b>Výsledky natrénovaného modelu YOLOv4:</b>
<p float="center">
  <img src="https://drive.google.com/uc?id=1dp1jt9ALL_nuU_jnZwyNFSQzIr7gsMcd" width="450" />
</p>

<p float="center">
  <img src="https://drive.google.com/uc?id=1rSnwwOM7-kvNuHolyzvFvrJOlRvSQqER" width="650" />
</p>
