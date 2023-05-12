# Deep Generative Chemistry 
A repository of update in generative chemistry with deep learning. Those efforts are cast into the following categories:

1. [Molecular Generation in 3D](#3DGen)  
2. [Molecular Generation in 1D (string-based)](#1DGen)
3. [Reviews](#reviews)
4. [Recent advances in Deep Diffusion Probabilistic Models ](#diffusion)

### 1. Molecular Generation in 3D <a name='3DGen'>
  [Equivariant Diffusion for Molecule Generation in 3D](https://arxiv.org/pdf/2203.17003.pdf) \
  Emiel Hoogeboom et al (2022) \
  This work introduces a diffusion model for molecule generation in 3D that is equivariant to Euclidean transformations. They generate both atom coordinates and element types. First paper introducing full molecule generation with Diffusion Models.
  
  [Geometry-Complete Diffusion for 3D Molecule Generation](https://arxiv.org/pdf/2302.04313.pdf) \
  Alex Morehead et al (2023) \
  This work proposes GCDM, a geometry-complete diffusion model that achieves new state-of-the-art results for 3D molecule diffusion generation and optimization by leveraging the representation learning strengths offered by GNNs that perform geometry-complete message-passing. 

### 1. Molecular Generation in 1D (string-based) <a name='1DGen'>
 [LibINVENT: Reaction Based Generative Scaffold Decoration for in silico Library Design](https://chemrxiv.org/engage/api-gateway/chemrxiv/assets/orp/resource/item/611f467d8a6faa8c529c5407/original/lib-invent-reaction-based-generative-scaffold-decoration-for-in-silico-library-design.pdf) \
 Vendy Fialková et al. (2021) \
  LibINVENT, a novel in silico tool, is introduced for de novo drug design. It generates chemical libraries with shared cores, maximizing desirable properties. Users can specify chemical reactions for library creation. The resulting compounds are similar, have desirable properties, and can be synthesized under similar conditions. The LibINVENT code is freely available online.
  
### 2. Reviews <a name='reviews'>
  [Generative Models as an Emerging Paradigm in the Chemical Sciences](https://pubs.acs.org/doi/10.1021/jacs.2c13467)\
  Dylan M. Anstine and Olexandr Isayev \
  (2023) \
  In this paper, the authors overview and critically analyze popular generative algorithms like generative adversarial networks, variational autoencoders, flow, and diffusion models. 

[Generative models for molecular discovery: Recent advances and challenges] (https://wires.onlinelibrary.wiley.com/doi/full/10.1002/wcms.1608) \
  Camille Bilodeau et al. (2022) \
  This text reviews the application of generative modeling in molecular design, a promising alternative to traditional, labor-intensive methods. It covers the choices required for generative model development and training, including various molecular representations and typical neural network architectures. It also explores different problem statements for molecular discovery applications and their corresponding benchmarks. Lastly, it discusses the integration of generative models into experimental workflows.
