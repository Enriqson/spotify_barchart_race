# Spotify Barchart Race

## Python 3.10.8

This repo produces an animated video tracing the evolution of a given Spotify Playlist by plotting the most relevant artists in a barchat race format.

The code may be easily extended to display other information in the barchart race format.

## Main libs:
- Spotipy - Easy connection with Spotify API
- Matplotlib - Barchart plotting and Animation
- Duckdb - Data transformation

## Caveats/TODOs:
- Matplotlib plotting/animating is really slow and takes most of the processing time. The performance drawback has to do with the plotting itself and is not affected by the presence of the artists' profile images. Alternative plotting solutions may be tested but must support png image plotting and text labels.
  
- Artist profile images don't always align perfectly with the barchart plot. Plotting the images aligned with the bars is rather finicky due to Matplotlib's coordinate system.

## Use

Install requirements via pip with `pip install -r requirements.txt`

Add Spotify developer credentials to .env, following the .env.template file

Run the notebook swapping the PLAYLIST_ID