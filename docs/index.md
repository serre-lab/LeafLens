<div style="display: flex;" class="container-title">
<div class="page-title" style="text-align:left; flex: 0 0 55%">

  <h1 style="text-align: left; font-weight: bold; color: inherit; margin-bottom: 0.2em; font-size:4em"> <span style="letter-spacing: 3px;">Leaf Lens</span></h1>
  <span class="author" style="font-weight: bold; font-size:1em">
  <a href="https://scholar.google.com/citations?user=KotPiIMAAAAJ&hl=en">Ivan Felipe Rodriguez</a><sup>🌿 1</sup>,
  <a href="https://thomasfel.me/">Thomas Fel</a><sup>🌿 2</sup>,
  <a href="https://github.com/gaga1313">Gaurav Gaonkar</a><sup> 1</sup>,
  <a href="https://github.com/gaga1313">Mohit Vaishnav</a><sup> 1</sup>,
  <a href="https://github.com/gaga1313">Herbert Meyer</a><sup> 4</sup>, <br>
  <a href="https://pdw3.myportfolio.com/"> Peter Wilf </a><sup>3</sup> &
  <a href="https://serre-lab.clps.brown.edu/person/thomas-serre/">Thomas Serre</a><sup>1</sup> <br>

  <!--<br>
  <span class="mono"> ivan_felipe_rodriguez@brown.edu; tfel@g.harvard.edu</span> <br>
  -->

  <br>
  <span class="affiliations">
    <sup>🌿</sup> Joint First Authors
    <br>
    <a href="https://serre-lab.clps.brown.edu/">
      <sup>1</sup>
      <img src="./assets/brown.png" class="univ-logo">
      Brown University</a> <br>
    <a href="https://kempnerinstitute.harvard.edu/" class="">
      <sup>2</sup>
      <img src="./assets/harvard.png" class="univ-logo">
      Kempner Institute, Harvard University</a> <br>
    <a href="https://www.upenn.edu/" class="">
      <sup>3</sup>
      <img src="./assets/penn.png" class="univ-logo">
      Pennsylvania State University</a><br>
    <a href="https://www.nps.gov/flfo/index.htm" class="">
      <sup>4</sup>
      <img src="./assets/nps.png" class="univ-logo">
      Florissant Fossil Beds, National Park Service</a>
  </span>



  <br>
  <br>

  <div class="button-style">
    <b><a href="classes/Betulaceae/"> 👋 Start exploring now » </a></b>
  </div>

</div>


<div class="flex-gif">
  <div class="gif-intro" style="width: 300px; height: 300px;">
    <img class="pan-image" src="./assets/little_dico.jpg">
  </div>
</div>

</div>

## Overview

*Leaf Lens* is one of three companion platforms for the study *Advancing Paleobotany with AI-guided Expert Fossil Leaf Identification*. This site focuses on **explainability**: how the network organizes **concepts** and **families** when classifying leaves, using cleared and x-rayed imagery so overlays stay easy to read.

### Companion apps

- **[Hugging Face Fossil App](https://huggingface.co/spaces/Serrelab/fossil_app)** — run the same family-level model on **your own** fossil leaf images in the browser. Fossil training is currently dominated by Florissant; images from other sites are run through the model but predictions may be more variable.

- **[Fossil Leaf Lens](https://serre-lab.github.io/FossilLeafLens/)** — browse **Predicted Fossil Identifications** and per-specimen pages for Florissant fossils (catalog numbers, similar training images, and model concepts for each specimen).

Our deep learning framework mitigates data scarcity by augmenting sparse fossil data with synthetic examples and by aligning extant and fossil leaf domains through representational learning. In the main article, we apply this approach to the late Eocene Florissant flora of Colorado and report well over 90% accuracy for family-level classification across 142 dicot families, compared with a chance level of 3.5%.

For dataset details, model training, fossil analyses, and the rest of the scientific story, see the paper—an **arXiv** preprint is *coming soon* (we will add the link here). The dataset is cited in the **Citation** section below.

!!! note "Training data and Leaf Lens"
    Our models are trained on the [Extant and Fossil Leaves dataset](https://phytokeys.pensoft.net/article/72350/list/9/) introduced by [Wilf et al.](https://www.geosc.psu.edu/directory/peter-wilf) (2021, *PhytoKeys*), a curated collection of cleared, x-rayed, and fossil leaf images spanning more than 150 angiosperm families. **Leaf Lens**, however, uses **cleared and x-rayed** images only. Fossil leaves differ sharply in contrast, breakage, matrix, and preservation, which would add variation unrelated to the taxonomic signal we aim to interpret.

---

## Project goals

Our primary objective is to use explainable AI to characterize the concepts that matter most when neural networks classify leaves. By tracing how these networks encode and organize visual information, we aim to:

- Reveal how the model makes decisions and which features it relies on for classification.
- Clarify how biological taxonomy relates to structure in the learned representation space.
- Provide visual, interactive tools for exploring how concepts and families are organized in those representations.

Our system addresses a fundamental challenge: the scarcity of taxonomically vetted fossil specimens. Modern leaf images are abundant, but fossilization—compression, mineralization, fragmentation—induces a difficult domain shift between living and fossil forms. By leveraging explainability methods, we surface internal visual “concepts” that highlight diagnostic patterns that are often hard for human observers to see.

---

## Explore the site

Use the **navigation** (sidebar) to open any **family** or **concept**, or start with the maps below.

### Interactive maps (UMAP)

| | |
| --- | --- |
| **Families** | 142 families in 2D feature space—hover points for details. |
| **Concepts** | 2000+ learned concepts—hover to see how patterns cluster. |

<div class="ll-explore-maps">
<div class="ll-explore-panel">
<p class="ll-explore-panel__label">Family UMAP</p>
<canvas id="scatterClass"></canvas>
</div>
<div class="ll-explore-panel">
<p class="ll-explore-panel__label">Concept UMAP</p>
<canvas id="scatterDico"></canvas>
</div>
</div>

### Family (class) pages

Per family: **representative samples**, **concept visualizations** (what matters for that family), and **activation heatmaps**.

### Concept pages

Per concept: **feature visualizations**, **top 10** images with strongest activation, and notes on each concept’s **role** in classification.

### Suggested flow

1. Pan and hover the **maps** above.
2. Open a **family** in the nav for specimen- and heatmap-level detail.
3. Open a **concept** for the pattern-level view.

---

## Broader implications

Using concept-based interpretability, we surface botanically meaningful cues by visually summarizing subtle morphological features that define families across fossil and extant specimens—suggesting new diagnostic characters.

We have applied our system to more than 1,700 previously unidentified Florissant fossils; expert paleobotanists report that many predictions are intriguing or plausible candidates for follow-up study.

We invite you to explore the results, interact with the visualizations, and engage with this work on concept learning.

## Citation

If you use **Leaf Lens** in your research, please cite:

```latex
@article{rodriguez2025fossils,
  title   = {Advancing Paleobotany with AI-guided Expert Fossil Leaf Identification},
  author  = {Rodriguez, Ivan Felipe and Fel, Thomas and Gaonkar, Gaurav and
             Vaishnav, Mohit and Meyer, Herbert and Wilf, Peter and Serre, Thomas},
  year    = {2025},
  note    = {arXiv preprint: coming soon}
}
```

This work also uses the following dataset:

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


<script src="https://cdnjs.cloudflare.com/ajax/libs/Chart.js/3.8.0/chart.min.js" integrity="sha512-sW/w8s4RWTdFFSduOTGtk4isV1+190E/GghVffMA9XczdJ2MDzSzLEubKAs5h0wzgSJOQTRYyaz73L3d6RtJSg==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>

<script src="js/class_umap.js"></script>
<script src="js/dico_umap.js"></script>
