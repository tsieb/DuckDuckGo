# DIY Duck Face
## DuckDuckGo's Quackathon project
This project consists of an app, api, and machine learning model.
## Mobile Application
The mobile application was developed in flutter for IOS and Android.
It allows the user to photograph a duck and then receive a cut out duck image that is pasted over their face on video.
The face of the user is tracked in the camera using OpenCV.

## Duck Classification Model
The model was trained on 3000 pictures of birds. 1029 Ducks of all available species, and the remainder were photos of various other types of birds.
The model used the pretrained `ResNet50` model followed by additional layers trained using the aforementioned data.

## API
Using the API, the application sends an image for classification. 
The image is fed through the classification model and the highest output node is used to return an appropriate image to the app
