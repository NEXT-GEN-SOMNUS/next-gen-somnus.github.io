---
layout: wp
number: 4
name: Quantum-Machine Learning approach
description: Quantum machine learning for biomedical signals, focusing on data encoding, quantum model design, and integrating attention mechanisms to enable transformer-like architectures.
image_path: /assets/img/wp/wp_4.png
---

<style>
  /* --- CSS for Simple Milestone Pathway Diagram --- */
  .wp-simple-path-container {
    display: flex;
    justify-content: space-around; /* Distributes items evenly */
    align-items: flex; /* Aligns content to the top of each box */
    flex-wrap: wrap; /* Allows items to wrap onto the next line on small screens */
    margin: 30px 0;
    padding: 20px;
  }

  .wp-path-step {
    flex: 1; /* Each step takes equal space */
    min-width: 200px; /* Minimum width before wrapping */
    margin: 13px; /* Space around each step */
    padding: 15px;
    border: 1px solid #dcdcdc; /* Subtle border */
    border-radius: 7px;
    box-shadow: 0 2px 5px rgba(0,0,0,0.05); /* Light shadow for depth */
    text-align: center;
    position: relative;

  }

  /* Optional: Simple arrow between steps */
  .wp-path-step:not(:last-child)::after {
    content: '→'; /* Right arrow */
    position: absolute;
    right: -30px; /* Position to the right of the box */
    top: 50%;
    transform: translateY(-50%);
    font-size: 2em;
    z-index: 1;
    /* Hide arrow if items wrap (basic responsiveness) */
    display: none;
  }

  /* Show arrow only when there's enough space for inline flow */
  @media (min-width: 768px) {
    .wp-path-step:not(:last-child)::after {
      display: block;
    }
  }
  /* box title */
  .wp-path-step h5 {
    font-size: 0.9em;
    margin-top: 0;
    margin-bottom: 10px;
    padding-bottom: 5px;
    border-bottom: 1px dashed #e0e0e0; /* Dashed line under title */
  }

  /* box body */
  .wp-path-step p {
    font-size: 0.75em;
    line-height: 1.4;
    margin-bottom: 0;
  }

</style>

<div class="wp-simple-path-container">
  <div class="wp-path-step">
    <h5>QML applicability and data encoding</h5>
    <p>Investigate QML for biomedical signals and encode data into a quantum system.</p>
  </div>
  <div class="wp-path-step">
    <h5>Quantum feature map construction</h5>
    <p>Construct a quantum feature map that's hard to simulate classically for potential quantum advantage.</p>
  </div>
  <div class="wp-path-step">
    <h5>QNNs (Ansatz) or Quantum Kernels</h5>
    <p>Develop either parameterized quantum circuits (Ansatz) for quantum neural networks or use quantum kernels for kernel methods.</p>
  </div>
  <div class="wp-path-step">
    <h5>Attention layers</h5>
    <p>Analyze introducing attention layers to quantum models to move towards Transformer-like architectures.</p>
  </div>
</div>


This WP investigates the applicability of quantum machine learning (QML) to biomedical signal processing, trying to use the quantum properties to obtain a better understanding of complex correlations in high-dimensional data. This process will be carried out in parallel with the previous WPs dedicated to next-generation ML algorithms, searching for synergies between them. 