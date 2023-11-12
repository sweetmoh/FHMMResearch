MASSIVE DISTRIBUTED MICROPHONE ARRAY DATASET
An open dataset of speech recorded with 160 microphone

Authors: Ryan M. Corey, Matthew D. Skarha, and Andrew C. Singer
Institution: University of Illinois at Urbana-Champaign
Date: October 2019

This dataset is freely available on the Illinois Data Bank. Please cite this dataset in the following way:
Ryan M. Corey, Matthew D. Skarha, and Andrew C. Singer, Massive Distributed Microphone Array Dataset, University of Illinois at Urbana-Champaign, 2019. https://doi.org/10.13012/B2IDB-6216881_V1.

This dataset is licensed under a Creative Commons Attribution 4.0 International License CC BY, which requires attribution.

Please see the 'dataset_documentation.pdf' file located in this directory for details about the dataset and experimental procedure. This readme file contains an abbreviated description of the dataset.


INTRODUCTION

This dataset contains audio recordings from 10 loudspeakers and 160 microphones spread throughout a large, reverberant conference room. There were 16 microphones in each of 4 wearable arrays placed on plastic mannequins and 8 microphones in each of 12 tabletop enclosures.

The dataset includes four signal types:
1. 20-second exponential frequency sweeps from each of 10 loudspeakers,
2. Separate 60-second speech recordings from each loudspeaker,
3. A 60-second recording of all 10 speech signals together, and
4. A 55-second recording of ambient noise in the room.


SOURCE DATA

The speech clips used in this dataset are derived from the CSTR VCTK corpus:

Veaux, Christophe; Yamagishi, Junichi; MacDonald, Kirsten. (2017). CSTR VCTK Corpus: English Multi-speaker Corpus for CSTR Voice Cloning Toolkit, [sound]. University of Edinburgh. The Centre for Speech Technology Research (CSTR). https://doi.org/10.7488/ds/1994.


MEASUREMENT PROCEDURE

The recordings were made using 10 studio monitors and 16 omnidirectional lavalier microphones. The loudspeakers remained fixed and the microphones were moved 10 times for a total of 160 locations. Wearable arrays were measured individually and tabletop arrays were measured in pairs (1 and 2, 3 and 4, etc.).

Audio data was captured at 48 kHz by a Focusrite Scarlett 18i20 and OctoPre digital audio interface.


DATASET ORGANIZATION

The dataset is distributed as multichannel WAVE audio files. The naming convention is as follows, where XX is the array number and YY is the loudspeaker number.

Wearable arrays (XX = 01-04, YY = 01-10):
	Chirps:			wearableXX/wearableXX_chirpYY.wav
	Individual speech:	wearableXX/wearableXX_speechYY.wav
	Speech mixture:		wearableXX/wearableXX_mix.wav
	Ambient noise:		wearableXX/wearableXX_noise.wav

Tabletop arrays (XX = 01-12, YY = 01-10):
	Chirps:			tabletopXX/tabletopXX_chirpYY.wav
	Individual speech:	tabletopXX/tabletopXX_speechYY.wav
	Speech mixture:		tabletopXX/tabletopXX_mix.wav
	Ambient noise:		tabletopXX/tabletopXX_noise.wav

Source signals (YY = 01-10):
	Chirp:			sources/chirp.wav
	Speech:			sources/speechYY.wav
