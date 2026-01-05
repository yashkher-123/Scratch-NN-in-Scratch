To view code, either download file and load in Scratch, or go to https://scratch.mit.edu/projects/1260182823/. 

Fully connected neural network made and trained entirely from scratch in Scratch. 

To view model parameters and loss changing as the model trains, "see inside" and show the "mae list" and "weights" lists.

Early stopping when model loss gets low (mae < 0.6)

Note: Network doesn't use conventional backprop to train, when I tried that I kept getting exploding gradients.
I implemented a random search (hill-climbing) algorithm for its simplicity. 
The drawback is the minima that the loss settles into is completely by chance due to the random initialization of parameters, so even a decent loss is not guaranteed.

Keep the number of hidden layers and nodes per layer between 1 and 10 because training takes a while.

Network can perform simple regression and binary classification (sigmoid in output layer).

Highly recommended to make all activations ReLU.
