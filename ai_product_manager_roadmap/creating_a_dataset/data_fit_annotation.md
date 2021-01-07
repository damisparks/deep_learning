# Data Fit and Annotation

This article covers how data can affect a machine learning model's performance and see how to create your labelled dataset using Appen's annotation platform.

> Data Annotation is also known as Data Labelling.

## Scope

By the end of the article, you should have the essential information you need to build a data annotation of your own.

## Answering Questions with Data.

### Building a dataset.

In this section, I discuss how you can build a dataset with the business problem.

When building a dataset for the problem, ask yourself :

- does the dataset fit the problem
- is the dataset complete (_whether a data-set is complete and if it contains enough information to represent all real world use cases_)
- how can you annotate a dataset and ensure the data quality and user experience over time (_strategy for ensuring data quality and user experience_)

## As Good as your data.

Your model is as good as your data.

There is a concept in computer science that says :
**Garbage in, Garbage out**

> _Garbage in, garbage out (GIGO) describes the concept that flawed, or nonsense input data produces nonsense output or 'garbage - [reference](https://en.wikipedia.org/wiki/Garbage_in,_garbage_out)_

The size of your data is essential. If you are using a **deep learning** algorithm, as opposed to some traditional machine learning techniques, data size is even more important.

Deep learning (**neural networks**) often need to see many samples of every possible category before they can learn to distinguish different classes of data and find general patterns in some data.

If few or not evenly distributed data points, you could get some significant [sampling bias](https://en.wikipedia.org/wiki/Sampling_bias) in your end predictions; _predictions that are biased towards classifying all data into one class_

## Ensuring Data Fit.

To ensure data fit,

- Use production data to ensure the training data matches real-world scenarios.
- Determine the success criteria for a trained model:
  - Precision
  - Recall
  - F1 Score.
  - _If not met --> re-train, go back to the data._

I wrote an article on [Medium daminotes](https://daminotes.medium.com/understanding-precision-recall-f1-score-and-confusion-matrix-b701659b9a21) on how to understand these concepts.

## Data Completeness

Not only does your data need to match the reality of your problem, it needs to be complete. As much as possible, it needs to represent all scenarios that could come up in real-world data.

Narrow down how you want to ensure data completeness.
Start with :

- what is the problem you're trying to solve, and how does it benefit your end-users?
- what data will help you solve that problem?
  - collect data and observe relationships, patterns and similarities among the data.
  - identify potential anomalies or missing data.
- Conduct research and get the best data to serve your use case.

## Case Study

An example of case study is **Parking Signs Detention**.
You can use **[Figure Eight](https://www.figure-eight.com/platform/)**
You can create an Appen account by going to their Client Workspace [homepage](https://client.appen.com/users/new) and creating an account for yourself.

## Planning For Failure.

You may not be able to train your model on all the possible data points.
So, you will need to design for **unknown cases**.

How do you handle cases the model has not seen before?
The answer is :

- Design an option with the least negative impact.

## Planning For Longevity.

Since real continuous data also changes all the time.
So how can you plan for long-term success?

If your dataset does not change, then you can use a static model which is trained once and used indefinitely until an update is required.

For ever-evolving data, which is common, you should use dynamic model

- Continuously trained on new datasets so it can keep learning.

For frequently changing data, you may need to change
your annotation job to reflect more relevant definitions or examples.

..:TBC
