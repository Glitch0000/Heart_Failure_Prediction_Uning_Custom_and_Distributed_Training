# Heart_Failure_Prediction_Uning_Custom_and_Distributed_Training
In this rrpository, we will train a neural network on the Heart failure clinical records Data Set to predict if the patient will die or live in the followed-up period. We are going to model this problem as a binary classification problem which detects whether the patient will live or die in the follow-up periodm, based on the other features.  This example is built using custom training, but we could've used the pre-made keras fucnctions for training like model.comple and model.fit. The core of custom training is using the model to calculate the logits on specific set of inputs and compute the loss(in this case binary crossentropy) by comparing the predicted outputs to the true outputs. We then update the trainable weights using the optimizer algorithm chosen. The optimizer algorithm requires our computed loss and partial derivatives of loss with respect to each of the trainable weights to make updates to the same. We'll use gradient tape to calculate the gradients and then update the model trainable weights using the optimizer.

