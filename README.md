<h1 align="center">
  <img src="https://github.com/serre-lab/LeafLens/blob/main/logo.png" width=42px> Leaf Lens
</h1>

<p align="center">
  Ivan Felipe Rodriguez<sup>1🌿</sup>,
  Thomas Fel<sup>1,2🌿</sup>,
  Gaurav Gaonkar<sup>1</sup>,
  Mohit Vaishnav<sup>1</sup>,
  Herbert Meyer<sup>3</sup>, <br>
  Peter Wilf<sup>4 🍂</sup>,
  Thomas Serre<sup>1 🍂</sup>
</p>

<p align="left">
  🌿 Joint First Authors <br>
  🍂 Corresponding Authors
  <br>
  <sup>1</sup> Department of Cognitive, Linguistic and Psychological Sciences, Brown University
  <br>
  <sup>2</sup> Kempner Institute, Harvard University
  <br>
  <sup>3</sup> Florissant Fossil Beds National Monument, National Park Service
  <br>
  <sup>4</sup> Department of Geosciences, Pennsylvania State University
</p>



<p align="center">
  <a href="https://serre-lab.github.io/LeafLens/">
    <img src="https://img.shields.io/badge/Visit-Leaf%20Lens-2e7d32?style=for-the-badge&logo=leaflet&logoColor=white">
  </a>
</p>

<p align="center">
  Explore fossil classification, concepts, and model interpretability.
</p>


<h1 align="center">
  <img src="https://github.com/serre-lab/LeafLens/blob/main/little_dico.jpg" width=800px>
</h1>


## Overview

*Leaf Lens* is the companion platform to our study *Decoding Fossil Floras with Artificial Intelligence: An application to the Florissant Formation (2025)*.
It explores how deep neural networks learn and structure concepts when classifying fossil and modern leaves at the level of the angiosperm family.

The models are trained on the [Extant and Fossil Leaves dataset](https://phytokeys.pensoft.net/article/72350/list/9/) introduced by [Wilf et al.](https://www.geosc.psu.edu/directory/peter-wilf), a comprehensive, curated collection of cleared, x-rayed, and fossil leaf images spanning more than 150 angiosperm families.
Using Explainable AI methods, *Leaf Lens* examines how internal representations—initially opaque feature spaces—crystallize into visual concepts, activation maps, and taxonomic structures that echo botanical organization.


## Goals

- Clarify which morphological features guide neural classification of leaves
- Relate computational representations to established biological taxonomy
- Provide interactive access to fossil data and model explanations


## Features

- Interactive visualizations of over 2,000 learned concepts and their relations in embedding space
- Class-level exploration of 150+ plant families with representative samples and explanatory maps
- Concept pages presenting feature visualizations, top activating examples, and their taxonomic relevance
- Comparisons between real fossils and high-fidelity synthetic fossils used for generative augmentation


## Broader Significance

Leaf Lens exemplifies how explainable artificial intelligence can be applied in scientific domains. By exposing the internal geometry of deep representations, it connects machine-learned features with biological structure. Beyond the Florissant Formation, the approach opens large fossil collections to systematic analysis, offering tools to uncover diagnostic features that have remained inaccessible to manual inspection.


## Citation

If you make use of Leaf Lens in your research, please cite:

```latex
@article{rodriguez2025fossils,
  title   = {Decoding Fossil Floras with Artificial Intelligence:
             An application to the Florissant Formation},
  author  = {Rodriguez, Ivan Felipe and Fel, Thomas and Gaonkar, Gaurav and
             Vaishnav, Mohit and Meyer, Herbert and Wilf, Peter and Serre, Thomas},
  year    = {2025}
}
```

This work also makes use of the following dataset:

```latex
@article{wilf2021leaves,
  title   = {An image dataset of cleared, x-rayed, and fossil leaves vetted to plant family for human and machine learning},
  author  = {Wilf, Peter and Wing, Scott L. and Meyer, Herbert W. and Rose, Jacob A. and Saha, Rohit and Serre, Thomas and Cúneo, N. Rubén and Donovan, Michael P. and Erwin, Diane M. and Gandolfo, Maria A. and Gonzalez-Akre, Erika and Herrera, Fabiany and Hu, Shusheng and Iglesias, Ari and Johnson, Kirk R. and Karim, Talia S. and Zou, Xiaoyu},
  journal = {phytokeys},
  volume  = {187},
  pages   = {93--128},
  year    = {2021},
  doi     = {10.3897/phytokeys.187.72350}
}
```
