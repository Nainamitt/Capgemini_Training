Optimizer = Method that adjusts model parameters to reduce prediction error.

How an Optimizer Works

Training a neural network follows these steps:

Forward Pass – Input data passes through the network to produce predictions.

Loss Calculation – Difference between predicted output and actual output is computed using a loss function.

Backward Pass (Backpropagation) – Gradients of the loss with respect to weights are calculated.

Optimizer Step – The optimizer updates weights using gradients to reduce the loss.

Basic update rule:

w=w−η×∇L

Where:

w = weight

η (eta) = learning rate

∇L = gradient of loss


Camparision of Optimizer

| Optimizer        | Speed     | Stability | Usage          |
| ---------------- | --------- | --------- | -------------- |
| Gradient Descent | Slow      | Stable    | Small datasets |
| SGD              | Fast      | Noisy     | Large datasets |
| SGD + Momentum   | Faster    | Better    | CNNs           |
| RMSProp          | Fast      | Good      | RNNs           |
| Adam             | Very Fast | Excellent | Most DL models |


Real Life Analogy

Imagine climbing down a mountain to reach the lowest point.

Gradient Descent → Walk slowly using the full map

SGD → Take steps based on local ground

Momentum → Gain speed while moving downhill

Adam → Smart navigation using past direction + terrain
