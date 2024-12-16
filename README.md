Project D10: KAGGLE - PLANT DISEASES
Authors: Liis Siigur, Mia Männi, Robert Sarnet

1. Motivation and goals of the project
Agriculture plays a vital role in sustaining life and supporting economies worldwide. However, plant diseases significantly affect agricultural productivity and food security worldwide by drastically reducing crop yields, causing economic losses, and leading to food shortages. Timely detection of plant diseases is crucial to prevent their spread and minimize losses, however farmers and agricultural professionals often struggle to detect and diagnose diseases early, leading to reduced yields and increased costs. Moreover, small/scale growers and hobby gardeners, who may lack the expertise and resources to identify plant diseases, often find it challenging to manage their gardens effectively when plants exhibit signs of distress.
The primary goal of this project is to develop an image classification model that accurately identifies plant diseases across multiple categories, including different plant species and specific diseases. This model will provide a tool for diagnosing plant diseases, helping farmers, especially individual and small-scale growers, make timely and informed decisions about disease management. The goal is to predict the plant diseases given in the Kaggle dataset with at least 85% accuracy.

2. Guide to the contents of the repository
The folder “IDS_data” contains the data used for training, validation and testing of the models. It has three subfolders “test”, “train” and “valid” with images of the corresponding set. The training and validation folders were downloaded from Kaggle and 10% of each of them was moved to the testing folder. The file “D10_report.pdf” is the report submitted for the homework nr 10.
The repository contains three .ipynb files. The file “IDS_project_model_training.ipynb” contains the code used for training the models used in this project. The trained models are saved and downloaded in this file. The file “IDS_project_model_testing” contains the code for testing the models used in this project. In this notebook, the previously saved models are used. The file “IDS_project_user_interface” contains the user interface for uploading or capturing images and predicting the class with the previously saved models.  When capturing an image from the camera for the first time, the code might have to be run twice, since after the first time, there might be a problem with permission to use camera. 
The model training notebook is connected to the GitHub repository and accesses training, validation and testing data from the repository. The notebook was run in Google Colab, since the use of GPU decreased model training time drastically compared to CPU. The models and label encoders trained in this file are saved in a Google Drive folder (link below), because the model files were too large to be uploaded to GitHub. The user interface notebook is connected to Google Drive, was run in Google Colab and accesses the models and label encoders from Drive. However, the testing notebook was not run in Google Colab, since predicting species first and then disease from the corresponding disease prediction model was not performed in batches, which caused the Google Colab to crash (probably due to too high RAM usage). Instead, the notebook was run on the local computer. 
In order to replicate the same analysis, one must first open the model training notebook in Google Colab or download it to a local computer. Then, the code must be run and models and label encoders saved. 





Google Drive folder: https://drive.google.com/drive/folders/1GbnBAhwdBQBJKpBTAmN5oNxhrZ263RQJ 



Link to saved models and label encoders: https://drive.google.com/drive/u/0/folders/1GbnBAhwdBQBJKpBTAmN5oNxhrZ263RQJ
