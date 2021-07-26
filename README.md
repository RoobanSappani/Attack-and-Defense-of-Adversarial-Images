# Attack-and-Defense-of-Adversial-Images
I have implemented three types of adversial attacks that can be used on a trained CNN model. To countermeasure these attacks, a defense algorithm is also implemented. The dataset is used is MNIST.

# Attack of Adversial Images

Adversarial examples are inputs to machine learning models that an attacker has intentionally designed to cause the model to make a mistake. They’re like optical illusions for machines.

I have implemented three types of white box attacks:

1. [Fast Gradient Sign Method](https://arxiv.org/abs/1412.6572)
2. [Iterative Fast Gradient Sign Method](https://arxiv.org/abs/1607.02533)
3. [Momentum Iterative Fast Gradient Sign Method](https://arxiv.org/abs/1710.06081)

Below given is the training and validation loss accross all the epochs.

![training](https://user-images.githubusercontent.com/63201896/126961865-2f891157-00a3-4ad0-85cf-27647235690f.png)

## Fast Gradient Sign Method

Test Accuracy after FGSM attack

![fgsm_graph](https://user-images.githubusercontent.com/63201896/126962188-4b0f9c4e-c556-4f42-a338-e037e6867b29.png)

Examples of some adversial images:

![fgsm_example](https://user-images.githubusercontent.com/63201896/126962298-9cb7be18-7caa-4458-81bb-eb055516b538.png)

## Iterative Fast Gradient Sign Method

Test Accuracy after I-FGSM attack

![ifgsm](https://user-images.githubusercontent.com/63201896/126962453-f9520943-a8f9-4428-b954-8b7e17a9f478.png)

Examples of some adversial images:

![ifgsm_example](https://user-images.githubusercontent.com/63201896/126962529-bf0e55a6-f0b0-4bb8-850e-b78b874dcbca.png)

## Momentum Iterative Fast Gradient Sign Method

Test Accuracy after MI_FGSM attack

![mifgsm_graph](https://user-images.githubusercontent.com/63201896/126962638-38158931-2140-4d8f-a106-d96987bcd5d8.png)

Examples of some adversial images:

![mifgsm_example](https://user-images.githubusercontent.com/63201896/126962737-271bcd75-6f66-466f-ad4e-1f573c032e36.png)

# Defense Distillation for Adversial Images

To countermeasure the above attacks, [distillation](https://arxiv.org/abs/1511.04508) was implemented.

# Results
