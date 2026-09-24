<div align="center">
  <h1>Person360: Diffusion-Guided 3D Gaussian Splatting <br> for Static 360-Degree Portrait Reconstruction</h1>

  **Cunqi Wu** · **Minhao Lin** · **Jianchao Wang** · **Peng Zhou** · **Jie Qin**

  College of Artificial Intelligence, Nanjing University of Aeronautics and Astronautics

  <a href="https://devin100086.github.io/person360-page/"><img src="https://img.shields.io/badge/Project_Page-Person360-green" alt="Project Page"></a>

<p align="center">
  <img src="assets/teaser.jpg" alt="Person360 reconstruction results" width="92%" />
</p>
</div>

 ## TODOs

[ ] Clean up the code and release it as open source.

## Method

Person360 uses a scene-specific diffusion prior to restore portrait details during 3D Gaussian Splatting optimization. Its iterative render-edit-refresh strategy updates close-up supervision as the reconstruction evolves, while bilateral-grid appearance correction and SfM-anchored sparse depth regularization help reduce appearance drift and stabilize geometry.

<p align="center">
  <img src="assets/pipeline.jpg" alt="Person360 pipeline" width="92%" />
</p>

## Software

<div class="col-md-8 col-md-offset-2">
  <h4>Interactive Viewer Demos</h4>
  <div align="center">
    <div style="display: inline-block; width: 49%; vertical-align: top;">
      <h4>Desktop Software</h4>
      <img src="assets/software/software.gif" alt="Person360 desktop software demo" width="100%" style="aspect-ratio: 16 / 9; object-fit: cover; padding: 2px;">
    </div>
    <div style="display: inline-block; width: 49%; vertical-align: top;">
      <h4>Mobile App</h4>
      <img src="assets/software/app.gif" alt="Person360 mobile app demo" width="100%" style="aspect-ratio: 16 / 9; object-fit: cover; padding: 2px;">
    </div>
  </div>
</div>

## Render comparisons

Qualitative render comparisons on 360-degree portrait scenes. The clips below show Person360 alongside a static reconstruction baseline and a dynamic reconstruction baseline.

### Static Method Comparison

<p align="center">
  <img src="assets/comparison/label-3dgs.svg" alt="3DGS" width="49%">
  <img src="assets/comparison/label-person360.svg" alt="Person360 (ours)" width="49%"><br>
  <img src="assets/comparison/scene1/3dgs.gif" alt="Scene 1 rendered with 3DGS (left)" width="49%">
  <img src="assets/comparison/scene1/person360.gif" alt="Scene 1 rendered with Person360 (right)" width="49%">
</p>

### Dynamic Method Comparison

<p align="center">
  <img src="assets/comparison/label-4dgs.svg" alt="4DGS" width="49%">
  <img src="assets/comparison/label-person360.svg" alt="Person360 (ours)" width="49%"><br>
  <img src="assets/comparison/scene2/4dgs.gif" alt="Scene 2 rendered with 4DGS (left)" width="49%">
  <img src="assets/comparison/scene2/person360.gif" alt="Scene 2 rendered with Person360 (right)" width="49%">
</p>
