AIM: Manually compute forward and backward pass for a single sigmoid neuron and update weights. 
ALGORITHM :  Compute gradient of cross-entropy loss and update weights via gradient descent. 
DETAILED EXPLANATION :
1. Define input x and target y.
2.Initialize weights w and bias b, set learning rate lr.
3. sigmoid function computes activation.
4. Forward: compute z = w·x + b, a = sigmoid(z).
5. Loss: binary cross-entropy (single-sample).
6. Backprop: dz = a - y (derivative of loss wrt z for sigmoid+cross-entropy), dw = dz * x, db = dz.
7. Weight update: w_new = w - lr * dw.
8.  SAMPLE OUTPUT : a (output): 0.4502 loss: 0.8014 dw: [-0.275  0.66] db: -0.55 Updated w: [0.1275 -0.266] Updated b: 0.055

RESULT: Learners observe numeric gradients and weight updates; demystifies backpropagation. 
THEORY: Back propagation is chain rule application in neural nets; cross-entropy + sigmoid simplifies gradients. 
