This is a final project for DTSA 5511 Introduction to Deep Learning. For this project, I decided to work on something 'fun': music generation. I will be utilizing attention based Bi-directional LSTM (Long Short-Term Memory) to produce classical style music. LSTMs perform well for processing sequences of data with long-range dependencies, making them suitable for generating music. They can capture information from earlier time steps and remember it for an extended period. 

For the dataset, I will use classical music MIDI files sourced from [*Classical Piano Midi Page*](http://www.piano-midi.de/midi_files.htm). The MIDI files contain compositions for a single instrument: piano, from various composers. 
I will focus specifically on works by Bach, Beethoven, Chopin, Mozart, and Debussy, who is considered a more modern composer compared to the others. 
Additionally, I've incorporated MIDI files from a different genre: anime music.

My objective is to generate music that is coherent and resembles the style of the original composers. I will train the network separately for each composer to allow the model to capture the distinctive style presents in their music.

My code is based on my interpretation of the works by Alex Issa [*DataScienceMusic*](https://github.com/alexissa32/DataScienceMusic). I examined his works to understand the process, especially since this is my first time working with music notes.

#### Listen to the Generated Music on SoundCloud
[![Audio Player](https://img.shields.io/badge/Listen-Click%20to%20Play-blue)](https://on.soundcloud.com/Xo9BkDfvNpRq1ED29)

#### Model Architecture
*Diagram showing Bi-directional LSTM with Attention mechanism. Credit: [Gullapalli Keerti et. al](https://arxiv.org/pdf/2002.03854)*

![bilstm_attn](https://github.com/WellyWong/LSTM_music_generation/assets/70742141/c2a07bdc-80d1-4837-9d26-f061f059a860)
