# DTW Template
Implementation of 'Exact indexing of dynamic time warping' - Keogh / Ann Ratanamahatana
http://www.cs.ucr.edu/~eamonn/KAIS_2004_warping.pdf


A classifier of time series based on dynamic time warping is built. To improve performance
Keogh Lower Bound and a classification system based on templates is implemented. As proved in
the paper, these modifications make classifying a time series linear in complexity.


Main.trainDTW function receives the training set and the list of labels to detect. It returns
a data structure composed of templates for each label. Given a new sample, it predicts its label
by finding the most similar template.
