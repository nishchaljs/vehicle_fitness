# vehicle_fitness
The goal of this project is to automate the various steps involved in vehicle fitness tests.  
  
## Technologies Used
We have used technologies such as:
* Object detection 
* Object Localisation
* Pixel per meter and Trianguar Distance Measurement
* OCR  
* Google Translate API
  
## Flask Webpage  
The Flask Webpage can be executed by running the app.ipynb notebook  
The WebPage contains:  
* Login for Normal User and RTO Officer  
* Documents Upload for OCR - RC Book and PUC Certificate  
* Vehicle Registration Plate detection using OCR    
* Tyre Condition estimation - Normal, Worn Out, Cracked etc..  
* Headlights On/Off Detection
* Indicator Blinking Detection    
* Geo-Location  
  
## Car Parts Detection 
Download the weights from drive link and place it in _CarPartsDetectionChallenge-master\Data\Model_Weights_ folder  
Run the first block of code on Test_parts.ipynb for Car Parts detection. It performs MultiClass Object Localisation and detection using the YOLO Architecture to identify the following parts in the car:  
* Wheel  
* Head Lights  
* Door  
* Windshield  
* Rear View-Mirror  
* Glass - Front and Rear  

## Tyre defect Classification  
Run the "Tyre" block of code in the Test_parts.ipynb for executing the Tyre defect classification. It performs Multiclass Image Classificiation with the simple Convolutional Neural Network into 6 different categories:  
* Normal  
* Exposed  
* Tread Wear  
* Linear Air  
* Cracked Tyres  
* Bulges  

## Headlights ON/OFF Classification  
Run the "Headlights" block of code in the Test_parts.ipynb for executing the Headlights On/Off classification. It performs Binary Image Classification with a simple Convolutional Neural Network.  
## Horn detection
Run the horn_pitch_detection.ipynb in the horn_detect folder. The audio file should be in wav format and the path of it should be mentioned in the ipynb file.For testing the 2 wav files in the horn_detect folder can be used.Here the algorithms AMDF(Average Magnitude Difference Function) and CAMDF(circular average magnitude difference function)are used.
  
## OCR for Vehicle Registartion Plate detection and Document Verification  
Refer to the OCR.ipynb for the OCR Tesseract code implementation. The details Extracted from the documents are:  
* Vehicle Plate Registration Number  
* Engine Number and Chassis Number
* Manufacturing Date of Vehicle and its Age
* Owner Information  
