# Attack-and-Defense-of-Adversial-Images
I have implemented three types of adversial attacks that can be used on a trained CNN model. To countermeasure these attacks, a defense algorithm is also implemented. The dataset is used is MNIST.

# Attack of Adversial Images

Adversarial examples are inputs to machine learning models that an attacker has intentionally designed to cause the model to make a mistake. They’re like optical illusions for machines.

I have implemented three types of white box attacks:

1. [Fast Gradient Sign Method](https://arxiv.org/abs/1412.6572)
2. [Iterative Fast Gradient Sign Method](https://arxiv.org/abs/1607.02533)
3. [Momentum Iterative Fast Gradient Sign Method](https://arxiv.org/abs/1710.06081)

# Defense from Adversial Images

To countermeasure the above attacks, [distillation](https://arxiv.org/abs/1511.04508) was implemented.

# Results

Below given is the training loss accross all the epochs.

![training](https://user-images.githubusercontent.com/63201896/126961865-2f891157-00a3-4ad0-85cf-27647235690f.png)

