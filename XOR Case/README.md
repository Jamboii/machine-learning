# XOR Case with ReLU Activation
A 2-layer implementation of the XOR case using a 2-neuron hidden layer. This network only tests the manually computed weights of the layer connections which were found using paper and pencil. The logic for an XOR function is as follows:

y = ~(x1 * x2) * (x1 + x2) = AND(NAND(x1,x2), OR(x1,x2))

The network defines test points between the region of (-1,-1) and (+1,+1), where any point in quadrant 1 or 3 belongs to the +1 class, and any point in quadrant 2 or 4 belongs to the -1 class. Since this network uses ReLU activations at each layer, the class of the prediction is defined using a threshold function. If the value at the output layer <= 0, then the class belongs to -1; else, the class belongs to +1.

