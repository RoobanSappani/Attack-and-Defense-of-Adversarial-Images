# Attack-and-Defense-of-Adversarial-Images
I have implemented three types of adversarial attacks that can be used on a trained CNN model. To countermeasure these attacks, a defense algorithm is also implemented. The dataset is used is MNIST.

# Attack of Adversarial Images

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

Examples of some adversarial images:

![fgsm_example](https://user-images.githubusercontent.com/63201896/126962298-9cb7be18-7caa-4458-81bb-eb055516b538.png)

## Iterative Fast Gradient Sign Method

Test Accuracy after I-FGSM attack

![ifgsm](https://user-images.githubusercontent.com/63201896/126962453-f9520943-a8f9-4428-b954-8b7e17a9f478.png)

Examples of some adversarial images:

![ifgsm_example](https://user-images.githubusercontent.com/63201896/126962529-bf0e55a6-f0b0-4bb8-850e-b78b874dcbca.png)

## Momentum Iterative Fast Gradient Sign Method

Test Accuracy after MI_FGSM attack

![mifgsm_graph](https://user-images.githubusercontent.com/63201896/126962638-38158931-2140-4d8f-a106-d96987bcd5d8.png)

Examples of some adversarial images:

![mifgsm_example](https://user-images.githubusercontent.com/63201896/126962737-271bcd75-6f66-466f-ad4e-1f573c032e36.png)

# Defense Distillation for Adversarial Images

To countermeasure the above attacks, [distillation](https://arxiv.org/abs/1511.04508) was implemented.

Below given is the training and validation loss for netowrkf and networkf1

![collage](https://user-images.githubusercontent.com/63201896/126963642-23b4a992-e479-4328-b81e-86ebe237c691.png)

## Defense against FGSM

Below is the Test accuracy after defending the FGSM attack

![defense_fgsm](https://user-images.githubusercontent.com/63201896/126964134-1b51042e-a8f2-4e9b-9547-517c08ca6b79.png)

Examples of the predicitions after defense:

![fgsm_defense_example](https://user-images.githubusercontent.com/63201896/126964391-379c946b-1ff0-4042-922d-aa53d4a5d967.png)

## Defense against I-FGSM

Below is the Test accuracy after defending the I-FGSM attack

![ifgsm_defense](https://user-images.githubusercontent.com/63201896/126964690-eb42c297-04f5-40ff-b492-ec915318c064.png)

Examples of the predicitions after defense:

![ifgsm_defense_example](https://user-images.githubusercontent.com/63201896/126964788-6c4fdd46-e338-4986-b7ab-3fc16bf67cd5.png)

## Defense against MI-FGSM

Below is the Test accuracy after defending the MI-FGSM attack

![mifgsm_defense](https://user-images.githubusercontent.com/63201896/126964928-f9b28f6d-b734-47da-b6d3-bc1b6c2d2c55.png)


Examples of the predicitions after defense:

![mifgsm_defense_example](https://user-images.githubusercontent.com/63201896/126965007-7237f9ca-02c1-4013-9f72-bdfcf7bc8e97.png)
