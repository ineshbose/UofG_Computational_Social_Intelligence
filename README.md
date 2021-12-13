# UofG Computational Social Intelligence (H)

This repository contains the coursework for CSI (H) (2021-22).

## Part 1

### Introduction

This is the __first part__ of the Assessed Exercise, the __second part__ would be handed out on November 18, 2021. The marking will be done over both parts.

The deadline for submission is December 3, 2021 at 17:00.

### The Data

The data (file "`laughter-corpus.csv`") is a collection of laughter events observed during 60 phone conversations between 120 unacquainted speakers. For every laughter event, the following information is available:

- Gender of the person that laughs: "Male" or "Female";
- Role of the person that laughs: "Caller" or "Receiver";
- Duration of the laughter events in seconds.

Out of 120 speakers, 57 are male and 63 are female. In terms of roles, 60 speakers are callers, and 60 receivers.

### The Assessed Exercise

Use appropriate statistical tests to answer the following questions:

- Is the number of laughter events higher for women than for men?
- Is the number of laughter events higher for callers than for receivers?
- Are laughter events longer for women?
- Are laughter events longer for callers?

For each of the above questions, the following tasks are expected to be performed:

- To formulate a clear research hypothesis and, correspondingly, a suitable null hypothesis;
- To select an appropriate statistical test among those that have been presented during the course;
- To explain whether the null hypothesis will be rejected and, if yes, what is the confidence level.
- To explain whether a two-tailed or a one-tailed test will be used and why.

Any programming language is free to use, but libraries that perform statistical tests are not allowed. Knowledge of calculating a statistic for the test needs to be shown.

### The Report

The report must include a general description of the problem and, for each of the above research questions, the following elements:

- Formulation of research hypothesis and corresponding null hypothesis;
- Description of the data, e.g., number of laughter occurrences for female and male subjects, average and variance of laughter length for female and male subjects, etc.;
- Description of the approach, e.g., which test? What are the parameters (degrees of freedom, expectations, etc.) and what is the motivation behind every choice (why a certain test? Why a certain value of the parameters?)
- Results of the hypothesis testing (can the null hypothesis be rejected? What is the confidence level? etc.);
- Explanation of the results (e.g., in case the test shows that the number of laughter events is higher for female subjects to a statistically significant extent, mentioning that the conclusion is that female subjects tend to laugh more than male ones);
- Analysis software written (the code must be added in appendix);

The report should not include more than one page per each of the questions to be addressed.

### Marking Scheme

The Assessed Exercise (including both first and second part) accounts for 20% of the final mark. The weight across the different components is as follows:

- Analysis of the data: 60%;
- Editorial quality: 20%;
- Quality of the code: 20%.

The two parts of the Assessed Exercise have the same weight (each accounting for 10% of the final mark).

### Submission Instructions

Only the report is expected to be submitted and `pdf` if the recommended format. However, any other format can be used if `pdf` cannot be generated (the only format that is not accepted is Jupyter Notebook). The submission must be performed via the Moodle Page of the course.

## Part 2

### Introduction

This is the __second part__ of the Assessed Exercise; the __first part__ was handed out on November 4, 2021. The marking will be done over both parts.

The deadline for submission is December 3, 2021.

### The Data

The data (files "`training-part-2.csv`" and "`test-part-2.csv`") includes 52 feature vectors extracted from 52 face images, split into training and test set. Half of the vectors (26) have been extracted from smiling faces, while the other half (26) have been extracted from faces of people displaying frown.

Every record of the `csv` files includes one feature vector and its respective class:

- The feature vectors include 17 components that account for the activation level of 17 Action Units (AU01, AU02, AU04, AU05, AU06, AU07, AU09, AU10, AU12, AU14, AU15, AU17, AU20, AU23, AU25, AU26, AU45);
- The class is either "smile" or "frown".

The minimum value of the features is zero (meaning that the muscles underlying an Action Unit are not active) and larger values correspond to higher activation.

### The Assessed Exercise

The goal of the second part of the exercise is to develop a classifier capable to automatically map every vector into its class:

- The classification approach must be based on Gaussian Discriminant Functions;
- The approach should make the assumption that the features are statistically independent given the class;
- The Gaussian Discriminant Functions must be trained over the training set and tested over the test set;
- The results have to be reported in terms of error rate, the percentage of times the approach maps a vector into the wrong class.

Any programming language is free to use, but the Gaussian Discriminant Functions must be implemented (the code must be attached to the report). The use of packages implemented the Gaussian Discriminant Functions is not allowed.

### The Report

The report must include the following elements:

- An introduction to the problem of facial expression analysis;
- A description of the theory underlying the Gaussian Discriminant Functions;
- A description of the experimental setup (training and test set, etc.);
- A description of the results;
- The software written (the code must be added in the appendix);

The report should not include more than one page per each of the points above.

### Marking Scheme

The Assessed Exercise (including both first and second part) accounts for 20% of the final mark. The weight accross the different components is as follows:

- Classification Experiments: 60%;
- Editorial quality: 20%;
- Quality of the code: 20%.

The two parts of the Assessed Exercise have the same weight (each accounts for 10% of the final mark).
