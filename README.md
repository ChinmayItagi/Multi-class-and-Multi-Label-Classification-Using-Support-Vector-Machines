# Multi-class-and-Multi-Label-Classification-Using-Support-Vector-Machines


1. Multi-class and Multi-Label Classification Using Support Vector Machines

(a) Download the Anuran Calls (MFCCs) Data Set from: https://archive.ics.
uci.edu/ml/datasets/Anuran+Calls+%28MFCCs%29. Choose 70% of the data
randomly as the training set.

(b) Each instance has three labels: Families, Genus, and Species. Each of the labels
has multiple classes. We wish to solve a multi-class and multi-label problem.
One of the most important approaches to multi-class classification is to train a
classifier for each label. We first try this approach:

i. Research exact match and hamming score/ loss methods for evaluating multi-
label classification and use them in evaluating the classifiers in this problem.

ii. Train a SVM for each of the labels, using Gaussian kernels and one versus
all classifiers. Determine the weight of the SVM penalty and the width of
the Gaussian Kernel using 10 fold cross validation. You are welcome to try
to solve the problem with both standardized 1 and raw attributes and report
the results.

iii. Repeat 1(b)ii and L 1 -penalized SVMs. 2 Remember to standardize 3 the at-
tributes

iv. Repeat 1(b)iii by using SMOTE or any other method you know to remedy
class imbalance. Report your conclusions about the classifiers you trained.

v. Extra Practice: Study the Classifier Chain method and apply it to the above
problem.

vi. Extra Practice: Research how confusion matrices, precision, recall, ROC,
and AUC are defined for multi-label classification and compute them for the
classifiers you trained in above.

2. K-Means Clustering on a Multi-Class and Multi-Label Data Set
Monte-Carlo Simulation: Perform the following procedures 50 times, and report
the average and standard deviation of the 50 Hamming Distances that you calculate.

(a) Use k-means clustering on the whole Anuran Calls (MFCCs) Data Set (do not
split the data into train and test, as we are not performing supervised learning in
this exercise). Choose k automatically based on one of the methods provided in
the slides (CH or Gap Statistics or scree plots or Silhouettes) or any other method
you know.

(b) In each cluster, determine which family is the majority by reading the true labels.
Repeat for genus and species.

(c) Now for each cluster you have a majority label triplet (family, genus, species).
Calculate the average Hamming distance (score) between the true labels and the
labels assigned by clusters.
