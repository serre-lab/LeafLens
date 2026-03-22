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

##  Overview

Leaf Lens is one of the three companion platform to our study "Advancing Paleobotany with AI-guided Expert Fossil Leaf Identification". This website provides an interactive exploration of how deep neural networks learn to classify fossil angiosperm leaves—one of paleobotany's most persistent challenges.

Our deep learning framework overcomes data scarcity by augmenting sparse fossil data with synthetic examples and aligning extant and fossil leaf domains through representational learning. In the primary article we demonstrate this approach on the late Eocene Florissant flora of Colorado, achieving well over 90% accuracy for family-level classification across 142 dicot families—compared to a chance level of just 3.5%.

For dataset details, model training, fossil analyses, and the rest of the scientific story, see the paper—arXiv coming soon (link will be added here). The dataset reference is under Citation below.

---

## Project Goals

Our primary objective is to leverage Explainable AI techniques to understand the concepts that matter most for neural networks when classifying leaves. By revealing these concepts, we aim to provide:


By tracing how these networks encode and organize visual information, we aim to:

- Insights into the model's decision-making process, identifying the key features used for classification.
- A deeper understanding of the relationships between biological taxonomy and computational representations.
- Visual and interactive tools for exploring how concepts and families are structured within the learned representations.

Our system addresses a fundamental challenge: the extreme scarcity of taxonomically vetted fossil specimens. While modern leaf specimens are abundant, fossilization processes—compression, mineralization, fragmentation—create a challenging domain shift between living and fossil forms. By leveraging explainability techniques, we identify internal visual "concepts" that reveal diagnostic patterns difficult for human observers to discern.

---

## Explore the website

1. **Interactive UMAP Visualizations:**
   - **2,000+ Concepts:** Explore how the network organizes learned concepts in a 2D UMAP projection. Each point represents a distinct concept, clustered based on similarity. Hover over clusters for details.
   - **150+ Classes:** See how the leaf families relate to one another in the feature space through an interactive UMAP plot. Gain insights into class-level similarities and separations.

   **Visualizations (interactive plots will be embedded here):**

   **Family visualization:**
   <canvas id="scatterClass"></canvas>

   **Concepts visualization:**
   <canvas id="scatterDico"></canvas>


2. **Class-Specific Pages:**
   - For each of the 150+ leaf families, a dedicated page includes:
     - **Representative samples** from the dataset.
     - **Concept visualizations** that highlight the features most critical for classifying leaves in this family.
     - **Activation heatmaps** showing how the neural network processes these leaves.

3. **Concept-Specific Pages:**
   - Each of the 2,000+ discovered concepts has its own page, detailing:
     - **Feature visualizations** representing the concept.
     - The **top 10 leaf images** that activate the concept most strongly.
     - **Insights into the concept's role** in classifying specific leaf families.

---

## Navigating the Investigation

- Begin with the **UMAP Visualizations** to explore the relationships between concepts and classes.
- Dive deeper into **Class Pages** to learn about specific leaf families and the features the model uses to classify them.
- Explore the **Concept Pages** for an in-depth look at the learned concepts and their biological or computational significance.

---

## Broader Implications

Using concept-based interpretability methods, our system surfaces botanically meaningful cues by visually summarizing subtle morphological features that define families across fossil and extant specimens, suggesting new diagnostic characters.

We have already applied our system to over 1,700 previously unidentified Florissant fossils, with expert paleobotanists finding a high proportion of the predictions to be intriguing or plausible candidates for detailed follow-up studies.

We invite you to explore the findings, interact with the visualizations, and engage with this collaborative exploration into concept learning.

## Citation

If you make use of **Leaf Lens** in your research, please cite:

```latex
@article{rodriguez2025fossils,
  title   = {Advancing Paleobotany with AI-guided Expert Fossil Leaf Identification},
  author  = {Rodriguez, Ivan Felipe and Fel, Thomas and Gaonkar, Gaurav and
             Vaishnav, Mohit and Meyer, Herbert and Wilf, Peter and Serre, Thomas},
  year    = {2025}
  note    = {arXiv preprint: coming soon}
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


<script src="https://cdnjs.cloudflare.com/ajax/libs/Chart.js/3.8.0/chart.min.js" integrity="sha512-sW/w8s4RWTdFFSduOTGtk4isV1+190E/GghVffMA9XczdJ2MDzSzLEubKAs5h0wzgSJOQTRYyaz73L3d6RtJSg==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>

<script src="js/class_umap.js"></script>
<script src="js/dico_umap.js"></script>