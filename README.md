# Action-Recognition

Framework used: tensorflow keras

keras layers: convolution, pooling, dropout( avoid overfitting), flatten( convo to fully connected dense layer- 1D array)

optimizer='rmsprop', loss='categorical_crossentropy'( classification), metrics='accuracy' (classification metrics)

why not precision recall: two metrics is that both can only be used in specific scenarios since both of them identify only one set of errors. FP, FN
tradefoff.  we can deduce that precision and recall alone aren’t very good metrics to rely on and work with. 
F1 score is the harmonic mean of the two. With low F1, it’s unclear what the problem is (low precision or low recall?), and whether the model suffers from type-I or type-II error.
AUROC metric has no use other than academic research, and comparing different classifiers.

RMS prop is an advancement in AdaGrad optimizer as it reduces the monotonically decreasing learning rate. focuses on accelerating the optimization process by decreasing the number of function evaluations to reach the local minimum. The algorithm keeps the moving average of squared gradients for every weight and divides the gradient by the square root of the mean square. converges quickly and requires lesser tuning than gradient descent algorithms and their variants.

train: set pattern
validation: unbiasly evaluate model perfomance, tune hyperparameters
test: test on unseen data
