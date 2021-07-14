# Collaborative Filtering Recommender

## Goal

The goal of this project is to: 1) demo a simple Collaborative Filtering process, and 2) recommend a movie to Toby based on his view history and movie reviews from other users (who are similar to Toby). 

## Recommendation Engine
In a nutshell, there are 3 major steps for a recommendation system:
- 1 Find candidates (**Candidate Generation**)
- 2 Assign score to each candidate (**Scoring**)
- 3 Rank candidates based on the highest scores, and also consider freshness, diversity, and fairness (**Re-Ranking**)

## Collaborative Filtering

- User-based, which measures the similarity between target users and other users.
- Item-based, which measures the similarity between the items that target users rate or interact with and other items.

### Step 1: Find Similar Users to Toby Using Correlation Score

In this example, Lisa Rose has the highest similarity with Toby regarding movie ratings. Thus it is reasonable to assume that they have similar movie preferences.

![2021-07-14 18_10_53-Window](https://user-images.githubusercontent.com/44503223/125704330-0615b017-e4e4-4172-8277-a088f0fb608e.png)

### Step 2: Assign Scores to Movies that Toby Hasn't Seen

The score assigning process is based on other movie watchers' scores. And Lisa Rose's score has higher importance on the final score because Lisa is most similar to Toby.

![2021-07-14 18_17_31-Window](https://user-images.githubusercontent.com/44503223/125704818-bfdc9e4b-320c-48c5-8830-082cdeb7a216.png)

### Step 3: Calculate Weighted Average for the Final Review Score

It seems Toby will like The Night Listener than the rest movies. 

![2021-07-14 18_20_11-Window](https://user-images.githubusercontent.com/44503223/125704957-84fc4457-be6d-4507-a4a4-533ad5e9e2c4.png)


## Reference:

The notebook is based on a [blog post](http://tungwaiyip.info/2012/Collaborative%20Filtering.html)., which is based on the book Toby Seragan's book Programming Collective Intelligence.

## Learn More

You can learn more in [Tingting Duan's Project Portfolio](https://tingting0618.github.io).

