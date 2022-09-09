# Speech-based-interactive-quiz-game
Developed a voice-controlled interactive quiz game where computer will speak up the questions for the palyer and player will have to speak up their answers.
<p align="center" width="100%">
    <img width="33%" src="https://user-images.githubusercontent.com/47311900/189338996-ed5ae0a2-1386-499f-acf6-9e70cc9fda79.PNG">
</p>

# Requirements
Basic requirements to develop this project are as follows:
<br />✓ Windows OS 
<br />✓ Microsoft Visual Studio 2010 
<br />✓ C++ 11 integrated with VS2010
<br />✓ Recording Module

# Experimental setup
This project is divided into following modules: 
1. Training Module 
2. Testing Module 
3. Live Training Module
# 1. Training Module: 
The flow for training over data is as follows: 
<br />a. Record 20 utterances for each word which are used in project. 
<br />b. Extract frames of speech part from these recordings with 2-3 frames silence 
at beginning and end of word
<br />c. Use front end analysis to get observation sequence from the speech.
<br />d. Pass this observation sequence to HMM for model designing by using Bakis 
model(feed forward model) as initial model.
<br />e. Now enhance the model using HMM re-estimation algorithm (Baum welch).
Now reference models for each word are ready for our project. The training of data is 
not integrated with GUI application. This is different module which will just evaluate 
reference model
# 2. Testing Module 
We need search the word by speaking into the microphone. 
The flow of testing is as follows: 
<br />a. Live recording of data is done on clicking on record answer button . 
<br />b. Testing will be done on the data with pretrained models. 
<br />c. Verifying the answer with 4 options using in that question. 
<br />d. If verification is successful then show that your answer is correct. 
<br />e. If verification fails then show that your answer is correct. 

# 3. Live Training Module 
The flow for live training over data is as follows: 
<br />a. Put the word and directory from the list mention in that page . 
<br />b. Click on train button.
<br />c. Extract frames of pre recorded words. 
<br />d. Using front end analysis to find the observation sequence. 
<br />e. Pass this observation sequence to HMM for model designing by using Bakis 
model(feed forward model) as initial model.
<br />f. Now enhance the model using HMM re-estimation algorithm (Baum welch). 
Now the reference models for each word are ready and saved 
# Screenshots
![Capture](https://user-images.githubusercontent.com/47311900/189337268-83236e5e-1e03-45ba-b5c9-e3440e31ae7b.PNG)


![ui1](https://user-images.githubusercontent.com/47311900/189338903-efe6b4a7-ee47-4277-afea-2016423d4e43.PNG)
![ui2](https://user-images.githubusercontent.com/47311900/189338927-2296c06f-4db0-4094-8bfe-1f719a13e432.PNG)

![end](https://user-images.githubusercontent.com/47311900/189340139-3db7d5d6-32dc-4d8a-8664-abaacff58a2c.PNG)

