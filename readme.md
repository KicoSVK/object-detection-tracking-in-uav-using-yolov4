# Aplikace modelu neuronové sítě YOLO pro detekci a sledování objektů z perspektivy UAV
Tato práce představuje další způsob využití detekce a následné analýzy objektů z pohledu bezpilotních letounů (UAV). Celý systém využívá jednu kameru, která je vhodně umístěna na UAV pro zachycení scény. Zpracování obrazu a následná detekce objektů pomocí modelu konvoluční neuronové sítě YOLOv4. Model YOLO byl natrénován na naší vlastní datové sadě. Tato tréninková sada byla vytvořena speciálně pro aplikace UAV. Výsledkem této práce je naučený model neuronové sítě YOLO určený pro UAV s ohledem na použitou trénovací sadu.

<p float="center">
  <img src="https://drive.google.com/uc?id=1BHYKVwZjPXDLr79f-iMFqag8bND_PbhK" width="200" />
  <img src="https://drive.google.com/uc?id=16S1AyNxcbtK8W0tqslKpSOrbu-wxosyA" width="200" />
  <img src="https://drive.google.com/uc?id=1AlfS5QZ-hxuejowRljwp6be9Ej8JqAN0" width="200" />
  <img src="https://drive.google.com/uc?id=16rHmn-riswi_pw3NGHB-II0hkqAtQBBD" width="200" />
</p>

<b>Datovou sadu, skripty a další soubory použité v této práci lze nalézt na:</b></br>
https://drive.google.com/drive/folders/16-P7WJXk4s_M7V-P9I_9HOSBaXcYndMZ?usp=share_link

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
