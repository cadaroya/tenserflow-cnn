# Tenserflow CNN Files
## TIPS

### 1. Define NN Variables and Flow (for easy documentation)

SAMPLE: Network Architecture 
- for MNIST handwritten numbers dataset
- basis: https://medium.com/data-science-group-iitr/building-a-convolutional-neural-network-in-python-with-tensorflow-d251c3ca8117

* Convolution, Filter shape:(5,5,6), Stride=1, Padding=’SAME’
* Max pooling (2x2), Window shape:(2,2), Stride=2, Padding=’Same’
* ReLU
* Convolution, Filter shape:(5,5,16), Stride=1, Padding=’SAME’
* Max pooling (2x2), Window shape:(2,2), Stride=2, Padding=’Same’
* ReLU
* Fully Connected Layer (128)
* ReLU
* Fully Connected Layer (10)
* Softmax


### 2. Define learning parameters
* Cost function - softmax/cross entropy, 
* Optimizer - AdamOptimizer
* Accuracy - reduce_mean,
* Learning rate
* Epochs
* Batch size (or just use mnist.next_batch() `deprecated`)


### 3. Build Model (CNN layers, weights, biases)

Basic:
- https://www.tutorialspoint.com/tensorflow/tensorflow_convolutional_neural_networks.htm
- https://github.com/aymericdamien/TensorFlow-Examples/blob/master/examples/3_NeuralNetworks/convolutional_network_raw.py
- I like the 2nd one better





FAQS:

1.  How to choose filter shape? (https://stackoverflow.com/questions/40025382/why-does-convolution-over-a-5x5-image-with-a-2x2-filter-produce-32-features-in-t/40027473)
2   What are input channels? (https://www.quora.com/What-do-channels-refer-to-in-a-convolutional-neural-network)
3.  How to choose output channels? (https://stats.stackexchange.com/questions/380996/convolutional-network-how-to-choose-output-channels-number-stride-and-padding/381032)
