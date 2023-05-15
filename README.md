# Deep Generative Chemistry 
A repository of update in generative chemistry with deep learning. Those efforts are cast into the following categories:

1. [Molecular Generation in 3D](#3DGen)  
2. [Molecular Generation in 1D (string-based)](#1DGen)
3. [Reviews](#reviews)
4. [Recent advances in Deep Diffusion Probabilistic Models ](#diffusion)

### 1. Molecular Generation in 3D <a name='3DGen'></a>
  [Equivariant Diffusion for Molecule Generation in 3D](https://arxiv.org/pdf/2203.17003.pdf) \
  Emiel Hoogeboom et al (2022) \
  This work introduces a diffusion model for molecule generation in 3D that is equivariant to Euclidean transformations. They generate both atom coordinates and element types. First paper introducing full molecule generation with Diffusion Models.
  
  [Geometry-Complete Diffusion for 3D Molecule Generation](https://arxiv.org/pdf/2302.04313.pdf) \
  Alex Morehead et al (2023) \
  This work proposes GCDM, a geometry-complete diffusion model that achieves new state-of-the-art results for 3D molecule diffusion generation and optimization by leveraging the representation learning strengths offered by GNNs that perform geometry-complete message-passing. 

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
