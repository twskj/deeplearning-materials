The **training and validation** sets are used during **training**.

    for each epoch
        for each training data instance
            propagate error through the network
            adjust the weights
            calculate the accuracy over training data
        for each validation data instance
            calculate the accuracy over the validation data
        if the threshold validation accuracy is met
            exit training
        else
            continue training
            
            
Once you're finished training, then you run against your testing set and verify that the accuracy is sufficient.

Training Set: this data set is used to adjust the weights on the neural network.

Validation Set: this data set is used to minimize overfitting. You're not adjusting the weights of the network with this data set, you're just verifying that any increase in accuracy over the training data set actually yields an increase in accuracy over a data set that has not been shown to the network before, or at least the network hasn't trained on it (i.e. validation data set). If the accuracy over the training data set increases, but the accuracy over then validation data set stays the same or decreases, then you're overfitting your neural network and you should stop training.

Testing Set: this data set is used only for testing the final solution in order to confirm the actual predictive power of the network.

Taken from: http://stackoverflow.com/questions/2976452/whats-is-the-difference-between-train-validation-and-test-set-in-neural-networ
