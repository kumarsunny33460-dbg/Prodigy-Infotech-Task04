Task 04 – Conditional GAN (cGAN) for Image-to-Image Translation
📌 Project Overview

This project is part of my internship at Prodigy Infotech.
In this task, I implemented a Conditional Generative Adversarial Network (cGAN) using the Pix2Pix architecture to perform image-to-image translation on the CMP Facades dataset.

The goal was to train a model that can translate edge maps of buildings into realistic facade images.

📂 Dataset

CMP Facades Dataset – provided by Czech Technical University.

Contains paired images of building facades and their edge maps.

Used for supervised training of Pix2Pix.

🛠️ Methodology

Framework: PyTorch

Generator: U-Net architecture with skip connections

Discriminator: PatchGAN (classifies image patches as real/fake)

Loss Functions:

Adversarial Loss

L1 Reconstruction Loss

Optimizer: Adam (lr = 0.0002, β1 = 0.5)

Training: 20 epochs on GPU (Google Colab CUDA support)

🚀 Results

The model showed progressive improvement in generating realistic facades from edge maps.

Sample Outputs


Epoch 1: Blurry, unclear structures![1](https://github.com/user-attachments/assets/af19b362-268b-4f79-9405-528b6a728b9c)


Epoch 5: More details visible, but artifacts remain![5](https://github.com/user-attachments/assets/5680c6dd-550a-4e39-b348-251037d83deb)


Epoch 20: Clear and realistic building facades![20](https://github.com/user-attachments/assets/61c91d40-1fa9-456a-8d6c-ee7d9981d018)


📌 Applications

Architectural design automation

Urban planning visualization

Satellite imagery enhancement

Artistic sketch-to-photo generation

📖 References

Goodfellow, I., et al. (2014). Generative Adversarial Networks.

Isola, P., Zhu, J., Zhou, T., & Efros, A. A. (2017). Image-to-Image Translation with Conditional Adversarial Networks (Pix2Pix).

CMP Facades Dataset – Czech Technical University.

✍️ Author: Sunny Kumar
📚 Course: B.Tech CSE, 2nd Year
🎯 Internship: Prodigy Infotech – Task 04
