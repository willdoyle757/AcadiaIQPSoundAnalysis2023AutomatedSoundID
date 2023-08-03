# AcadiaIQPSoundAnalysis2023AutomatedSoundID
This repository contains the python notebooks necessary for processing training data, training a CNN model and using the model to analyze sounds collected in Acadia national park

There should be 3 python notebook files each used for a different step in training the CNN model and using it to analyze data. 

The first is the TrainingWavFileProcessing.ipynb. This is used to process raw audio that has been labeled and use them for training the model. This is important if you wish to continue to add more training data.

The way Raw audio files should be named is as such below

Format audio Title: Location-MMddhhmmss-Category 
Example title: P-0701040230-10.wav 

Static/ nothingness is 51 
 

![Screenshot 2023-07-22 163033](https://github.com/willdoyle757/AcadiaIQPSoundAnalysis2023AutomatedSoundID/assets/61399895/ce959f2f-30d5-4bec-854e-ad783268b020)
![Screenshot 2023-07-22 162945](https://github.com/willdoyle757/AcadiaIQPSoundAnalysis2023AutomatedSoundID/assets/61399895/e1eae2a4-424d-40fe-aa09-a5cfd4af94cd)


The second notebook is used to train the model once the raw training files have been put into the dataset and registered on the csv. You can run the second notebook and where it will convert the audio into spectrograms and then train the model. Feel free to adjust hyperparameters as you see fit

The third notebook is used to analyze new data from Acadia to do this you must collect raw audio files each representing an hour subset of data. This can be done by using NTI Data explorer by exporting a project witht he clip in it. From there the wav file in the exported folder can be used. You must rename the wav file from 1.wav to:

Format audio Title: Location-MMddhhmm 
the minute is the start minute of the recording
Example title: P-07010402.wav

