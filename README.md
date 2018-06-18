# Random-Forest-Algorithm
Machine Learning Algorithms

Let the number of training cases be N, and the number of variables in the classifier be M.
• We are told the number m of input variables to be used to determine the decision at a node of the
tree; m should be much less than M.
• Choose a training set for this tree by choosing n times with replacement from all N available
training cases (i.e. take a bootstrap sample). Use the rest of the cases to estimate the error of the
tree, by predicting their classes.
• For each node of the tree, randomly choose m variables on which to base the decision at that node.
Calculate the best split based on these m variables in the training set.
• Each tree is fully grown and not pruned (as may be done in constructing a normal tree classifier).
• For prediction, a new sample is pushed down the tree. It is assigned the label of the training sample
in the terminal node it ends up in. This procedure is iterated over all trees in the ensemble, and the
average vote of all trees is reported as random forest prediction.
