#Avocoder: An Interface for Tangible Voice Manipulation

Sravanti Tekumalla and Galen Chuang

Created for MUS378: Deconstructive Audio, Professors Jenny Johnson and Nicholas Knouf

Presented at the Ruhlman Conference 2015 at Wellesley College

## Overview
Avocoder is a musical interface created for MUS378: Deconstructive Audio. Built with Arduino and Max/MSP, our interface allows people to manipulate their voices by tangibly varying pitch, volume and distortion. Modern musical synthesizers come with a myriad of preset patches and filters to alter pitch and voice, and that abstraction creates an environment for passive interaction. We aim to give people the chance to directly manipulate parameters of sound with their hands and voice, allowing them to explore sound beyond the paradigm of rigid systems. We hope that people will take away an experience of playing with digital sound and the sound of their own voice in ways they hadn’t before, and that Avocoder encourages them to challenge predefined constraints of modern musical software. 

Our project was inspired by the vocoder, a synthesis technique used to reproduce human speech. The vocoder was originally developed for telecommunication purposes in the 1930s, using the ideas of “codifying” speech and encrypting sound to avoid interception by third parties. The vocoder works by performing digital signal processing to modify the voice input, measuring how its spectral, or ghost-like, characteristics change over time. Avocoder uses a similar technique to manipulate voice (or voices). 

## MAX patches

There are two modes: 

__Uniform pitch__ – voice is set to two uniform pitches.

__Relative pitch__ – every pitch in the voice is shifted by a defined value.


### Master MAX Patch

![Alt text](/master_patch.png)

### Uniform pitch MAX patch

Two knob inputs are shown at the top, and calculations are performed on the data. Then, the data are converted into audio signals, which are then fed back into the main patch.

![Alt text](/second_mic.png)

### Second microphone MAX patch

Audio signal from microphone 2 is inputted and converted into non-audio data, which is used to modify the output of microphone 1.

![Alt text](/uniform_pitch.png)
