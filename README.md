# MOVIE RECOMMENDATION

## A. PROJECT SUMMARY

**Project Title:** Movie Recommendation

**Team Members:** 
- [insert Member Name]
- [insert Member Name]
- [insert Member Name]
- [insert Member Name]


- [ ] **Objectives:**
- Break out the project goal into more specific objectives
- To help people make the right choices, without having to expend their cognitive resources.
- To search for content that would be interesting to an individual
- To help the people find something they like.


##  B. ABSTRACT 

Nowadays we live in era of abundance. For any given product, there are many of options to choose from. For example like streaming videos, social networking, online shopping; the list goes on. Recommender systems help to personalize a platform and help the user find something they like. The easiest and simplest way to do this is to recommend the most popular items. However, to really enhance the user experience through personalized recommendations, we need dedicated recommender systems.

There are two categories for recommender system which are Content-Based Movie Recommendation Systems and Collaborative Filtering Movie Recommendation Systems

![Coding](https://github.com/Fairuza97/AI/blob/main/movieRecommendation.png)

Figure 1 shows the AI output of movie recommendation.


## C.  DATASET

For our own system, I use the open-source MovieLens dataset from GroupLens. This dataset contains 100K data points of various movies and users.
I will use three columns from the data which is userId, movieId, rating.

![Coding](https://github.com/Fairuza97/AI/blob/main/dataset.JPG)

Figure 2 shows the dataset from MovieLens.

There are two categories for recommender system which are Content-Based Movie Recommendation Systems and Collaborative Filtering Movie Recommendation Systems

**Content-Based Movie Recommendation Systems:** 

Content-based methods are based on the similarity of movie attributes. Using this type of recommender system, if a user watches one movie, similar movies are recommended. For example, if a user watches a comedy movie starring Adam Sandler, the system will recommend them movies in the same genre or starring the same actor, or both. With this in mind, the input for building a content-based recommender system is movie attributes.

![Coding](https://github.com/Fairuza97/AI/blob/main/ContentBased.JPG)
Figure 3 show overview of content-based recommendation system

**Collaborative Filtering Movie Recommendation Systems:** 

With collaborative filtering, the system is based on past interactions between users and movies. With this in mind, the input for a collaborative filtering system is made up of past data of user interactions with the movies they watch.
For example, if user A watches M1, M2, and M3, and user B watches M1, M3, M4, we recommend M1 and M3 to a similar user C. You can see how this looks in the figure below for clearer reference.

![Coding](https://github.com/Fairuza97/AI/blob/main/Collabarative.JPG)

Figure 4 show an example of the collaborative filtering movie recommendation system


## D.   PROJECT STRUCTURE

For the project use Matrix Factorization-based Algorithm for Collaborative filtering

Matrix factorization algorithms work by decomposing the user-movie interaction matrix into the product of two lower dimensionality rectangular matrices, say U and M. The decomposition is done in such a way that the product results in almost similar values to the user-movie interaction matrix. Here, U represents the user matrix, M represents the movie matrix, n is the number of users, and m is the number of movies.
Each row of the user matrix represents a user and each column of the movie matrix represents a movie.

![Coding](https://github.com/Fairuza97/AI/blob/main/matric.JPG)

Figure 5 show Matrix factorization 


## E   PERFORMANCE METRICS

There are two main ways to evaluate a recommender system’s performance: Root Mean Squared Error (RMSE) and Mean Absolute Percentage Error (MAPE). RMSE measures the squared loss, while MAPE measures the absolute loss. Lower values mean lower error rates and thus better performance.
Both are good as they allow for easy interpretation.

**Root Mean Squared Error (RMSE):**
RMSE is the square root of the average of squared errors and is given by the below formula.

![Coding](https://github.com/Fairuza97/AI/blob/main/matric.JPG)

Where:
r is the actual rating,
r^ is the predicted ratings and
N is the total number of predictions

**Mean Absolute Percentage Error (MAPE):**
MAPE measures the error in percentage terms. It is given by the formula below:

![Coding](https://github.com/Fairuza97/AI/blob/main/matric.JPG)

Where:
r is the actual rating,
r^ is the predicted ratings and
N is the total number of predictions

![Coding](https://github.com/Fairuza97/AI/blob/main/matric.JPG)

Our model resulted in 0.67 RMSE, and 19.86 MAPE on the unseen test data, which is a good-to-go model. An RMSE value of less than 2 is considered good, and a MAPE less than 25 is excellent. That said, this model can be further enhanced by adding features that would be recommended based on the top picks dependent on location or genre. We could also test the efficacy of our various models in real-time through A/B testing.


## F.  RESULT AND CONCLUSION

Detecting COVID-19 face masks with OpenCV in real-time

You can then launch the mask detector in real-time video streams using the following command:
- $ python detect_mask_video.py
- [INFO] loading face detector model...
- INFO] loading face mask detector model...
- [INFO] starting video stream...

[![Figure5](https://img.youtube.com/vi/wYwW7gAYyxw/0.jpg)](https://www.youtube.com/watch?v=wYwW7gAYyxw "Figure5")

Figure 5: Mask detector in real-time video streams

In Figure 5, you can see that our face mask detector is capable of running in real-time (and is correct in its predictions as well.



## G.   PROJECT PRESENTATION 

In this project, you learned how to create a COVID-19 face mask detector using OpenCV, Keras/TensorFlow, and Deep Learning.

To create our face mask detector, we trained a two-class model of people wearing masks and people not wearing masks.

We fine-tuned MobileNetV2 on our mask/no mask dataset and obtained a classifier that is ~99% accurate.

We then took this face mask classifier and applied it to both images and real-time video streams by:

- Detecting faces in images/video
- Extracting each individual face
- Applying our face mask classifier

Our face mask detector is accurate, and since we used the MobileNetV2 architecture, it’s also computationally efficient, making it easier to deploy the model to embedded systems (Raspberry Pi, Google Coral, Jetosn, Nano, etc.).

[![demo](https://img.youtube.com/vi/-p7HGwOWxtg/0.jpg)](https://www.youtube.com/watch?v=-p7HGwOWxtg "demo")




