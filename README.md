I conducted a comparison between two neural networks that are identical except for the presence of a convolutional layer. In the model containing the convolutional layer, we achieved an accuracy of 0.9687 after 10 epochs. Conversely, the model without the convolutional layer only reached an accuracy of 0.0581 in the same timeframe. This discrepancy is logical because convolutional layers are specifically designed to extract intricate features and analyze spatial patterns, making them particularly effective for tasks involving the recognition of complex shapes in traffic-related data.

Additionally, elevating the number of filters in the convolutional layer from 32 to 40 resulted in enhanced accuracy for both the training and testing datasets.(for example in testing data : accuracy = 0.9245 improving to -> 0.9329 ) This improvement is coherent since increasing the number of filters allows the neural network to learn a broader range of features, thereby enhancing its ability to understand and represent the underlying patterns in the data .
Raising the number of filters from 40 to 70 resulted in a decrease in accuracy for the testing data, dropping from 0.9329 to 0.9298. This decline can be attributed to overfitting, where the model becomes too tailored to the training data, making it less adept at generalizing to new, unseen data.










