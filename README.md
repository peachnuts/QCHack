# QCHack
This is our project about IBM Creative Challenge!
Please find our code in the [`notebook`](https://github.com/peachnuts/QCHack/blob/start/Creative_challenge.ipynb) and the results in [`csv`](https://github.com/peachnuts/QCHack/blob/start/raw_result.csv) and [`mp3`] (https://github.com/peachnuts/QCHack/blob/start/raw_result_avg_subtracted.mp3) file!
## Steps 
1. We first create a simple circuit to show the impact of quantum interference.
2. Then, we demonstrate a show case of quantum interference using Simon's algorithm.
3. Finally, we implement our idea on the lines of ['Joy Vazirani'](https://www.jrussellhuffman.com/joyvazirani/) and convert our sample string "Qiskit" to musical tone.We take the input string "Qiskit" and generate corresponding circuits for each letter. Later we use simulator  with noise model to generate 6 outputs as a csv file. These raw data will serve as input for generating the musical sounds.

## Audio

1. From the csv file, we took an average of the data, and subtracted it from each of the data values, so that there would be both negative and positive data points, to make the sound better and so the waveform would be more balanced over the center.  
2. We then imported the updated txt file into Audacity by going to File > Import > Raw Data with the settings: 
                                               Encoding: Signed 8-bit PCM (we tried some values in binary form but weren't able to notice a difference for                                                                        some reason, so we used decimal)
                                               Byte order: Little-endian
                                               Channels: 1 Channel (Mono)
                                               Sample Rate: 8000Hz (sounded best with this)

