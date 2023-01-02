# Detekcija vozila koristeći OpenCV i Python

OpenCV `dnn` module supports running inference on pre-trained deep learning models from popular frameworks like Caffe, Torch and TensorFlow. 
 
 ## Potrebne biblioteke
  * opencv
  * numpy
  
`pip install numpy opencv-python`

 ## YOLO (You Only Look Once)

 Potrebno je downloadovati pretrenirani YOLO v3 weights file sa ovog linka [link](https://pjreddie.com/media/files/yolov3.weights) i postaviti ga u trenutni direktorij ili ga je moguće direktno downloadovati u trenutni direktorij kroz terminal koristeći 
 
 `$ wget https://pjreddie.com/media/files/yolov3.weights`
 
 Sliku nad kojom će se primijeniti detekcija vozila potrebno je smjestiti u folder `images`. Pod uslovom da su svi ostali fajlovi u trenutnom direktoriju, naredba ispod će primijeniti detekciju vozila na ulaznu sliku `test.jpg`
 
 `$ python yolo_opencv.py --image ./images/test.jpg --config yolov3.cfg --weights yolov3.weights --classes yolov3.txt`
 
 **Način pozivanja komande** 
 
 _$ python yolo_opencv.py --image /path/do/ulazne/slike --config /path/do/config/fajla --weights /path/to/weights/file --classes /path/do/classes/filea_
 
 
 ### primjer izlaza :
 ![](vehicle-detection.jpg)
 