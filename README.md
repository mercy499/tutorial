# Crofting Hybrid Robot

# Introduction
Farmers face difficult in identifying if any kind of disease infects the plants and also adding adequate and type of fertilizers to soil is crucial. Finding the amount of [N-nitrogen, P-phosphorus, K-potassium] levels in soil requires time consuming process of collecting soil sample and taking it to nearest city LAB to get tested there is a requirement for a modern robot which can do both the task of finding the plant disease and also finding the NPK concentration of soil.

## Technologies
Our project is micro-controller based solution for soil testing.
Soil testing sensor is connected to Arduino which provide NPK content of the soil. 
 The development of  system consist of 2 modules :
       1: Training of machine learning module with data sets
       2: Detection of disease 
Training of machine learning module with data sets: The neural machine learning module is created using  python in google collab editor.
For training the module 1000's of images of plant leaves with  disease  are collected and stored in a file. The file is divided into two parts training datasets and testing data sets. training data sets is used to train the machine learning module. It consists 38 classes of plant disease  images labelled respectively. These images will be fed into machine learning module, and trained module is extracted.
DETECTION OF PLANT DISEASE :
The detection of plant disease  starts with the collection of plant leaf image  sample at the farm, the image is then passed into trained neural module for diagnosis.
The trained machine learning module will give output whether the sample image contains any disease and if disease is detected a precaution for that disease will also be displayed.

### Requirements
Software requirements:
 Code Editor : Google collab 
 Language : Python, C++
Hardware requirements:
 Arduino Mega
 GPS Module
 PH Sensor
 Camera
 Motors
 Robot Wheels
 Soil testing 
 Battery (Li-ion) 
 Transmitter and Receiver (Joystick)
These are the software and hardware requirements we used to develop this project

#### Dataset
https://www.kaggle.com/datasets/vipoooool/new-plant-diseases-dataset
Download the dataset from this link and store it in a drive

##### Execution
From Google collab notebook execute the python code stored in .py file,
which will give the disease setection and NPK values.

###### Applications
It can be used to detect plant disease.
It can be used to measure NPK of soil.
It can be used to detect the color of the soil.
It can be used in small and large farm field. 
Can be used in farm to measure soil fertility.  
Can be used to know the kind of crops which can be grown. 

###### References
[1] A Novel Method of Plant Leaf Disease Detection Based on Deep Learning and 
Convolutional Neural Network Xulang Guan.
[2] Deep Neural Networks Based Recognition of Plant Diseases by Leaf Image 
Classification Srdjan Sladojevic,1 Marko Arsenovic,1 Andras Anderla,1 Dubravko 
Culibrk,2 and Darko Stefanovic1.
[3] Transfer Learning Based Plant Diseases Detection Using ResNet50 Ishrat Zahan Mukti, 
Dipayan Biswas.
[4] CNN based Leaf Disease Identification and Remedy Recommendation System Suma 
V R Amog Shetty, Rishab F Tated, Sunku Rohan, Triveni S Pujar.
[5] A Deep CNN Approach for Plant Disease Detection Fatma MARZOUGUI, Mohamed 
ELLEUCH, Monji KHERALLAH.
[6] Plant Leaf Disease Detection and Classification based on CNN with LVQ Algorithm 
Melike Sardogan, Adem Tuncer, Yunus Ozen

###### Conclusion
In this project, a Convolutional Neural Network was constructed to identify plant diseases automatically. Our developed model can distinguish between 38 classes of both healthy leaves and disease affected leaves. The entire method has been narrated specifically. Model performances have been analyzed through comparison with few other transfer learning models along with suitable graphs. With the increasing depth of CNN model, more image data is required for the best generalization of the model. For that reason, after preprocessing the data, we enlarged the dataset through the process of augmentation. Finally, It’s probably due to the nature of the leaves. The images of some species are very close to each other and share very similar shape, color, and texture. So, sometimes it is very hard for networks to correctly predict the true labels. Nowadays, smart mobile devices facilities us in terms of easy access and the flexibility in uses. Mobile camera can be used to capture these leaves of plant. A precise plant diseases detection model implemented in those smart phones will help farmers to recognize the plant diseases in a very short time through a convenient way. Farmers will be able to make decision own self. And, it will have a golden impact on the progress of agriculture.
