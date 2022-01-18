# AL_project
Project for Artificial Life course

This is the code for the generation of music sequences using a LSTM Recurrent Neural 
Network

2 ipynb files for each: LSTM implementation and the plotting of the CobWeb

Following preliminary steps are necessary to execute the code:

1. install python v.3.6+  (code was implemented and tested on version 3.8.8)
2. install tensorflow 2.6
3. install dependencies: 
	a) fluidsynth (either with "apt install","brew install", or others)
	b) pretty_midi (installation can be done with "pip")

The rational behind the code to create the LSTM model and manipulation the data is 
described as follows: (which is taken from the open source code provided at: 
tensorflow.org/tutorials/audio/music_generation)

1. create methods to manipulate MIDI files (inter alia, convert midi files to arrays 
containing their nodes with all the relevant information being: pitch, step (time 
distance from current to previous note, duration)
2. create the training dataset upon which the recurrent neural network will be trained on
3. create and train the model
4. evaluate the model
5. generate/predict an output/sequence of notes give an input of length 25


