# Predicting Major Subcellular Structures from a Transmitted Light Image using Diffusion Models

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/12zjYQ033V8n05D-SITDUZxXbxgK_u0EZ)

### Diffusion Sampling Output Example for lifeact-RFP to sir-DNA:

Input Conditional Signal (lifeact-RFP)         |  Diffusion Model Sampling Process          | Ground Truth Target (sir-DNA)
:-------------------------:|:-------------------------:|:-------------------------:
![](https://user-images.githubusercontent.com/30499524/193465472-e0957c63-d05a-4a1b-91a9-b2c28fbc76e9.png) |  ![](https://media1.giphy.com/media/5BdabGh0TVZKKnqezT/giphy.gif) | ![](https://user-images.githubusercontent.com/30499524/193465638-ee4dcd9b-61ca-44f5-8e11-ff1c52e9bde2.png) |
![](https://user-images.githubusercontent.com/30499524/193465403-ca1a16cf-abb4-41b9-a613-351d38b4faa2.png)  |  ![](https://media0.giphy.com/media/iUFuDEcPQrQ7MR4gMZ/giphy.gif) | ![](https://user-images.githubusercontent.com/30499524/193465609-2c79b4ea-beea-4cdf-a225-db9deaa33892.png)|
![](https://user-images.githubusercontent.com/30499524/193465589-8a466613-adb6-4eb6-a88e-43d9f3253ad1.png) |  ![](https://media4.giphy.com/media/XHT4rO3MzVLpkabIx8/giphy.gif) | ![](https://user-images.githubusercontent.com/30499524/193465646-bf15767d-67e7-4732-87d8-48fba0c0bbd2.png)|

### Architecture:



Credits:
1. Prafulla Dhariwal, and Alex Nichol 2021. Diffusion Models Beat GANs on Image Synthesis. CoRR, abs/2105.05233. (https://arxiv.org/abs/2105.05233)
   And source code found in: https://github.com/openai/guided-diffusion
2. https://github.com/junyanz/pytorch-CycleGAN-and-pix2pix - For the discriminator network architecture
3. Also many thanks to my supervisor Dr.Iain Styles(https://www.cs.bham.ac.uk/~ibs/) without whom this work wouldn't be done. His constant assistance and guidance at every stage of the research was immensely helpful. Also thanks to Dr. Carl Wilding (https://uk.linkedin.com/in/carl-wilding-4048a5101) for providing constructive feedback on my project.
