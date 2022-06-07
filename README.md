                                              LANGUAGE IDENTIFICATION
 
 Problem Statement -
 
 In this project we will doing language identification over six international language i.e English,German,French,Espanol,Chinese and Russian.Here the user need to give
 recording of the specific language as input and finally the input language will be predicted.
 
 Description Overview -
 
 Language Recognization is an important tasks in the field of Natural Language Processing.Here the user will provide speech recording of the specific language and
 then using deep learning approaches we will try to predict the spoken input language
 
 
 Technology Used -
 
 Python 3.6,Keras 2.2.4 using Tensorflow GPU 1.14.0 CUDA 10 with CuDNN10
 
 Installation of the Project -
 
 The installation of the project is easy.Please do follow the steps to create a virtual environment(good pratice while creating a new project) and then install the    necessary packages in the environment
 
 In PyCharm it's easy
 
 STEPS:-
 1. Create a New Project 
 2. Navigate to the directory of the project
 3. Select the option to create a new virtual environment using conda with python 3.6
 4. Finally create the project using used resources
 5. After the project has been created,install the necessary packages from requirements.txt fule using the command
 
 pip install -r requirements.txt
 
 In Conda also it's easy
 
 STEPS:-
 1. Create a new virtual environment using the command 
 
 conda create -n your_env_name python=3.6
 
 2. Navigate to the project directory
 3. Install the necessary packages from requirements.txt file using the command 
 
 pip install -r requirements.txt
 
 Workflow Diagram - 
 
 ![image](https://user-images.githubusercontent.com/61505882/172393102-91dbc9fc-00e0-47fd-9329-45d269399f57.png)
 
 Implementation 

1. Project Directory

![image](https://user-images.githubusercontent.com/61505882/172393664-edc8bb43-b369-4d4e-ba3d-246724ff371b.png)

This is the folder structure of the project

2. SpectrogramGenerator.py

![image](https://user-images.githubusercontent.com/61505882/172411082-6b3a7caf-708b-4604-9b0c-cfc5fe961854.png)

The file present in the dataloaders folder.SpectrogramGenerator.py is used to convert our .wav speech recorded file to spectogram images which will be used for training

3. train.py

![image](https://user-images.githubusercontent.com/61505882/172412914-00a34458-cf00-4c07-a89b-5d991a9d4b0b.png)

This file is used to do the training of the dataset and finally we will get the trained model which will be used for prediction

4. predict.py

![image](https://user-images.githubusercontent.com/61505882/172413613-935c84e4-9096-46f0-ba96-348975b1ab42.png)

It is used to do the prediction of the given user input with two other argument parameters

5. clientApp.py

![image](https://user-images.githubusercontent.com/61505882/172414025-d9056f19-217e-43c7-9ec3-06a94bf0f5c5.png)

This is the flask server file and entry point of application

Testing in Local/API

To run this project in your local system just run the file clientApp.py and after that web server will start at localhost 5005 port

![image](https://user-images.githubusercontent.com/61505882/172415309-0e1711c3-e389-4bb7-9223-459d45c0abe6.png)

Enter the .wav file and click on predict button

![image](https://user-images.githubusercontent.com/61505882/172415406-5e60470f-222b-4fb9-9987-27e0f52724d6.png)

![image](https://user-images.githubusercontent.com/61505882/172415457-c5409cd6-d547-4371-a1a2-fac69bb354c0.png)


Conclusion -

In this project we have successfully built a language identification which can classify and identify six internatonal languages.

Improvements -

Here we can do a lot of improvements. We can go with pre trained models like BERT , GPT2 etc to increase the accuracy. We can also increase the size of the training data.












