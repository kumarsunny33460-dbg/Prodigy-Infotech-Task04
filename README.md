Task 04 – Conditional GAN (cGAN) for Image-to-Image Translation
📌 Project Overview
This project is part of my internship at Prodigy Infotech.
In this task, I implemented a Conditional Generative Adversarial Network (cGAN) using the Pix2Pix architecture to perform image-to-image translation on the CMP Facades dataset.
The goal was to train a model that can translate edge maps of buildings into realistic facade images.
________________________________________
📂 Dataset
•	CMP Facades Dataset – provided by Czech Technical University.
•	Contains paired images of building facades and their edge maps.
•	Used for supervised training of Pix2Pix.
________________________________________
🛠️ Methodology
•	Framework: PyTorch
•	Generator: U-Net architecture with skip connections
•	Discriminator: PatchGAN (classifies image patches as real/fake)
•	Loss Functions:
o	Adversarial Loss
o	L1 Reconstruction Loss
•	Optimizer: Adam (lr = 0.0002, β1 = 0.5)
•	Training: 20 epochs on GPU (Google Colab CUDA support)
________________________________________
🚀 Results
The model showed progressive improvement in generating realistic facades from edge maps.
Sample Outputs
•	Epoch 1: Blurry, unclear structures![1](https://github.com/user-attachments/assets/1fbccd42-e716-4704-9ade-62fc333f53e5)


•	Epoch 5: More details visible, but artifacts remain ![5](https://github.com/user-attachments/assets/9bead936-839a-4b19-9834-74e510a495ab)

•	Epoch 20: Clear and realistic building facades![20](https://github.com/user-attachments/assets/868d9f6d-8759-4c60-88d8-2cfa6378c2c3)
 
________________________________________
📌 Applications
•	Architectural design automation
•	Urban planning visualization
•	Satellite imagery enhancement
•	Artistic sketch-to-photo generation

📖Reference
1.	Goodfellow, I., et al. (2014). Generative Adversarial Networks.
2.	Isola, P., Zhu, J., Zhou, T., & Efros, A. A. (2017). Image-to-Image Translation with Conditional Adversarial Networks (Pix2Pix).
3.	CMP Facades Dataset – Czech Technical University.
________________________________________
✍️ Author: Sunny Kumar
📚 Course: B.Tech CSE, 2nd Year
🎯 Internship: Prodigy Infotech – Task 04

