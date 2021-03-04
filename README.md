# Eluvio_Scene_Segmentation

## EDA
Contains analysis of the data in hand

## LGSS_Model_1
Contains the implementation of the architecture mentioned in the paper 'A Local-to-Global Approach to Multi-modal Movie Scene Segmentation'. Here the data is trained is such a way that each shot is considered as a different data point.

## LGSS_Model with SA
A movie level formulation is suggested in the above mentioned paper because of the fact that a LSTM can't contain large number of shots due to memory limitations. An idea which I think could work instead of the Movie-Level formulation is the concept of self attention. Instead of using a LSTM, a multi-head self attention module could bring out the relationships between different shots in a movie in a much better way. 
The architecture is presented in this notebook, but I still need to figure out a way to feed data into the model for which I will need a little bit more time.
Here, each movie will be considered as a single data point with n number of sequences where the sequences are the movie shots.
