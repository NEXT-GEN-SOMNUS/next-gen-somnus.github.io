---
layout: wp
number: 5
name: Explainability
description: Integrate explainability into ML models using self-attention mechanisms, visualizing attention over PSG signals, and incorporating model-agnostic methods.
image_path: /assets/img/wp/wp_5.png
---


<style>
/* --- CSS for Progress Path List --- */

.wp-progress-list-container {
  max-width: 800px;
  margin: 40px auto;
  padding: 25px;
  background-color: #fcfcfc;
  border-radius: 10px;
  box-shadow: 0 5px 20px rgba(0,0,0,0.06);
}

.wp-progress-list-container h3 {
  text-align: center;
  margin-bottom: 30px;
  border-bottom: 2px solid #e0e0e0;
  padding-bottom: 15px;
}

.wp-progress-list {
  list-style: none; /* Remove default list bullets/numbers */
  padding: 0;
  margin: 0;
  position: relative; /* For the connecting line */
}

/* The vertical connecting line */
.wp-progress-list::before {
  content: '';
  position: absolute;
  left: 30px; /* Position line to the left of markers */
  top: 0;
  bottom: 0;
  width: 2px; /* Thickness of the line */
  background-color: #d0d0d0; /* Light gray line */
  z-index: 0; /* Behind the markers */
}

.wp-progress-list li {
  display: flex; /* Use flexbox for marker and content */
  align-items: flex-start; /* Align marker and content to the top */
  margin-bottom: 25px; /* Space between list items */
  position: relative;
  padding-left: 70px; /* Space for the marker */
}

.wp-progress-list li:last-child {
  margin-bottom: 0; /* No bottom margin for the last item */
}

.step-marker {
  width: 40px;
  height: 40px;
  background-color: #d1dceb; /* Blue background for marker */
  color: #1f374f;
  border-radius: 50%; /* Circular marker */
  display: flex;
  justify-content: center;
  align-items: center;
  font-weight: bold;
  flex-shrink: 0; /* Prevent marker from shrinking */
  position: absolute; /* Position marker over the line */
  left: 10px; /* Adjust to sit on the line */
  top: 0; /* Align with top of content */
  z-index: 1; /* Above the line */
  box-shadow: 0 2px 5px rgba(0,0,0,0.2);
}

.step-content {
  flex-grow: 1; /* Allows content to take remaining space */
  padding-left: 20px; /* Space between marker and content */
}

.step-content h4 {
  margin-top: 0;
  margin-bottom: 8px;
}

.step-content p {
  font-size: 0.95em;
  line-height: 1.6;
  margin-bottom: 0;
}

/* Responsive adjustments */
@media (max-width: 600px) {
  .wp-progress-list::before {
    left: 25px; /* Adjust line position */
  }
  .wp-progress-list li {
    padding-left: 60px; /* Adjust padding for smaller screens */
    margin-bottom: 20px;
  }
  .step-marker {
    width: 35px;
    height: 35px;
    left: 8px; /* Adjust marker position */
    font-size: 1.1em;
  }
}
</style>


<div class="wp-progress-list-container">
  <ol class="wp-progress-list">
    <li>
      <div class="step-marker">1</div>
      <div class="step-content">
        <h4>Self-Attention for Model-Specific Explainability</h4>
        <p>Leveraging self-attention mechanisms to inherently include explainability by relating elements along the input sequence. This addresses the opaqueness of deep learning models.</p>
      </div>
    </li>
    <li>
      <div class="step-marker">2</div>
      <div class="step-content">
        <h4>Visualizing Attention Scores</h4>
        <p>Producing visual representations by coloring specific signal intervals based on their attention scores, providing clinicians with intuitive feedback on model focus.</p>
      </div>
    </li>
    <li>
      <div class="step-marker">3</div>
      <div class="step-content">
        <h4>Model-Agnostic Explainability</h4>
        <p>Incorporating model-agnostic explainability techniques, independent of the ML model used, such as LIME (Local Interpretable Model-Agnostic Explanations) and SHAP (SHapley Additive exPlanations).</p>
      </div>
    </li>
    <li>
      <div class="step-marker">4</div>
      <div class="step-content">
        <h4>Human-in-the-Loop (HITL) for Explanation Refinement</h4>
        <p>Improving explainability with HITL techniques: human experts review and numerically score explanation quality, feeding into a Bayesian optimization process for hyperparameter adjustment.</p>
      </div>
    </li>
  </ol>
</div>



Explainability is one of the most important parts of any machine learning design today. The problem with deep learning is that the developed models are mostly opaque. Using self-attention mechanisms allow us to include model-specific explainability capabilities, because self-attention learns a representation by relating elements at different positions along the input sequence. Attention scores can be used to expand interpretability of the model by mapping them back to the input signals.

In this regard, we aim to produce a visual representation by coloring the specific signal intervals with an intensity proportional to their associated attention scores, therefore providing the clinician with valuable and intuitive feedback about how the model is scoring the PSG.