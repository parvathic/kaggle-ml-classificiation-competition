# Quora Insincere Questions Classification

The Kaggle competition we picked is the Quora Insincere Questions Classification. The
dataset provided here is a collection of questions from Quora with labels identifying them
as sincere or insincere. Questions that are worded strongly for shock value, have
disparaging terms and disingenuous motives are labeled as insincere.

- The training data contains 1306122 samples with 3 columns, including a question id, the
question text and the label which classifies it into an insincere or sincere question.

- The test data contains 56370 samples with 2 columns.

Before working on developing the model, initially the first step taken was to inspect the
dataset. The problem here is a classification text related problem.

- Analyzing the ratio of sincere to insincere questions, it is seen that the number of sincere
questions [0’s] are higher than 1’s. With this realization, there was an idea to not set
accuracy as a performance metric in any model that would be run as the dataset is
unevenly distributed.

- F-1 score is a good metric to use as it combines both precision and recall which are
useful metric when dealing with a text-based dataset.

## Motivation

Quora is a platform that empowers people to learn from each other. On Quora, people can ask questions and connect with others who contribute unique insights and quality answers. A key challenge is to weed out insincere questions -- those founded upon false premises, or that intend to make a statement rather than look for helpful answers.

## Data Analysis

![ratio](/images/3.JPG)
