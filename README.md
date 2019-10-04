# Yelp Dataset

This dataset is a sample of Yelp dataset extracted from round 12 of Yelp Challenge. It consists of 4 files. 

Underscores

### ratings.txt

It contains the ratings given by users to businesses (items).

Every line has the following format:

	userid businessid rating

This file contains 

* 1,355 users who provided 
* 100,409 ratings on 
* 1,272 businesses.


### friendships.txt

It contains the friendship (trust) statements issued by users.

Every line has the following format:

	source_user_id target_user_id trust_statement_value

This file contains

* 919 source users who stated 
* 26,453 friendships (trustworthiness) toward
* 1,172 target users

trust_statement_value is always 1.


### users.txt

It contains users' demographic information.

Every line has the following format:

	userid name gender gender_accuracy samples

In this file

* Values for gender attribute are extracted by name using https://gender-api.com.
* Gender has 3 values: F, M, and N. F means female, M means male, and N means unkown.
* gender_accuracy is the accuracy of predicted gender.
* samples is the number of samples used for predicting gender.


### items.txt

It contains items information.

Every line has the following format:

	itemid category

One or more categories are assigned to each item.

### Citing

If you find this dataset useful for your research, please consider citing the following paper:

	@inproceedings{yelp40-rmse-recsys19,
	author = {Mansoury, Masoud and Mobasher, Bamshad and Burke, Robin and Pechenizkiy, Mykola},
	title = {Bias Disparity in Collaborative Recommendation: Algorithmic Evaluation and Comparison},
	booktitle = {RecSys workshop on Recommendation in Multi-Stakeholder Environments},
	year = {2019}
	}
