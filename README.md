# 🖼️ Image Processing Techniques: Inpainting, Steganography, and Adversarial Attacks  

This repository contains Jupyter notebooks covering three key image processing techniques: inpainting, steganography, and adversarial attacks.  

## 📌 Inpainting  
Reconstruction of missing image regions using classical methods:  
- **Navier-Stokes** – propagates information based on fluid dynamics equations, effective for smooth areas.  
- **Telea** – propagates pixel values using brightness minimization, often used for filling small gaps.  

Additionally, a **GAN-based model** has been used for more advanced image reconstruction. Details and code are available in a separate repository:  
🔗 [Link to GAN repository](https://github.com/tlatkowski/inpainting-gmcnn-keras)  

## 🔒 Steganography  
Implementation of information hiding in images using the Least Significant Bit (LSB) method.  
In this experiment, the four least significant bits of the carrier image were replaced with the four most significant bits of the embedded image.  

## ⚠️ Adversarial Attacks  
Evaluation of model robustness against adversarial attacks:  
- **Jacobian-based Saliency Map Attack (JSMA)** – manipulates selected image pixels to force misclassification.  
- **Synthesizing Robust Adversarial Examples** – generates adversarial examples that are more resistant to conventional defense techniques.  

## ⚙️ Requirements  
- Python 3.8+  
- OpenCV  
- NumPy, Matplotlib  
- Tensorflow/Keras (for adversarial attacks)  

# 📌 Most Popular Databases and Evaluation Metrics in Digital Masking Research  

Below is a list of the most commonly used databases and evaluation metrics in research related to digital masking, including inpainting, steganography, adversarial attacks, and the generation of synthetic images. The table provides references to publicly available datasets along with the key metrics used to assess the quality of results.  

## 📊 Databases and Evaluation Metrics  

<table>
  <tr>
    <th>Method</th>
    <th>Database</th>
    <th>Metric</th>
  </tr>
  <tr>
    <td rowspan="6"><b>Inpainting</b></td>
    <td><a href="https://www.image-net.org/">ImageNet</a> [1], [3], [4], [5], [6]</td>
    <td rowspan="6">Mean L1 Loss, Mean L2 Loss, PSNR, Total Variation (TV Loss), SSIM, FID, LPIPS, U-IDS, P-IDS</td>
  </tr>
  <tr>
    <td><a href="http://mmlab.ie.cuhk.edu.hk/projects/CelebA.html">CelebA</a> [3], [5], [6], [7], [8], [9], [10]</td>
  </tr>
  <tr>
    <td><a href="https://github.com/tkarras/progressive_growing_of_gans">CelebA-HQ</a> [2], [6], [8], [9], [11], [12], [13]</td>
  </tr>
  <tr>
    <td><a href="https://github.com/NVlabs/ffhq-dataset">FFHQ</a> [14], [15]</td>
  </tr>
  <tr>
    <td><a href="http://places.csail.mit.edu/">Places</a> [2], [12], [14], [15], [16], [17], [18], [19], [20], [21]</td>
  </tr>
  <tr>
    <td><a href="https://github.com/pathak22/context-encoder">Paris Street View</a> [16], [19], [20]</td>
  </tr>
  <tr>
    <td><b>Steganography</b></td>
    <td>Random images used in analyzed research</td>
    <td rowspan="2">SSIM, FID, PSNR</td>
  </tr>
  <tr>
    <td><b>Synthesizing Robust Adversarial</b></td>
    <td>Random images used in analyzed research</td>
  </tr>
  <tr>
    <td rowspan="5"><b>Generating False Images</b></td>
    <td><a href="https://www.cs.toronto.edu/~kriz/cifar.html">CIFAR-10</a> [22], [23], [24], [25], [26], [27]</td>
    <td rowspan="5">SSIM, FID, PSNR</td>
  </tr>
  <tr>
    <td><a href="https://www.image-net.org/">ImageNet</a> [26], [27], [28], [29], [30], [31], [32], [33]</td>
  </tr>
  <tr>
    <td><a href="http://mmlab.ie.cuhk.edu.hk/projects/CelebA.html">CelebA</a> [24], [27], [32], [33], [34]</td>
  </tr>
  <tr>
    <td><a href="https://github.com/tkarras/progressive_growing_of_gans">CelebA-HQ</a> [31], [32], [34]</td>
  </tr>
  <tr>
    <td><a href="https://github.com/NVlabs/ffhq-dataset">FFHQ</a> [23], [27]</td>
  </tr>
</table>

## References
[1] D. Pathak, P. Krahenbuhl, J. Donahue, T. Darrell, and A. A. Efros, ‘Context Encoders: Feature Learning by Inpainting’, in 2016 IEEE Conference on Computer Vision and Pattern Recognition (CVPR), Las Vegas, NV, USA: IEEE, Jun. 2016, pp. 2536–2544. doi: 10.1109/CVPR.2016.278.  
[2] R. Suvorov et al., ‘Resolution-robust Large Mask Inpainting with Fourier Convolutions’, Nov. 10, 2021, arXiv: arXiv:2109.07161. doi: 10.48550/arXiv.2109.07161.  
[3] J. Yu, Z. Lin, J. Yang, X. Shen, X. Lu, and T. S. Huang, ‘Generative Image Inpainting with Contextual Attention’, Mar. 21, 2018, arXiv: arXiv:1801.07892. Accessed: Mar. 11, 2024. [Online]. Available: http://arxiv.org/abs/1801.07892.  
[4]	P. Jeevan, D. S. Kumar, and A. Sethi, ‘WavePaint: Resource-efficient Token-mixer for Self-supervised Inpainting’, Jul. 01, 2023, arXiv: arXiv:2307.00407. Accessed: Mar. 11, 2024. [Online]. Available: http://arxiv.org/abs/2307.00407.  
[5]	Y. Wang, J. Yu, and J. Zhang, ‘Zero-Shot Image Restoration Using Denoising Diffusion Null-Space Model’, Dec. 07, 2022, arXiv: arXiv:2212.00490. doi: 10.48550/arXiv.2212.00490.  
[6]	X. Lu, R. Lu, W. Zhao, and E. Ma, ‘Facial image inpainting for big data using an effective attention mechanism and a convolutional neural network’, Frontiers in Neurorobotics, vol. 16, 2022, doi: 10.3389/fnbot.2022.1111621.  
[7]	J. Qin, H. Bai, and Y. Zhao, ‘Multi-scale attention network for image inpainting’, Computer Vision and Image Understanding, vol. 204, p. 103155, Mar. 2021, doi: 10.1016/j.cviu.2020.103155.  
[8]	A. Lahiri, A. K. Jain, S. Agrawal, P. Mitra, and P. K. Biswas, ‘Prior Guided GAN Based Semantic Inpainting’, in 2020 IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR), Jun. 2020, pp. 13693–13702. doi: 10.1109/CVPR42600.2020.01371.  
[9]	C. Han and J. Wang, ‘Face Image Inpainting With Evolutionary Generators’, IEEE Signal Processing Letters, vol. 28, pp. 190–193, 2021, doi: 10.1109/LSP.2020.3048608.  
[10]	C. Agarwal and C. Bhatnagar, ‘Unmasking the potential: evaluating image inpainting techniques for masked face reconstruction’, Multimed Tools Appl, vol. 83, no. 1, pp. 893–918, Jan. 2024, doi: 10.1007/s11042-023-15807-x.  
[11]	W. Quan, R. Zhang, Y. Zhang, Z. Li, J. Wang, and D.-M. Yan, ‘Image Inpainting With Local and Global Refinement’, IEEE Transactions on Image Processing, vol. 31, pp. 2405–2420, 2022, doi: 10.1109/TIP.2022.3152624.  
[12]	J. Yu, Z. Lin, J. Yang, X. Shen, X. Lu, and T. Huang, ‘Free-Form Image Inpainting with Gated Convolution’, Oct. 21, 2019, arXiv: arXiv:1806.03589. doi: 10.48550/arXiv.1806.03589.  
[13]	Z. Luo, F. K. Gustafsson, Z. Zhao, J. Sjölund, and T. B. Schön, ‘Image Restoration with Mean-Reverting Stochastic Differential Equations’, May 31, 2023, arXiv: arXiv:2301.11699. doi: 10.48550/arXiv.2301.11699.  
[14]	W. Li, Z. Lin, K. Zhou, L. Qi, Y. Wang, and J. Jia, ‘MAT: Mask-Aware Transformer for Large Hole Image Inpainting’, Jun. 26, 2022, arXiv: arXiv:2203.15270. doi: 10.48550/arXiv.2203.15270.  
[15]	S. Zhao et al., ‘Large Scale Image Completion via Co-Modulated Generative Adversarial Networks’, Mar. 18, 2021, arXiv: arXiv:2103.10428. doi: 10.48550/arXiv.2103.10428.  
[16]	M. Zhu et al., ‘Image Inpainting by End-to-End Cascaded Refinement with Mask Awareness’, IEEE Trans. on Image Process., vol. 30, pp. 4855–4866, 2021, doi: 10.1109/TIP.2021.3076310.  
[17]	Y. Zeng, Z. Lin, J. Yang, J. Zhang, E. Shechtman, and H. Lu, ‘High-Resolution Image Inpainting with Iterative Confidence Feedback and Guided Upsampling’, Jul. 14, 2020, arXiv: arXiv:2005.11742. doi: 10.48550/arXiv.2005.11742.  
[18]	Y. Zeng, Z. Lin, H. Lu, and V. M. Patel, ‘CR-Fill: Generative Image Inpainting with Auxiliary Contexutal Reconstruction’, Mar. 31, 2021, arXiv: arXiv:2011.12836. doi: 10.48550/arXiv.2011.12836.  
[19]	H. Liu, B. Jiang, Y. Xiao, and C. Yang, ‘Coherent Semantic Attention for Image Inpainting’, Jul. 04, 2019, arXiv: arXiv:1905.12384. Accessed: Mar. 11, 2024. [Online]. Available: http://arxiv.org/abs/1905.12384  
[20]	C. Xie et al., ‘Image Inpainting with Learnable Bidirectional Attention Maps’, Sep. 05, 2019, arXiv: arXiv:1909.00968. doi: 10.48550/arXiv.1909.00968.  
[21]	H. Zheng et al., ‘CM-GAN: Image Inpainting with Cascaded Modulation GAN and Object-Aware Training’, Jul. 20, 2022, arXiv: arXiv:2203.11947. doi: 10.48550/arXiv.2203.11947.  
[22]	D. Kim et al., ‘Consistency Trajectory Models: Learning Probability Flow ODE Trajectory of Diffusion’, Oct. 01, 2023, arXiv: arXiv:2310.02279. doi: 10.48550/arXiv.2310.02279.
[23]	Y. Xu, Z. Liu, Y. Tian, S. Tong, M. Tegmark, and T. Jaakkola, ‘PFGM++: Unlocking the Potential of Physics-Inspired Generative Models’, Feb. 10, 2023, arXiv: arXiv:2302.04265. doi: 10.48550/arXiv.2302.04265.  
[24]	S. Li, W. Chen, and D. Zeng, ‘SciRE-Solver: Accelerating Diffusion Models Sampling by Score-integrand Solver with Recursive Difference’, Sep. 11, 2023, arXiv: arXiv:2308.07896. doi: 10.48550/arXiv.2308.07896.  
[25]	M. Ning, M. Li, J. Su, A. A. Salah, and I. O. Ertugrul, ‘Elucidating the Exposure Bias in Diffusion Models’, Oct. 10, 2023, arXiv: arXiv:2308.15321. doi: 10.48550/arXiv.2308.15321.  
[26]	A. Brock, J. Donahue, and K. Simonyan, ‘Large Scale GAN Training for High Fidelity Natural Image Synthesis’, Feb. 25, 2019, arXiv: arXiv:1809.11096. doi: 10.48550/arXiv.1809.11096.  
[27]	D. Kim, Y. Kim, S. J. Kwon, W. Kang, and I.-C. Moon, ‘Refining Generative Process with Discriminator Guidance in Score-based Diffusion Models’, Jun. 04, 2023, arXiv: arXiv:2211.17091. doi: 10.48550/arXiv.2211.17091.  
[28]	S. Gao, P. Zhou, M.-M. Cheng, and S. Yan, ‘MDTv2: Masked Diffusion Transformer is a Strong Image Synthesizer’, Feb. 21, 2024, arXiv: arXiv:2303.14389. Accessed: Mar. 11, 2024. [Online]. Available: http://arxiv.org/abs/2303.14389  
[29]	H. Chang, H. Zhang, L. Jiang, C. Liu, and W. T. Freeman, ‘MaskGIT: Masked Generative Image Transformer’, Feb. 08, 2022, arXiv: arXiv:2202.04200. doi: 10.48550/arXiv.2202.04200.  
[30]	A. Nichol and P. Dhariwal, ‘Improved Denoising Diffusion Probabilistic Models’, Feb. 18, 2021, arXiv: arXiv:2102.09672. doi: 10.48550/arXiv.2102.09672.  
[31]	J. Teng et al., ‘Relay Diffusion: Unifying diffusion process across resolutions for image synthesis’, Sep. 04, 2023, arXiv: arXiv:2309.03350. doi: 10.48550/arXiv.2309.03350.  
[32]	Z. Xiao, K. Kreis, J. Kautz, and A. Vahdat, ‘VAEBM: A Symbiosis between Variational Autoencoders and Energy-based Models’, Nov. 04, 2021, arXiv: arXiv:2010.00654. doi: 10.48550/arXiv.2010.00654.  
[33]	P. Esser, R. Rombach, and B. Ommer, ‘Taming Transformers for High-Resolution Image Synthesis’, Jun. 23, 2021, arXiv: arXiv:2012.09841. Accessed: Mar. 11, 2024. [Online]. Available: http://arxiv.org/abs/2012.09841  
[34]	D. P. Kingma and P. Dhariwal, ‘Glow: Generative Flow with Invertible 1x1 Convolutions’, Jul. 10, 2018, arXiv: arXiv:1807.03039. doi: 10.48550/arXiv.1807.03039.  
