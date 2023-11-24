# Spotify Country Based Data Analysis
---


This repo consists of a practice data analysis of Spotify data collected through the Spotify API, using the  **[spotipy](https://spotipy.readthedocs.io/en/2.22.1/)** python package. \
The main idea is to collect the data in *Top 50* playlists from 5 different countries; Turkey (TR), Japan (JP), France (FR), Russia (RUS), and Argentina (ARG). The collected data will consist of the song names, song IDs and artist names. Audio features - provided by Spotify - for each of the songs will then be added to the main dataset, and these features will be used for both exploratory and comparative data analyses to reveal any possible differences between the music tastes of different countries.

The files and directories within the repository are as follows:
1. **requirements.txt** - Contains the python packages that will be required to run the following analysis. \
The requirements can be installed from the command line using:
``` bash
  pip3 install -r requirements.txt
```
2. **spotify_analysis.ipynb** - This is the main analysis code file, which is a jupyter notebook. It has 3 \ 
main parts, indicated and separated within the notebook with markdown cells.
	- ***Part 1: Spotify Data Collection & Cleaning*** - In this part, 5 different playlist data (for each country) and audio features for each song is pulled from spotify, and cleaned up to form a merged dataset consisting of all useful variables.
	- ***Part2: Explorative Data Analysis*** - The second part uses the python package **[ydata-profiling](https://docs.profiling.ydata.ai/4.6/)** to apply an overall exploration of the obtained datasets, showing various visualizations and identifying possible problems with the dataset, like missing values and high correlations. The datasets are then expored more in detail by adding certain visualizations to summarize the dataset in a more concise way (like a pairs plot).
	- ***Part3: Comparative Data Analysis*** - 
3. **results** - The directory that contains the resulting plots, tables and reports of the analysis.
4. **csv files** - Info that was collected from spotify and merged. Contains both the audio features data and the playlist contents (songs).
