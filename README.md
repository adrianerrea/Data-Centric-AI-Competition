# Data-Centric AI Competition from DeepLearning.AI

## Description
A collaboration between DeepLearning.AI and Landing AI, the Data-Centric AI Competition aims to elevate data-centric approaches to improving the performance of machine learning models.

In most machine learning competitions, you are asked to build a high-performance model given a fixed dataset. However, machine learning has matured to the point that high-performance model architectures are widely available, while approaches to engineering datasets have lagged. The Data-Centric AI Competition inverts the traditional format and instead asks you to improve a dataset given a fixed model. We will provide you with a dataset to improve by applying data-centric techniques such as fixing incorrect labels, adding examples that represent edge cases, apply data augmentation, etc.

## Links
Discourse: https://discourse.deeplearning.ai/c/competitions-dlai/data-centric-ai/50

Home Page: https://https-deeplearning-ai.github.io/data-centric-comp/

## Insights

As shown in the notebook in the repository, my first trials were as following:
+ A first iteration with all the data provided to set up a baseline.
+ Second iteration after removing non number images and reorganising mislabelled examples.
+ My third iteration was changing the hyperparameters to get better results. I knew this was not going to improve the goal of the project (iterate over the data not over the model) but I wanted to check how difficult was the problem itself. After that I fixed the model and hyperparameters as close as the training phase described in the competition.
+ Next step I took was creating new images with the library _albumentations_. At the same time, I tried to balance the dataset with this technique getting around 500 images per class. 
+ I iterated again with the fixed model and hyperparameters and I did not notice any remarkable improvement.
+ So I decided to try this new dataset with the best model I built before. Then, I saw better results with this last tecnique.

## Conclusions and Improvements
+ I ended up the competition in an ordinary 350 position out of 486 submissions.
+ I did not spend so much time on this project but I decided to join because it was one of the first competitions of this type on internet (and if Andrew Ng is involved, we must try it out 😉).
+ Once the competition was done, I looked up again the data and I did notice there were still some mislabelled examples. We could have tried out another cleaning phase.
+ The limit of the images to upload was 10000 and I used just 5607 so I might have generated quite more data to improve the metric.
+ I read in the discourse page some troubles with the CodaLab platform. I also noticed this behavior and it is quite reasonable for the first time of this competition to carry out.
+ In relation with that, some participants claimed that the same data upload twice returned remarkable different results in the final leaderboard. Something to be aware of too.
+ Other tecnhiques I may give a try:
  + Creating new examples from scratch printing them manually.
  + Analysing the train/dev sets provided to ensure they follow the same distribution. If not, try to fix that.
