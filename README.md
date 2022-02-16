<h1> Realtime Object Detection using YOLOv4</h1>

### **Description**
- Objective: To recognize the shoe part in real-time and determine the process of the part.    
- POC(Proof of Concept): Recognize the swoosh of Nike shoes and distinguish how to assemble the parts.    


### **Process**     
**1. Data Preparation**     

    1.1 Data Collection     
    - I collected Nike shoes images using Google.(Data Crawling)    

    1.2 Data Annotation     
    - Data needs to be annotated according to YOLO Format.     
    - We manually label the swoosh part of the shoes with a square box using LabelImg Tool(Reference).    
    - Annotated datasets must have images and coordinates text files.     
    - According to the swoosh process, the annotation was different, and the process labeling was assisted by experts.    
    (In this repo, Data Preparation Part isn't contain)    


**2. Modeling**     

    2.1 Make YOLO Configuration("1. YOLOv4-Generate YOLO Configurations.ipynb")    
    - In order to implement YOLO, 1) weight file, 2) configuration file, 3) label classification file (process classification) is required.    
    - You can create it by using the above Jumpyter notebook file, and I used Google Colab to run the code for about 10 hours.    


**3. Real-time demo**     

    3.1 Real-time Detection Demo Using YOLO Configuration(2. YOLOv4-Swoosh Real-time Classifier.ipynb")    
    - It classifies object detection and process in real-time using above code.    
    ![Demo](https://user-images.githubusercontent.com/55779934/154224123-e760cd14-f43c-4407-a706-2fd17ab1b2c0.gif)    

#### Reference    
- LabelImg: https://byeon-sg.tistory.com/entry/labelImg%EC%82%AC%EC%9A%A9%ED%95%B4%EC%84%9C-yolo-%EC%9D%B4%EB%AF%B8%EC%A7%80-%EB%9D%BC%EB%B2%A8%EB%A7%81%ED%95%98%EA%B8%B0, https://iagreebut.tistory.com/92     
- YOLOv4: https://github.com/AlexeyAB/darknet 
