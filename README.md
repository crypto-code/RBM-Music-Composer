# Music-Generator
Use TensorFlow to Generate Music with a Restricted Boltzmann Machine.
<p align="center">
<img src="https://github.com/crypto-code/Music-Generator/blob/master/assets/music.JPG" width="800" height="300" align="middle" />   </p>

## Restricted Boltzman Machine
A Restricted Boltzmann Machine (RBM) is a generative stochastic Neural Network that can learn a probability distribution over its set of inputs. This setup can be used to predict the next note in a sequence given the previous note.
<p align="center">
<img src="https://github.com/crypto-code/Music-Generator/blob/master/assets/model.png" align="middle" />   </p>

For more info go [here](https://rubikscode.net/2018/10/01/introduction-to-restricted-boltzmann-machines/)

## Dependencies

  * Tensorflow
  * pandas
  * numpy
  * msgpack-python
  * glob2
  * tqdm 
  * python-midi

## Basic Usage
To train the model and create music, simply clone this directory and run
```
python gen_chords.py
```
The run usually takes 5 minutes in a modern PC.

## Changeable Parameters
* To change input midi files, modify line 28:
```
songs = get_songs('elvis')  #Change this to your folder name
```

* To change song length generated, modify line 39:
```
num_timesteps = 150  # number of timesteps that we will create, (change this to change the time of music generated)
```

* To change number of epochs, modify line 43:
```
num_epochs = 1000  # The number of training epochs that we are going to run.
```

* To change save location, modify line 135:
```
midi_manipulation.noteStateMatrixToMidi(S, "out/generated_chord_{}".format(i))
```

# G00D LUCK

For doubts email me at:
atinsaki@gmail.com
