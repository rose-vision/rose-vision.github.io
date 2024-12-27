---
title: "Research"
draft: false

lightgallery: true

math:
  enable: true
---

In this pape, we will introduce several representive works in our group.

## Mitigating the Trade-off Problem between Nature Accuracy and Adversarial Robustness

Deep neural networks (DNNs) can achieve excellent performance on various complex tasks. However, recent studies have found that deep neural networks face serious security risks, namely adversarial attacks. Adversarial attacks refer to adding subtle perturbations to input data that are imperceptible to humans, causing deep neural networks to produce wrong outputs. Current research often faces difficulties in the Trade-off between accuracy and adversarial robustness, as well as the Trade-off between overall robustness and worst robustness (fairness issues), which poses challenges for DNNs in practical applications. Therefore, finding effective methods to address those difficult trade-off phenomena, is an urgent and challenging issue in deep learning.

![framework1](/research/framework_1.jpg)

This direction aims to address the challenge of balancing the adversarial robustness of deep neural networks. The specific research content includes the following three aspects: Aiming at mitigating the Trade-off from network architecture, (1) a robust neural network architecture design based on a dynamic routing mechanism is proposed: Based on dynamic neural network architecture, the design of an inference model sensitive to input data, adaptively select the optimal network inference path and weight parameters for inference. Aiming at mitigating the Trade-off between accuracy and adversarial robustness, (2) an adversarial training method for multi-teacher network collaborative knowledge distillation is proposed: For dynamic neural network architecture, adopt teacher models with strong adversarial robustness and accuracy, responsible for weight training of adversarial examples and clean examples, respectively. Aiming at enhancing robust fairness, (3) an adversarial robustness distillation method based on anti-bias soft labels is proposed: Hard and easy classes are guided by teacher labels with different smoothness degrees, which are controlled by temperatures.



