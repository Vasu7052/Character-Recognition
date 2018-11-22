# Devanagri Character Recognition Assignment

Successfully created a classifier that can predict the character represented by an input image with an Accuracy of 98.81% (on colab) on the validation set. Dataset used is the same dataset i.e. ```Devanagari Handwritten Character Dataset Data Set``` that was mentioned in the assignment.

Link to the dataset : <a href="https://archive.ics.uci.edu/ml/datasets/Devanagari+Handwritten+Character+Dataset">https://archive.ics.uci.edu/ml/datasets/Devanagari+Handwritten+Character+Dataset</a>

My converted training dataset CSV file  : <a href="https://drive.google.com/open?id=1ER7LAip_Vjq_FqymUaRn-U62kPASrF0I">https://drive.google.com/open?id=1ER7LAip_Vjq_FqymUaRn-U62kPASrF0I</a>

My converted training dataset CSV file  : <a href="https://drive.google.com/open?id=1FuaAVgxzcNqZ2jHvOd2CrjhjUfXP-_vb">https://drive.google.com/open?id=1FuaAVgxzcNqZ2jHvOd2CrjhjUfXP-_vb</a>

## Google Colab Sharable Link

<a href="https://colab.research.google.com/drive/1EoR4ov7YIc0tIYeQ-0K92IWmgNkt6sSy">https://colab.research.google.com/drive/1EoR4ov7YIc0tIYeQ-0K92IWmgNkt6sSy</a>

## Steps of Approach
* Firstly, I converted dataset of images into a numeric dataset and stored them into a single CSV File. Reason being that uploading of approx 1 lakh images over colab was a tedious task. But upload just CSV files was much convenient.
* Then I checked the data range values and normalized the data between 0 and 1 for good practice.
* Now I created model structure consisting of multiple convolutional and max-pooling layers for input and dense layers for output.
* Now I choose some ideal hyperparameters for training the model and started training the model.
* Now I analyzed validation set accuracy as well as Accuracy and Loss over time through the graph using matplotlib
* Everything is final, then I created Web API using very known Backend Framework Flask.
* I successfully hosted my web API to Heroku dev center with proper documentation. 

## Features

* Converted Large set of images into simple Dataset CSV files for better numeric computations
* Created Web API for better usage and understanding
* High Accuracy
* Auto Saving of models for later use in web API

## Usage 

### For Jupyter Notebook
* Just run train_model.ipynb in the Jupyter notebook and it will start the training process

### For Web API Local
* Change directory from ``root`` to WebAPI
* Activate your virtual environment
* Run command ```python3 app.py```
* That's it, now open URL ```127.0.0.1:5000``` for usage
* Postman like 3rd party software can be used for creating API request at ```127.0.0.1:5000/predict/```


## For Web API Deployed

* Go to ```https://character-recognition.herokuapp.com/``` for seeing the overview of my work
* There you will find instructions for post request, which is as follow :
    * ```Endpoint : ``` https://character-recognition.herokuapp.com/predict/
    * ```Method : ``` POST
    * ```Only Parameter : ``` test_image (of file type)

## Common Libraries Used
* Numpy
* Pandas
* Flask (For web API)
* Keras
* Tensorflow
* Scipy (For web API)
* Pillow (For web API)

## Screenshots
<p float="left">
<img src="https://github.com/Vasu7052/Character-Recognition/raw/master/Screenshots/ss1.png" alt="" style="max-width:80%;">
<img src="https://github.com/Vasu7052/Character-Recognition/raw/master/Screenshots/ss2.png" alt="" style="max-width:80%;">
</p>
<p float="left">
<img src="https://github.com/Vasu7052/Character-Recognition/raw/master/Screenshots/ss3.png" alt="" style="max-width:100%;">
<img src="https://github.com/Vasu7052/Character-Recognition/raw/master/Screenshots/ss4.png" alt="" style="max-width:100%;">
</p>
<p float="left">
<img src="https://github.com/Vasu7052/Character-Recognition/raw/master/Screenshots/ss5.png" alt="" style="max-width:100%;">
<img src="https://github.com/Vasu7052/Character-Recognition/raw/master/Screenshots/ss6.png" alt="" style="max-width:100%;">
</p>
<p float="left">
<img src="https://github.com/Vasu7052/Character-Recognition/raw/master/Screenshots/ss7.png" alt="" style="max-width:100%;">
<img src="https://github.com/Vasu7052/Character-Recognition/raw/master/Screenshots/ss8.png" alt="" style="max-width:100%;">
</p>

# Deployed WEB API

I have deployed web api to Heroku for instant testing

Web API is running on <a href="https://character-recognition.herokuapp.com/">https://character-recognition.herokuapp.com/</a>

## Usage

* Go to ```https://character-recognition.herokuapp.com/``` for seeing the overview of my work
* There you will find instructions for post request, which is as follow :
    * ```Endpoint : ``` https://character-recognition.herokuapp.com/predict/
    * ```Method : ``` POST
    * ```Only Parameter : ``` test_image (of file type)


## Screenshots

<img src="https://github.com/Vasu7052/Character-Recognition/raw/master/Screenshots/web_ss1.png" alt="" style="max-width:100%;">
<img src="https://github.com/Vasu7052/Character-Recognition/raw/master/Screenshots/web_ss2.png" alt="" style="max-width:100%;">
