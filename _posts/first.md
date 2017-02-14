---
layout: post
date: "2017-01-31T00:00:31-08:00"
title: "Introductory Post about M.S. in Data Science"
categories: M.S. update
---

It's been a little over 2 weeks since I started my master's program in Data Science at the University of New Haven, and I thought it would be a good idea to document my experience. I'm currently taking two mathematics related courses - one being Mathematics for Data Scientists (DSCI6001), and second is Data Exploration, Feature Engineering, & Statistics for Data Scientists(DSCI6002). DSCI6001 is essentially a review of linear algebra and differential calculus, while DSCI6002 is more of applying statistics & probability to data sets using Python 3.

Since the first round of exams are coming up, I wanted to highlight some topics we've covered, and also talk about the specific things I've enjoyed.

Mathematics for Data Scientists:
- Solving systems of linear equations using augmented matrices.
- Gauss Elimination, Gauss-Jordan Elimination
- Determinants, Matrix Inversion, and Linear Independence
- Markov Processes
- Vector Spaces and Linear Tranformations
- Eigenvalues and Eigenvectors

I've noticed that my professor for this course wants us to understand the proofs behind these concepts. I've never been a fan of proofs in my college years, yet I really enjoy this part. I feel like it definitely helps me understand what is exactly going on, and as a result, makes my foundation in math stronger. The pace has been relatively fast, but since we have daily quizzes, I feel like it's been easy to follow along. On a side note, I think I'm starting to see how vector spaces and eigenvectors is involved with machine learning algorithms such as SVM and KNN clusters.

Data Exploration, Feature Engineering, & Statistics for Data Scientists
- Exploratory Data Analysis using Pandas
- Permutations and Combinations
- Independent and Dependent Probability
- Conditional Probability and Bayes Thereom
- Random Variables and Probability Mass Function

I've taken a couple of courses in statistics before, and so far, this class is more of a review for me. I'm really looking forward to our final project for this class - we will be doing exploratory data analysis and statistical breakdowns on a data set of our choice. I'm currently debating at looking at NBA advanced stats or NBA historical regular stats for my data set. Anyway, that's a bit in the future, so I'll mention something that's more relevant, and more interesting. Today in class, we actually had a quiz question that came from a Facebook Data Scienctist interview. I was pretty excited because I actually got the question right, and got to present my solution to the class. Here's the question below:

You're about to get on a plane to Seattle. You want to know if you should bring an umbrella. You call 3 random friends of yours who live there and ask each independently if it's raining. Each of your friends has a 2/3 chance of telling you the truth and a 1/3 chance of messing with you by lying. All 3 friends tell you that 'Yes' it is raining. What is the probability that it's actually raining in Seattle?

My solution was to use Bayes Theorem and find P(raining | 3Yes).
P(raining | 3Yes) = P(3Yes | raining) * P(raining) / P(3Yes)
P(raining | 3Yes) = (2/3)^3 * 0.25 / (2/3)^3 * 0.25 + (1/3)^3*.75

My rationale for the dominator is that each friend has 2/3 chance of telling the truth that it's raining, so you have to cube it, and then multiply it by the probability that it actually rains. Then the second part follows the same logic, each friend has 1/3 of lying to when it's actually not raining. 

Thus, the answer of P(raining | 3Yes) = 8/11 or .72

Apparently the answer to this question is heavily debated, but I definitely think a Bayesian approach makes the most sense.