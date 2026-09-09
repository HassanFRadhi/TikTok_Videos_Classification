# Classification of Claims in TikTok Videos
## Overview
The goal of this project was to create a predictive model that can determine whether a video contains a claim or offers an opinion. This project utilized different published TikTok videos in which a claim/opinion has been made. The final random forest model performed with nearly 100% accuracy and 99% recall determining what features were most important in separating claim from opinion videos. Based on the model, the count of views, likes, shares, downloads and comments of the video was most influential in determining a claim video versus a opinion video.

## Business Understanding
TikTok users have the ability to report videos and comments that contain user claims. These reports identify content that needs to be reviewed by moderators. This process generates a large number of user reports that are difficult to address quickly. With a successful prediction model, TikTok can reduce the backlog of user reports and prioritize them more efficiently.

## Data Understanding
This project uses a dataset called tiktok_dataset.csv. It contains synthetic data created for this project in partnership of Google advanced data analytics certificate program with TikTok. The dataset contains unique 19,383 video and 12 features for each one. The features included information on video claim status, duration, transcription text, and counts of different interactions. Also included author verification and ban status. The bar chart below shows the breakdown of how many claim videos versus opinion videos that exist in the data set. 
<img width="1023" height="630" alt="Sheet 2" src="https://github.com/user-attachments/assets/4ed71ce0-19f4-48b5-b901-896be6e64034" />
In connection to this, a feature was engineered to represent the transcript text length. Multiple redundant columns were dropped and encoded into the proper data type.  

## Modeling and Evaluation 
A random forest model comprising 75 decision trees was used to determine feature importance in video classification as a claim or not. The below plot shows that video views, likes, and downloads were the Top 3 most important factors in determining a claim video. The overall model performed with same scores after testing, nearly 100% accuracy and 99% recall.
<img width="777" height="879" alt="image" src="https://github.com/user-attachments/assets/c5298422-362b-431e-b4d8-5bdb7f3b66b7" />

## Conclusion
it is highly recommended to start using the model in a trial because it shows good measures and any helpful feedback would be of high benefit for further improvement. Getting the number of reports done by users on each claim classified video could be very useful where we can arrange claim videos by number of reports in descending order and review them manually. 
