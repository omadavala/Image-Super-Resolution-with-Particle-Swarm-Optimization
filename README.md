Image Super-Resolution using Particle Swarm Optimization (PSO) is an optimization-based approach aimed at reconstructing a high-resolution (HR) image from a given low-resolution (LR) input. 
Super-resolution is critical in domains such as medical imaging, satellite photography, surveillance, and digital forensics, where enhancing image clarity and detail is essential. 
In this method, PSO—a population-based metaheuristic inspired by the collective behavior of birds and fish—is used to iteratively search for the best possible HR image that, when downsampled, closely resembles the original LR image. 
Each particle in the swarm represents a candidate HR image, initialized by upsampling the LR image using bicubic interpolation and adding random perturbations. 
During each iteration, particles update their positions based on their own experience (personal best) and the experience of the swarm (global best), while a fitness function guides the search. 
This fitness function typically combines Peak Signal-to-Noise Ratio (PSNR) and Structural Similarity Index (SSIM) to assess how closely the generated HR image matches the original after downsampling. 
PSO’s ability to balance exploration and exploitation allows it to gradually enhance image details without the need for pretraining or large datasets, unlike deep learning approaches. 
This makes PSO a flexible and model-free technique that can be applied to various types of images. 
However, the approach can be computationally intensive and is generally slower than learning-based methods, especially on high-resolution images. 
Despite this, it often achieves noticeably better results than standard interpolation methods. For example, experimental results have shown improvements from a PSNR of 28.42 dB (bicubic) to 32.39 dB (PSO), 
and SSIM from 0.6501 to 0.7757, indicating a significant increase in both fidelity and perceptual quality.
