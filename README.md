# Poison-Mushroom-Classifier
Random Forest Classifier on Dataset of Poisonous &amp; Edible Mushrooms

In this personal project I implemented a random forest classifier in Python using Sci-Kit learn and Numpy packages. My goal was to classify a dataset of mushrooms labeled as poisonous or edible as accurately and safely as possible. Each decision tree in the ensemble model is constructed according to a greedy mutual information maximization (equivalent to entropy minimization) scheme over a random subset of the data. Specifically, I train each decision tree on a simple random sample of features from a boostrapped sample of the training data. In the training phase, I vary parameters such as decision tree depth, ensemble size, and sample sizes of features and training data.

These nominal models predict the test set with good accuracy, but fail when it comes to rare outcome detection and class robustness. To curb these limitations I also trained ensembles using the AdaBoost algorithm. This drives test error to nearly zero, AUC to nearly 1 and improves class-imbalance robustness metrics as well.
