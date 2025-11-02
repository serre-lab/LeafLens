<h1 align="center">
  <img src="https://github.com/serre-lab/LeafLens/blob/main/logo.png" width=42px> Leaf Lens
</h1>

<p align="center">
  Ivan Felipe Rodriguez<sup>1🌿</sup>,
  Thomas Fel<sup>1,2🌿</sup>,
  Gaurav Gaonkar<sup>1</sup>,
  Mohit Vaishnav<sup>1</sup>,
  Herbert Meyer<sup>3</sup>, <br>
  Peter Wilf<sup>4</sup>,
  Thomas Serre<sup>1🍂</sup>
</p>

<p align="center">
  <a href="https://serre.lab.brown.edu/"><img src="https://github.com/serre-lab/LeafLens/blob/gh-pages/assets/brown.png?raw=true" height="30"></a>
  &nbsp;&nbsp;
  <a href="https://kempnerinstitute.harvard.edu/"><img src="https://github.com/serre-lab/LeafLens/blob/gh-pages/assets/harvard.png?raw=true" height="30"></a>
  &nbsp;&nbsp;
  <a href="https://www.nps.gov/flfo/index.htm"><img src="https://github.com/serre-lab/LeafLens/blob/gh-pages/assets/nps.png?raw=true" height="30"></a>
  &nbsp;&nbsp;
  <a href="https://www.upenn.edu/"><img src="https://github.com/serre-lab/LeafLens/blob/gh-pages/assets/penn.png?raw=true" height="30"></a>
</p>

<p align="left">
  <sup>1</sup> Center for Computational Brain Science, Brown University
  <br>
  <sup>2</sup> Kempner Institute, Harvard University
  <br>
  <sup>3</sup> Florissant Fossil Beds National Monument, National Park Service
  <br>
  <sup>4</sup> Department of Geosciences, Pennsylvania State University
  <br><br>
  🌿 Joint first authors&nbsp;&nbsp;|&nbsp;&nbsp;🍂 Corresponding author
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

**Leaf Lens** is the companion platform to our study *"Decoding Fossil Leaves with Artificial Intelligence: An application to the Florissant Formation"*. This website provides an interactive exploration of how deep neural networks learn to classify fossil angiosperm leaves—one of paleobotany's most persistent challenges.

Our deep learning framework overcomes data scarcity by augmenting sparse fossil data with synthetic examples and aligning extant and fossil leaf domains through representational learning. We demonstrate this approach on the late Eocene **Florissant flora of Colorado**, achieving **well over 90% accuracy** for family-level classification across **142 dicot angiosperm families**—compared to a chance level of just 3.5%.


## Project goals

Our primary objective is to leverage Explainable AI techniques to understand the **concepts that matter most** for neural networks when classifying leaves. By revealing these concepts, we aim to provide:

- **Insights into the model's decision-making process,** identifying the key features used for classification
- A deeper understanding of the relationships between **biological taxonomy and computational representations**
- **Visual and interactive tools** for exploring how concepts and families are structured within the learned representations

Our system addresses a fundamental challenge: the extreme scarcity of taxonomically vetted fossil specimens. While modern leaf specimens are abundant, fossilization processes—compression, mineralization, fragmentation—create a challenging domain shift between living and fossil forms.


## Key highlights

- **Number of families:** 142 dicot angiosperm families
- **Total dataset:** Over 34,000 images (extant and fossil leaves)
- **Florissant fossils:** 3,200 taxonomically vetted specimens spanning 23 families
- **Classification performance:** Well over 90% top-5 accuracy (chance: 3.5%)
- **Discovered concepts:** 2,000+ unique visual concepts extracted via sparse dictionary learning

## Features

- Interactive visualizations of over 2,000 learned concepts and their relations in embedding space
- Family-level exploration of 142 dicot families with representative samples and explanatory maps
- Concept pages presenting feature visualizations, top activating examples, and their taxonomic relevance
- Comparisons between real fossils and high-fidelity synthetic fossils used for generative augmentation


## Broader implications

This research advances one of paleobotany's central challenges—accurate identification of fossil angiosperm leaves—and demonstrates how state-of-the-art AI can be applied to scientific domains with limited training data. Using concept-based interpretability methods, our system surfaces botanically meaningful cues by visually summarizing subtle morphological features that define families across fossil and extant specimens, suggesting new diagnostic characters.

Beyond the Florissant Formation, this cross-domain strategy is readily generalizable to other fossil deposits, positioning this approach for broad use in understanding the evolution and ecological dynamics of ancient terrestrial ecosystems.


## Funding and acknowledgments

This material is based upon work supported by the U.S. **National Science Foundation** under Award No. **EAR-1925481** (T.S.) and **EAR-1925755** (P.W.), and by **ANR-3IA Artificial and Natural Intelligence Toulouse Institute** (**ANR-19-PI3A-0004**).

Computing support was provided by the Center for Computation and Visualization (CCV) at Brown University (via NIH Office of the Director grant S10OD025181). We also acknowledge Google's Cloud TPU hardware resources via the TensorFlow Research Cloud (TFRC) program.

## Citations

If you make use of Leaf Lens in your research, please cite:

```bibtex
@article{rodriguez2025fossils,
  title  = {Decoding Fossil Leaves with Artificial Intelligence:
            An application to the Florissant Formation},
  author = {Rodriguez, Ivan Felipe and Fel, Thomas and Gaonkar, Gaurav and
            Vaishnav, Mohit and Meyer, Herbert and Wilf, Peter and Serre, Thomas},
  year   = {2025}
}
```

This work also makes use of the following dataset:

```bibtex
@article{wilf2021leaves,
  title   = {An image dataset of cleared, x-rayed, and fossil leaves vetted to plant family for human and machine learning},
  author  = {Wilf, Peter and Wing, Scott L. and Meyer, Herbert W. and Rose, Jacob A. and Saha, Rohit and Serre, Thomas and Cúneo, N. Rubén and Donovan, Michael P. and Erwin, Diane M. and Gandolfo, Maria A. and Gonzalez-Akre, Erika and Herrera, Fabiany and Hu, Shusheng and Iglesias, Ari and Johnson, Kirk R. and Karim, Talia S. and Zou, Xiaoyu},
  journal = {PhytoKeys},
  volume  = {187},
  pages   = {93--128},
  year    = {2021},
  doi     = {10.3897/phytokeys.187.72350}
}
```
