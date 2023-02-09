For this homework, we consider the best subsets algorithm based on validation set MSE,
instead of based on our originally presented criteria, e.g., AIC. We’ll again use the prostate
data.

The Steps for testing the best regression model is as follows 

(1) Start with the model of size m = 0, the null model µb0(x) = βb0, estimated
by the mean of the inputs, yi
.
(2) At model size (step) m = 1, pick the single input xj
, j ∈ {1, 2, . . . , k},
that fits the output best in terms of some loss, e.g., RSS, evaluated on
the training data in a regression, µb1(x) = βb0 + βbjxj
. Set A1 = {xj}.
(A0 is empty, corresponding to the null model in step (1).)
(3) For each subset of inputs of size m ∈ {2, 3, . . . , M}, with M ≤ min(n−
1, k), identify the best subsets of m inputs, Am, when fitting a linear
model µb(x) = βb0 + xtAmβbAm with m of the k possible inputs in terms of
some loss, e.g., RSS.
(4) Use some external data or other means to select the ‘best’ amongst these
M models (i.e., subsets) of size m ∈ {1, 2, . . . , M}.
