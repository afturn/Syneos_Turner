# Syneos_Turner
Syneos Health Coding Exercise

A python coding project used to build a Random Forest model in order to predict whether or not a song/artist will be on Spotify's Top Artists of the Year. 

## Credit to Open Source for Making this Possible 

Spotify: https://developer.spotify.com/documentation/web-api/reference/tracks/get-audio-features/

spotipy: https://spotipy.readthedocs.io/en/latest/

sklearn (Random Forest Classifier and Randomized/GridSearchCV) : https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestClassifier.html

Shreye's initial project: https://github.com/shreyejsaxena/bonnarhythms

## Background

For this project I decided to analyze the most popular artists on Spotify for the years 2013-2019 (most popular meaning most streamed). Spotify releases this information every year, and I wanted to attempt to build a model that can predict whether or not a song/artists will be on Spotify's top artist of the year. In its present state, the data that my model was built on was not randomly sampled. I included songs from the top artists as well as songs from artists that weren't included on the top lists. I tried to include both common artists that are common on the radio, but not on the top list as well as artists the I had never heard of. Ideally, I would have have a randomly sampled subset of all artists not on Spotify's top lists in order to reduce bias in the model. I also ran some initial cluster analysis to attempt to determine similarities in the songs by Spotify's top artists. 

The Spotify API enables users to retrieve the Top 10 tracks of an artist (by their name), and each track has audio features on which quantitative analysis can be peformed:

- acousticness
- danceability
- energy
- instrumentalness
- liveness
- loudness
- speachiness
- valence
- tempo


## Next Steps

I think Spotify already does a great job of using analytics in order to attempt to recommend songs already in order to improve the user's listening experience, so I wanted to attempt this from a different angle. One way that Spotify could use the model built would be to look into the songs that the model wrongly classified as popular and recommend them to users that like the "popular" songs to see if that artists is potentially just an "undiscovered" artist. 
