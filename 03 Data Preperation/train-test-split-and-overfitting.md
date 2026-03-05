# Train-Test Split and Overfitting

In machine learning, it is important to evaluate how well a model performs on new, unseen data.

If we train and test a model on the same dataset, the model may simply memorize the data rather than learning useful patterns.

## Train-Test Split

To evaluate models properly, the dataset is divided into two parts:

Training Data:
Used to train the machine learning model.

Test Data:
Used to evaluate the model's performance on unseen data.

Typical split:
- 80% training data
- 20% testing data

## Overfitting

Overfitting occurs when a model learns the training data too well, including noise and small variations.

Symptoms:
- Very high training accuracy
- Low testing accuracy

This means the model does not generalize well to new data.

## Underfitting

Underfitting occurs when a model is too simple to capture patterns in the data.

Symptoms:
- Low training accuracy
- Low testing accuracy

## Trainer Notes

Explain using a student exam example:
Memorizing answers vs understanding concepts.
Imagine a student preparing for an exam.

## Case 1:
The student memorizes exact answers from the book.

If the exam contains the same questions, the student scores 100%.

But if the questions change slightly, the student fails.

That student has memorized, not understood.

Machine learning models can behave the same way.
To avoid this problem, we divide the dataset into two parts:

## Training Data

Used to train the model.

## Test Data

Used to evaluate the model.

## Typical split:

80% training

20% testing
Ask learners:
Why is testing on unseen data important?
