# Multi-Human Face Classifier (ResNet18)

This project used transfer learning with pre trained ResNet18 to classify faces of multiple people.  
It was developed in Google Colab .

---

##  How to Run the AI
1. Upload **dataset_ready.zip** to /content/ in Google Colab.  
2. Run all cells in order inside **MultiHumanClassifier.ipynb**.  
3. The final cell will launch a **Gradio web app** where you can upload a face image and test the classifier.

---

##  Results
- **Final Accuracy:** 74 %  
- **Training Loss :** 0.198 
- **Precision:** 0.73 
- **Recall:** 0.74  

> The model was trained for 5 epochs using transfer learning on ResNet18, with Adam optimizer and CrossEntropyLoss.

---

##  Files


 MultiHumanClassifier.ipynb= Main notebook with all training, evaluation, and demo code 
 dataset_ready.zip = Compressed dataset 
README.md = Project overview and instructions 

---

##  Dataset
Download the dataset :  
 [Google Drive – dataset_ready.zip](https://drive.google.com/file/d/1q23xEeSfhe3famj7bgXc8tLNyuY040im/view?usp=sharing)

Place it inside /content/ before running the notebook.

---

## Model Info
- **Base Model:** ResNet18 pretrained on ImageNet) 
- **Modified:** Final FC layer replaced with num_classes outputs  
- **Optimizer:** Adam (lr = 1e-4)  
- **Loss:** CrossEntropyLoss  
- **Batch Size:** 16  
- **Epochs:** 5  

---

##  Demo
After training completes, the notebook opens a **Gradio web interface**:  
Upload a face which will get top-5 and predicted identities with confidence percentages.  

---

##  Credits
Created by *[Mohammed Abdo]*  
Course: **CAP 4630 – Introduction to Artificial Intelligence**  
Semester: **Fall 2025**


## refernces
- https://www.geeksforgeeks.org/deep-learning/resnet18-from-scratch-using-pytorch/
 the model we used for our project,also used some sample code to help implement the code and model to our project
- https://www.analyticsvidhya.com/blog/2023/12/adam-optimizer/
 Our optimizer that was used in our project
