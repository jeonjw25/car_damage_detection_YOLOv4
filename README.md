# car_damage_detection_YOLOv4 

<br/>
<br/>

## Introduction  

Implementing algorithm which can detect car damage parts using YOLO_v4.  
We can detect the following damages by the parts below.   

<br/>  

damages: scratch, collision  
car parts: front_door, back_door, hood, bumper, rear, fender  

<br/> 
<br/>

## Member
| 😁 | NAME | Introduction |
|------|------|--------|
| ![JongWonJeon](https://user-images.githubusercontent.com/54730375/123045448-e6795a80-d435-11eb-9f87-e20f79e5a43c.PNG) |   [전종원](https://github.com/jeonjw25/)  |  HUFS/ Information Communication Engineering/ Senier  |
| ![HyoSeopLee](https://user-images.githubusercontent.com/64147276/142341485-296e4a89-1a3c-4259-a99b-4e6b4a5cda01.png)  |   [이효섭](https://github.com/leehyoseop) |  HUFS/ Information Communication Engineering/ Senier  |

<br/> 
<br/>

## environment
ubuntu 18.04  
opencv 4.2.0  
CUDA 10.1  
CUDnn 10.1  
GTX-1080Ti x2  

<br/>  
<br/>

## Flow graph  
![image](https://user-images.githubusercontent.com/54730375/142163737-8b2d1749-7ef0-4ece-b675-908d123e9a42.png)  

<br/>  
<br/>

## Quick Apply

1. Put obj.data, obj.names, train.txt, img folder into opencv/opencv-4.2.0/build/darknet/data/  
2. Put yolov4.cfg into opencv/opencv-4.2.0/build/darknet/cfg/  
3. Put yolov4_final.weights into opencv/opencv-4.2.0/build/darknet/backup/  
4. Open the terminal from opencv/opencv-4.2.0/build/darknet/  
5. Input the test command  
```
sudo ./darknet detector test data/obj.data cfg/yolov4.cfg backup/yolov4_final.weights [test img path] -thresh 0.1
```
6. Check the result.

<br/>  
<br/>  

## Results samples

![image](https://user-images.githubusercontent.com/54730375/142167533-60511491-dada-40db-b6a3-bf244d01f0f0.png)  

![image](https://user-images.githubusercontent.com/54730375/142168211-d903e2ba-e43a-4fbc-8808-6b4c4f6e1785.png)  

![image](https://user-images.githubusercontent.com/54730375/142168745-8f34a986-0b6a-4667-be95-346b1e1b5a74.png)  
