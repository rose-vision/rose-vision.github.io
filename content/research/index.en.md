---
title: "Research"
draft: false

lightgallery: true

math:
  enable: true
---

In this page, we will introduce several representive works in our group.

## Robustness

We mainly focus on the Out-Of Distribution (OOD) robustness of vision models. 

Viewpoint Robustness of Vision Models: Obtaining robust and invariant representations has been a longstanding challenge in the field of computer vision. Previous deep learning research on robustness has largely concentrated on adversarial perturbations under the L-p norm. However, in complex and dynamic physical environments, there exist many natural perturbations worthy of investigation, among which 3D viewpoint transformations are a particularly important factor. Studying model robustness under natural viewpoint changes holds significant relevance for safety-critical applications in areas such as autonomous driving and embodied robotics.

<div class="framework">
<img src="/research/framework_2.jpg">
</div>

This direction focuses on investigating the robustness and invariance of existing deep learning-based vision models in the face of viewpoint transformations. It currently consists of four components: (1) Viewpoint robustness evaluation methods, which utilizes multi-view 3D reconstruction approaches such as neural radiance fields to capture the model’s worst-case viewpoint distribution. (2) An extreme/adversarial viewpoint sample generation method for producing realistic adversarial viewpoint examples. (3) A viewpoint-invariant adversarial training (VIAT) approach designed to enhance the viewpoint invariance of traditional single-task visual models via adversarial distribution training. (4) A viewpoint-invariant fine-tuning method for vision-language pre-trained (VLP) models. By performing cross-viewpoint alignment on a large-scale multi-view image-text dataset, we enhance the viewpoint-invariant representation capability of VLP models.


## Security

We mainly focus on the adversarial attacks and defense of vision models. 

Adversarial Attack: Geometry-Aware Adversarial Patches in the Physical World

Adversarial Patch is an important form of adversarial attack in the physical world. However, the current adversarial patch methods mainly optimize the patch's texture to achieve attacks (we call them as Texture-Aware Adversarial Patches). These physical attacks encounter several significant challenges. Firstly, these attacks often take the form of irregular noise patterns, which lack naturalness and make them less covert in real-world scenarios. Secondly, when transitioning from the digital space to the physical domain, the attack patterns are prone to distortions, compromising their effectiveness. Additionally, environmental factors such as variations in shooting angles, lighting conditions, and distances during real-world implementations can introduce further distortions, making it difficult to maintain consistency and reliability. These challenges highlight the complexity of designing robust physical attacks in real-world applications.

<div class="framework">
<img src="/research/framework_3.jpg">
</div>

To meet these challenges, our group proposes the Geometry-Aware Adversarial Patches in the Physical World by adversarially optimizing the geometric attributes of patches, such as their location, rotation and shape, etc., we create more natural and imperceptible adversarial patch attacks. This form of adversarial patch can improve the robustness of adversarial attacks in the physical world effectively. The representative works in our group in this direction are as follows: (1) Location-aware Adversarial stickers for face recognition models, which optimizes the location and rotation of existing meaning stickers on the object to perform physical attacks. (2) Shape-aware Adversarial Patches, which can be applied on the visible and infrared domain at the same time, and thus achieving the cross-modal physical attacks. (3) Texture-Geometry joint adversarial patches, where we show that the proposed geometry-aware adversarial patch can also combine the traditional texture-aware adversarial patch, and thus achieving better attack performance.  

Adversarial Defense: Trade-off between Nature Accuracy and Adversarial Robustness

Deep neural networks (DNNs) can achieve excellent performance on various complex tasks. However, recent studies have found that deep neural networks face serious security risks, namely adversarial attacks. Adversarial attacks refer to adding subtle perturbations to input data that are imperceptible to humans, causing deep neural networks to produce wrong outputs. Current research often faces difficulties in the Trade-off between accuracy and adversarial robustness, as well as the Trade-off between overall robustness and worst robustness (fairness issues), which poses challenges for DNNs in practical applications. Therefore, finding effective methods to address those difficult trade-off phenomena, is an urgent and challenging issue in deep learning.

<div class="framework">
<img src="/research/framework_1.jpg">
</div>


This direction aims to address the challenge of balancing the adversarial robustness of deep neural networks. The specific research content includes the following three aspects: Aiming at mitigating the Trade-off from network architecture, (1) a robust neural network architecture design based on a dynamic routing mechanism is proposed: Based on dynamic neural network architecture, the design of an inference model sensitive to input data, adaptively select the optimal network inference path and weight parameters for inference. Aiming at mitigating the Trade-off between accuracy and adversarial robustness, (2) an adversarial training method for multi-teacher network collaborative knowledge distillation is proposed: For dynamic neural network architecture, adopt teacher models with strong adversarial robustness and accuracy, responsible for weight training of adversarial examples and clean examples, respectively. Aiming at enhancing robust fairness, (3) an adversarial robustness distillation method based on anti-bias soft labels is proposed: Hard and easy classes are guided by teacher labels with different smoothness degrees, which are controlled by temperatures.




<style>
    .framework {
        width: auto;
        height: auto;
        display: flex;
        /* border-radius: 50%; */
        align-items: center;
        justify-content: center;
        overflow: hidden;
        float: left;
        margin-left: 80px;
        margin-right: 80px;
        margin-bottom: 10px;
    }
</style>
