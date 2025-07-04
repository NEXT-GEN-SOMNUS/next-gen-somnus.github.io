---
layout: wp
number: 1
name: Data preparation and validation framework
description: Acquiring and preprocessing annotated PSG datasets from various sources using the open EDF standard, assessing inter-database differences, and establishing a baseline for human agreement.
image_path: /assets/img/wp/wp_1.png
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
    <h5>Data acquisition</h5>
    <p>Obtain annotated PSG datasets from various sources.</p>
  </div>

  <div class="wp-path-step">
    <h5>Data preprocessing</h5>
    <p>Resample, normalize and transform for model compatibility.</p>
  </div>

  <div class="wp-path-step">
    <h5>Databases analysis</h5>
    <p>Characterize differences and establish experts agreement.</p>
  </div>

  <div class="wp-path-step">
    <h5>State-of-the-art</h5>
    <p>Analysis of next-generation machine learning techniques.</p>
  </div>
</div>



In this WP we will perform the basic tasks that will allow us to start building the Machine Learning models. Specifically, we will focus on obtaining the annotated PSG datasets from different sources (where usage of the open EDF standard will be key for simple and flexible data exchange and storage from different data sources). This will include also the typical <strong>preprocessing</strong> tasks needed to adapt the raw data into a format that is valid for feeding a Machine Learning model.

Also, since much of these tasks will be done with the collaborating medical institutions, we will take advantage of the close contact with the physicians to establish and <strong>characterize the inter-database differences</strong> and establish a baseline of human agreement. Finally, we will include a state-of-the-art analysis of all the three next-generation Machine Learning techniques that we want to include in the project in relation to the datasets obtained.

