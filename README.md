# Beatle-Basslines
The project trains a Deep Learning model (including all data pre-processing) to generate basslines in the style of Paul McCartney from other tracks in a MIDI file. The code is easily modified to learn other instruments - e.g. vocal melodies or drums. Different real-world performers can be modeled by using a different dataset of MIDI files.

## Features
* Reads MIDI files (with properly labeled tracks) into a Pandas dataframe.
* Transforms pianoroll data into ML-ready k-hot sequences of training, validation, and test data. Dimensionality is reduced with automatic note range clipping.
* Play predicted and original sequence audio in-notebook for progress monitoring.
* Model is currently a stacked BiLSTM.
* Notebook includes all initialization to work from a repository clone in Google Drive.

## Dependencies
* Currently, TensorFlow/Keras is used for the modeling. This could be easily swapped for another tool.

* The dataset is primarily based on a version of [David W Barnes' MIDI library](http://www.davidbmidi.com/beatles.htm) with relabeled and cleaned instrument tracks. I currently do not have permission to redistribute those files directly.

## Licensing
This code is licensed under MIT license.
