
# Mood Spotifier with Chatbot (MODIC)

In our proposed system, a mood-based music player is created which performs real time mood detection and suggests songs as per detected mood. 

We have developed the web-application in following steps:-
It starts with a visuals conversation between user and program.
Program will take a real-time image of the user.
Image will be processed and mood of the user will be detected.
The detected mood will be cross-checked from the user end.
If OK, then music album of related mood will be shown.
One of the song will be played.


## Team

Hari Om Shukla(Team Lead)
Sarthak Jain
Pratham Singh
Alokik Gupta


## Acknowledgements

It would be our pleasure to express special thanks to our Mini-Project Mentor "S.S. Parihaar" in providing his helping hand in this project.

His valuable guidance,support and supervision all through this project
titled "Mood Spotifier with Chatbot (MODIC)" are responsible for attaining its present form.

Thanks a lot Sir.


## Documentation

I. Chatbot Module:
This system starts with a conversation to the user like “Hello”, ”What’s Your Mood”, “Let me check it”, etc. It is also used for getting feedback from the user. Chatbot will be implemented in python language using Chatterbot Library.
Each time a user enters a statement, the library saves the text that they entered and the text that the statement was in response to.
The program selects the closest matching response by searching for the closest matching known statement that matches the input, then chooses a response from the selection of known responses to that statement.

II. Mood Detection Module :
This Module is divided into two parts: 
Face Detection — Ability to detect the location of face in any input image or frame. The output is the bounding box coordinates of the detected faces. For this task,  the python library OpenCV was considered.
Mood Detection — Classification of the emotion on the face as happy, angry, sad, neutral, surprise, fear or disgust. Keras which is a CNN architecture model for Image Classification and Mobile Vision was used since it uses very less computation power.
The dataset used for training was obtained by combining FER 2013 dataset [6] and MMA Facial Expression Recognition dataset [7] from Kaggle. Keras was used to train and test our model for seven classes - happy, angry, neutral, sad, surprise, fear and disgust. We trained it for different epochs and achieved an accuracy of approximately 75%.
The MMA Facial Expression Recognition dataset had images of different specifications. Thus, all these images were converted as per the images in FER 2013 dataset and combined to obtain an even larger dataset.

III. Music Recommendation Module 
The dataset of songs classified as per mood was found on Kaggle for two different languages - Hindi and English. 
Research for a good cloud storage platform to store, retrieve and query this song data as per user’s request was conducted .
We have selected Kaggle for this purpose.

IV. Integration
 For the integration of these two modules, the trained Keras model was saved as an .h5 file, and this .h5 file was then converted to a .tflite file using TensorFlow Lite Converter.
 It takes a TensorFlow model as input and generates a TensorFlow Lite model as output with .tflite extension. Since the Keras model is used, the size of the tflite file is expected be around 20- 25 Megabyte (MB) which was the desired size. 
The labels.txt file contains the class labels of the model. All the appropriate methods were created for loading the model, running the interpreter and obtaining the results.


## Lessons Learned

The most valuable and life remembering lesson was 'Great Works always comes with Difficulties".

But I we will not stop or loose our patience then that work becomes easy day by day.

"Team Work makes Dream, work".

We all have faced challenges in our assigned part but we helped each other and made this project as what we want to make.


## Features

- Comparatively Faster
- AI and CV are used
- User Friendly
- Easy to Understand
- Cross platform
- Mood Detection
- Use of rich libraries


## Installation

Install this project folder from github account.
    

## Deployment

Hardware Tools:
Processor : Intel core i-5   
Storage – 512 SSD          
RAM- 16 GB DDR4
WEBCAM – 5MP

Software Tools:
Operating System – Microsoft Windows 10
Platform – V S Code
Back End: Open CV, Keras 
Front End : streamlit,Chatterbot

Use any Editor or IDE which supports Python3.
We have used VSCode as our Code Editor.

Python IDLE version Python 3.10 64-bit

Install Extensions:-
Python:  ms-python.python
Jupyter: ms-toolsai.jupyter

Import Modules:-
tensorflow-cpu,opencv-python-headless,imutils==0.5.3,imageio,dj-database-url==0.5.0,Django==3.1.2,gunicorn==20.0.4,psycopg2-binary,whitenoise==5.2.0

Run manage.py, It will create a local host.
Copy that and go to face_detector->settings.py.
Add the copied host ID in ALLOWED_HOSTS.
Then paste that ID in Chrome Address bar and Enter.
The program will run.
Click 'detect my mood', it the program will recognize your mood and then play a song accordingly.
In any unexpected conditions, it will play song of 'calm' mood.
Enjoy the music ;)

he data we have used here is from https://www.kaggle.com/yamaerenay/spotify-dataset-19212020-160k-tracks.


## References


Geeks for Geeks - https://www.geeksforgeeks.org

ProgrammingHut - https://www.youtube.com/watch?v=uDzLxos0lNU

Buildmedia - https://buildmedia.readthedocs.org

Edureka! - https://www.youtube.com/watch?v=G1Uhs6NVi-M&t=565s

CodeWithHarry - https://www.youtube.com/watch?v=RhEjmHeDNoA

Applied DL & CV for Images & Video Data Analysis from Eduxlabs
https://www.eduxlabs.com/live-dl-cv-training


## Feedback

If you have any feedback, please reach out to us at email jainsarthak97162@gmail.com or contact us on Watsapp Number 9557234083.