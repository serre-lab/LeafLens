<h1 align="center">
  <img src="https://github.com/serre-lab/LeafLens/blob/main/logo.png" width=42px> Leaf Lens
</h1>

<p align="center">
  Ivan Felipe Rodriguez<sup>1🌿</sup>,
  Thomas Fel<sup>2🌿</sup>,
  Gaurav Gaonkar<sup>1</sup>,
  Peter Wilf<sup>3</sup>,
  Thomas Serre<sup>1</sup>
</p>

<p align="left">
  🌿 Joint First Authors
  <br>
  <sup>1</sup> Brown University
  <br>
  <sup>2</sup> Kempner Institute, Harvard University
  <br>
  <sup>3</sup> Pennsylvania State University
</p>

<p align="center">
  <a href="https://serre-lab.github.io/Leaf-Lens">
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

Leaf Lens is the companion platform to our study *Decoding Fossil Floras with Artificial Intelligence: An application to the Florissant Formation (2025)*.
It investigates how deep neural networks learn and organize concepts for the classification of fossil and extant leaves across more than 150 families.

The site acts as a lens into the model’s representational space: abstract internal features are rendered as visual concepts, activation maps, and class-level structures. This allows both a critical examination of the model’s decision process and a new perspective on the relationship between morphology and taxonomy.


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
