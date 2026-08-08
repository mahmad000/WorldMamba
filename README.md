# WorldMamba: World-State Representation Learning for Hyperspectral Image Classification[https://ieeexplore.ieee.org/document/11640768]

<img width="5082" height="1974" alt="WorldMamba" src="https://github.com/user-attachments/assets/6eb72ec5-460a-4811-ade2-9320ed084047" />

# Overview
WorldMamba formulates hyperspectral image classification (HSIC) as a
world-state inference problem rather than conventional discriminative
feature learning. Instead of relying on a single latent representation,
the proposed framework learns three complementary world states:
-   Material State – captures class-specific spectral composition through prototype-based representation learning.
-   Scene State – models contextual spatial organization and long-range spectral-spatial dependencies.
-   Physical State – learns intrinsic physical variations using variance-covariance regularization.
A lightweight 3D spectral-spatial tokenizer converts hyperspectral patches into latent tokens, which are processed by a Vision Mamba encoder. The learned world states are adaptively fused to generate the final prediction.
------------------------------------------------------------------------
# Framework
The complete WorldMamba architecture consists of:
1.  3D Spectral-Spatial Tokenizer
2.  Vision Mamba World Encoder
3.  Material State Branch
4.  Scene State Branch
5.  Physical State Branch
6.  Adaptive World-State Fusion
7.  Multi-Objective Optimization
------------------------------------------------------------------------
Highlights
-   Novel world-state representation learning framework for HSIC.
-   Vision Mamba backbone for efficient long-range spectral-spatial modeling.
-   Prototype-based material representation learning.
-   Context-aware scene modeling.
-   Physically regularized latent representation learning.
-   Adaptive fusion of complementary latent states.
-   State-of-the-art performance on multiple hyperspectral benchmarks.
------------------------------------------------------------------------
# Datasets
Experiments are conducted on:
-   University of Houston 2013 (UH13)
-   Dioni (DI)
-   Loukia (LK)
The datasets are publicly available from: https://hsi.yale.edu/resource/681

------------------------------------------------------------------------
# Results
WorldMamba consistently outperforms recent Mamba-based HSIC methods on
UH13, Dioni, and Loukia datasets by learning structured latent world
representations instead of a single discriminative embedding.

------------------------------------------------------------------------
# Citation
    @ARTICLE{11640768,
  author={Ahmad, Muhammad and Maslovskaya, Anna and Mazzara, Manuel},
  journal={IEEE Geoscience and Remote Sensing Letters}, 
  title={WorldMamba: World-State Representation Learning for Hyperspectral Image Classification}, 
  year={2026},
  volume={},
  number={},
  pages={1-1},
  doi={10.1109/LGRS.2026.3719470}}

## If you find this repository useful, please consider starring it and citing our paper.
