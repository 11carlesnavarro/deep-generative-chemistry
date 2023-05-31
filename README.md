# Deep Generative Chemistry 
A repository of update in generative chemistry with deep learning. Those efforts are cast into the following categories:

1. [Molecular Generation in 3D](#3DGen)  
2. [Molecular Generation in 1D (string-based)](#1DGen)
3. [Reviews](#reviews)
4. [Recent advances in Deep Diffusion Probabilistic Models ](#diffusion)
5. [The Foundations](#diffoundations)

### 1. Molecular Generation in 3D <a name='3DGen'></a>
  [Equivariant Diffusion for Molecule Generation in 3D](https://arxiv.org/pdf/2203.17003.pdf) \
  Emiel Hoogeboom et al (2022) \
  This work introduces a diffusion model for molecule generation in 3D that is equivariant to Euclidean transformations. They generate both atom coordinates and element types. First paper introducing full molecule generation with Diffusion Models.
  
  [Geometry-Complete Diffusion for 3D Molecule Generation](https://arxiv.org/pdf/2302.04313.pdf) \
  Alex Morehead et al (2023) \
  This work proposes GCDM, a geometry-complete diffusion model that achieves new state-of-the-art results for 3D molecule diffusion generation and optimization by leveraging the representation learning strengths offered by GNNs that perform geometry-complete message-passing. 
  
  [Geometric Latent Diffusion Models for 3D Molecule Generation](https://arxiv.org/pdf/2305.01140.pdf) \
  Minkai Xu et al (2023) \
  This paper introduces Geometric Latent Diffusion Models (GEOLDM), the first latent diffusion model for 3D molecular geometry. GEOLDM uses autoencoders to encode structures into continuous latent codes, while the diffusion models operate in the latent space. The model captures critical roto-translational equivariance constraints of 3D molecular geometries through a point-structured latent space. GEOLDM shows improved performance in multiple molecule generation benchmarks and allows for more controllable generation due to the latent modeling.
 
[MolDiff: Addressing the Atom-Bond Inconsistency Problem in 3D Molecule Diffusion Generation](https://arxiv.org/pdf/2305.07508.pdf) \
Xingang Peng et al. (2023)
This research highlights the issue of atom-bond inconsistency in 3D molecule generation, a problem that occurs when atoms are generated without considering potential bonds, resulting in unrealistic 3D molecules. To address this, the authors propose MolDiff, a new diffusion model capable of simultaneously generating atoms and bonds, thereby maintaining consistency by explicitly modeling their interdependence. The model was evaluated based on both geometry and chemical properties, and it significantly outperformed previous approaches, tripling the success rate and yielding molecules of markedly higher quality.

### 2. Molecular Generation in 1D (string-based) <a name='1DGen'></a>
 [LibINVENT: Reaction Based Generative Scaffold Decoration for in silico Library Design](https://chemrxiv.org/engage/api-gateway/chemrxiv/assets/orp/resource/item/611f467d8a6faa8c529c5407/original/lib-invent-reaction-based-generative-scaffold-decoration-for-in-silico-library-design.pdf) \
 Vendy Fialková et al. (2021) \
  LibINVENT, a novel in silico tool, is introduced for de novo drug design. It generates chemical libraries with shared cores, maximizing desirable properties. Users can specify chemical reactions for library creation. The resulting compounds are similar, have desirable properties, and can be synthesized under similar conditions. The LibINVENT code is freely available online.
  
  [REINVENT 2.0 – an AI Tool for De Novo Drug Design](https://chemrxiv.org/engage/chemrxiv/article-details/60c74f75bdbb89eaf7a39d8a) \
  Thomas Blaschke (2020) \
  This application note introduces a ready-to-use tool for de novo design in drug discovery, useful for addressing exploration or exploitation issues in chemical space navigation. By releasing the code.
  
  [Randomized SMILES Strings Improve the Quality of Molecular Generative Models](https://chemrxiv.org/engage/chemrxiv/article-details/60c743b14c8919d703ad26a1) \
  Josep Arús-Pous (2019) \
  This study benchmarks Recurrent Neural Networks (RNNs) for creating chemical spaces using SMILES representations and recurrent cell types. It found that LSTM models trained with 1 million randomized SMILES generate larger, more accurate chemical spaces. When trained on ChEMBL molecules, these models better represent drug-like chemical spaces, producing twice the unique molecules compared to canonical SMILES models.

### 3. Reviews <a name='reviews'></a>
  [Generative Models as an Emerging Paradigm in the Chemical Sciences](https://pubs.acs.org/doi/10.1021/jacs.2c13467)\
  Dylan M. Anstine and Olexandr Isayev \
  (2023) \
  In this paper, the authors overview and critically analyze popular generative algorithms like generative adversarial networks, variational autoencoders, flow, and diffusion models. 

[Generative models for molecular discovery: Recent advances and challenges](https://wires.onlinelibrary.wiley.com/doi/full/10.1002/wcms.1608) \
  Camille Bilodeau et al. (2022) \
  This text reviews the application of generative modeling in molecular design, a promising alternative to traditional, labor-intensive methods. It covers the choices required for generative model development and training, including various molecular representations and typical neural network architectures. It also explores different problem statements for molecular discovery applications and their corresponding benchmarks. Lastly, it discusses the integration of generative models into experimental workflows. 
  
[A Survey on Graph Diffusion Models: Generative AI in Science for Molecule, Protein and Material](https://arxiv.org/pdf/2304.01565.pdf) \
Mengchun Zhang et al. (2023) \
This work surveys the use of graph diffusion models, a cutting-edge generative modeling method. It provides a brief overview of other generative modeling methods applied to graphs and elucidates the mechanisms of various forms of diffusion models. It explores their applications, especially in the generation of molecules, proteins, and materials design in the realm of AI-generated scientific content. Furthermore, it discusses evaluation methods and the existing challenges in the graph domain.

### 4. Recent Advances in Deep Diffusion Probabilistic Models <a name='diffusion'></a>
[One Transformer Fits All Distributions in Multi-Modal Diffusion at Scale](https://arxiv.org/pdf/2303.06555.pdf) \
Fan Bao et al. (2023) \
The paper introduces UniDiffuser, a unified diffusion framework for fitting all distributions related to multi-modal data. The model predicts noise in perturbed data across different modalities, learning all distributions simultaneously with minimal modifications to the original diffusion model. UniDiffuser, parameterized by a transformer, is applied to large-scale paired image-text data, enabling various generation tasks by setting appropriate timesteps, without extra overhead. The model's performance, producing perceptually realistic samples and superior quantitative results, is not only better than existing general-purpose models but also comparable to specialized models like Stable Diffusion and DALL·E 2.

[Text-to-image Diffusion Models in Generative AI: A Survey](https://arxiv.org/pdf/2303.07909.pdf) \
Chenshuang Zhang et al. (2023) \
This survey provides an in-depth examination of text-to-image diffusion models, a prominent tool in various generative tasks. It begins by outlining the fundamentals of a basic diffusion model used for image synthesis and the ways conditioning or guidance enhance learning. The review then details the latest methods in text-conditioned image synthesis or text-to-image generation. Furthermore, it extends to applications beyond simple text-to-image generation, including text-guided creative generation and image editing. The survey concludes by discussing current challenges and potential future developments in the field.

### 4. The Foundations <a name='diffoundations'></a>
[SCORE-BASED GENERATIVE MODELING THROUGH STOCHASTIC DIFFERENTIAL EQUATIONS](https://arxiv.org/pdf/2011.13456.pdf) \
Yang Song et al. (2021) \
The authors introduce a framework that uses a stochastic differential equation (SDE) to transform complex data distributions to known prior ones and vice versa by gradually injecting and removing noise. This process depends on the time-dependent gradient field of the perturbed data distribution, and these transformations can be estimated accurately using advances in score-based generative modeling and neural networks. The paper also introduces a predictor-corrector framework to correct errors in the SDE evolution and an equivalent neural ODE that allows exact likelihood computation. These innovations enable the solution of inverse problems with score-based models and result in record-breaking performance in tasks such as unconditional image generation, class-conditional generation, image inpainting, and colorization.

[Elucidating the Design Space of Diffusion-Based Generative Models](https://arxiv.org/pdf/2206.00364.pdf) \
Tero Karras et al. (2022) \
The authors propose a simplification of the theory and practice of diffusion-based generative models, presenting a design space that clearly outlines design choices. This clarity enables improvements to the sampling and training processes and to the preconditioning of score networks. 

[GDDIM: GENERALIZED DENOISING DIFFUSION IMPLICIT MODELS](https://arxiv.org/pdf/2206.05564.pdf) \
Qinsheng Zhang et al. (2023) \
This research aims to extend the denoising diffusion implicit model (DDIM) to general diffusion models (DMs) beyond isotropic diffusions. The study interprets the accelerating effects of DDIM and the advantages of deterministic sampling for fast sampling. Based on these insights, the researchers introduce the generalized DDIM (gDDIM), a variation with a minor alteration in parameterizing the score network. The effectiveness of gDDIM is validated with two non-isotropic DMs: Blurring diffusion model (BDM) and Critically-damped Langevin diffusion model (CLD), with the former achieving more than 20 times acceleration. In the CLD model, the algorithm reaches impressive FID scores on CIFAR10 with a significantly reduced number of score function evaluations. 

[FAST SAMPLING OF DIFFUSION MODELS WITH EXPONENTIAL INTEGRATOR](https://arxiv.org/pdf/2204.13902.pdf) \
Qinsheng Zhang et al. (2023) \
This study seeks to address a significant limitation of Diffusion Models (DMs) in generative modeling tasks: their slow sampling procedure which often requires hundreds to thousands of time discretization steps for accurate results. The authors develop a fast sampling method, the Diffusion Exponential Integrator Sampler (DEIS), which maintains high sample quality with fewer steps. The DEIS, grounded in the Exponential Integrator designed for discretizing ordinary differential equations (ODEs), leverages the semi-linear structure of the learned diffusion process to reduce discretization error. This approach can be applied to any DM and can generate high-quality samples in as few as 10 steps.
