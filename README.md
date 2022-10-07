# Predicting Major Subcellular Structures from a Transmitted Light Image using Diffusion Models

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/12zjYQ033V8n05D-SITDUZxXbxgK_u0EZ)

Fluorescence microscopy have many application, especially in healthcare field. But they are often expensive, time-consuming, and damaging to cells. So, a potential solution is to use transmitted light image which is relatively low cost to obtain and is label/dye free. But it lacks clear and specific contrast between different structures. So, my work explored the use of diffusion models to translate from transmitted light image to fluorescence image. Over traditional method, like U-net, my approach is also able to produce variance maps since I'm trying to predict the entire target image distribution.

### Diffusion Sampling Output - Example -Transmitted Light Image to Fluorescent Target(TOM20 labeled with Alexa Fluor 594):

##### Dataset credit: Spahn, C., & Heilemann, M. (2020). ZeroCostDL4Mic - Label-free prediction (fnet) example training and test dataset (Version v2) [Data set]. Zenodo. https://doi.org/10.5281/zenodo.3748967

Input Transmitted Light Image     | Ground Truth Fluorescent Target (TOM20)|  Diffusion Model Sampling Process 
:-------------------------:|:-------------------------:|:-------------------------:
![](https://user-images.githubusercontent.com/30499524/194135624-5fb52acf-9672-442d-801a-a3c5cc02687f.jpg) | ![ (5)](https://user-images.githubusercontent.com/30499524/194135737-0587f546-5b3d-4ae3-aaf6-924d317b6cd2.jpg) | ![](https://user-images.githubusercontent.com/30499524/194133483-f3897ba4-f7af-4d63-8b0a-3e047651fe85.gif) |
![visdom_image (2)](https://user-images.githubusercontent.com/30499524/194136017-83472a77-9034-4577-86e3-313c992937aa.jpg) | ![visdom_image (3)](https://user-images.githubusercontent.com/30499524/194136061-51eee711-6760-415b-bc40-7ae320798d5b.jpg) | ![](https://user-images.githubusercontent.com/30499524/194133858-73ddd43b-824f-4243-9d9d-d0e62f482250.gif)
![visdom_image (1)](https://user-images.githubusercontent.com/30499524/194136130-4ec441c1-9465-4f3d-8b22-1f493fe0c0c0.jpg) | ![visdom_image (4)](https://user-images.githubusercontent.com/30499524/194136178-301bfcf2-6916-4b4c-b63f-9cbe7c0ea8af.jpg) | ![](https://user-images.githubusercontent.com/30499524/194134903-098a3cf0-ae9b-4ad1-9076-74d6fcdc6a21.gif)



### Diffusion Sampling Output - Example - lifeact-RFP to sir-DNA:

Input Conditional Signal (lifeact-RFP)          | Ground Truth Target (sir-DNA) |  Diffusion Model Sampling Process 
:-------------------------:|:-------------------------:|:-------------------------:
![](https://user-images.githubusercontent.com/30499524/193465472-e0957c63-d05a-4a1b-91a9-b2c28fbc76e9.png)  | ![](https://user-images.githubusercontent.com/30499524/193465638-ee4dcd9b-61ca-44f5-8e11-ff1c52e9bde2.png) | ![](https://media1.giphy.com/media/5BdabGh0TVZKKnqezT/giphy.gif)
![](https://user-images.githubusercontent.com/30499524/193465403-ca1a16cf-abb4-41b9-a613-351d38b4faa2.png) | ![](https://user-images.githubusercontent.com/30499524/193465609-2c79b4ea-beea-4cdf-a225-db9deaa33892.png)| ![](https://media0.giphy.com/media/iUFuDEcPQrQ7MR4gMZ/giphy.gif)
![](https://user-images.githubusercontent.com/30499524/193465589-8a466613-adb6-4eb6-a88e-43d9f3253ad1.png) | ![](https://user-images.githubusercontent.com/30499524/193465646-bf15767d-67e7-4732-87d8-48fba0c0bbd2.png)| ![](https://media4.giphy.com/media/XHT4rO3MzVLpkabIx8/giphy.gif)

### Uncertainity Map for lifeact-RFP to sir-DNA:

![](https://raw.githubusercontent.com/raghuveerbhat/BrightFieldDiffusion/main/figures/mean_var_fig14.png)

### Architecture:

![](https://raw.githubusercontent.com/raghuveerbhat/BrightFieldDiffusion/main/figures/proposed_arch_fig10.png)

### Complete Report:
https://drive.google.com/file/d/15_wCXFuqHkFsNnH8OVUgwUu_2FYEw33r/view?usp=sharing

Credits:
1. Prafulla Dhariwal, and Alex Nichol 2021. Diffusion Models Beat GANs on Image Synthesis. CoRR, abs/2105.05233. (https://arxiv.org/abs/2105.05233)
   And source code found in: https://github.com/openai/guided-diffusion
2. https://github.com/junyanz/pytorch-CycleGAN-and-pix2pix - For the discriminator network architecture
3. Weng, Lilian. (Jul 2021). What are diffusion models? Lil’Log. https://lilianweng.github.io/posts/2021-07-11-diffusion-models/
4. Also many thanks to my supervisor Dr.Iain Styles(https://www.cs.bham.ac.uk/~ibs/) without whom this work wouldn't be done. His constant assistance and guidance at every stage of the research was immensely helpful. Also thanks to Dr. Carl Wilding (https://uk.linkedin.com/in/carl-wilding-4048a5101) for providing constructive feedback on my project.

For complete credits please refer my report. For any issues please feel free to contact me, and i'll try to respond.
