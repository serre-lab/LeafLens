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

## Explore Leaf Lens

!!! abstract "Get started"
    *Leaf Lens* is the interactive companion to our study of how deep neural networks learn concepts for leaf classification. This page sends you straight into the visual exploration tools.
    
    For the complete scientific background—dataset details, model training, and fossil analyses—see the **main article** and the linked dataset paper below.

---

### What you can do

| Action | Description |
|--------|-------------|
| **Explore concepts** | 2D maps showing how the network organizes leaf patterns in feature space |
| **Browse families** | Class pages with representative leaves and the features that matter most |
| **Inspect concepts** | Individual concept pages with example leaves that activate each pattern |

!!! note "Extant leaves only"
    The interactive UMAP visualizations on this page use **extant (modern) leaf images only**. Fossil leaves and their interpretation are covered in the main article and fossil-focused pages elsewhere on the site.

---

### Visualizations

**Family visualization**
<canvas id="scatterClass"></canvas>

**Concepts visualization**
<canvas id="scatterDico"></canvas>

---

### Citation

If you make use of **Leaf Lens** in your research, please cite:

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


<script src="https://cdnjs.cloudflare.com/ajax/libs/Chart.js/3.8.0/chart.min.js" integrity="sha512-sW/w8s4RWTdFFSduOTGtk4isV1+190E/GghVffMA9XczdJ2MDzSzLEubKAs5h0wzgSJOQTRYyaz73L3d6RtJSg==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>

<script src="js/class_umap.js"></script>
<script src="js/dico_umap.js"></script>