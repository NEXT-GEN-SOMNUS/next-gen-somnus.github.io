---
layout: wp
number: 2
name: Attention mechanisms
description: Developing deep learning algorithms based on attention mechanisms to enable robust and efficient identification of multiple event types within PSG data.
image_path: /assets/img/wp/wp_2.png
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
  color: #0056b3; /* Darker blue for step headings */
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
        <p>Development of <strong>Deep Learning algorithms</strong> for detection of different sleep events, overcoming limitations of current approaches.</p>
      </div>
    </li>
    <li>
      <div class="step-marker">2</div>
      <div class="step-content">
        <p>Integration of <strong>Transformers</strong> within the PSG analysis framework due to their ability to model complex time series dynamics without sequential analysis.</p>
      </div>
    </li>
    <li>
      <div class="step-marker">3</div>
      <div class="step-content">
        <p>Use the <strong>Perceiver architecture</strong> to reduce space complexity by adding a cross-attention layer between the input sequence and multi-headed attention.</p>
      </div>
    </li>
    <li>
      <div class="step-marker">4</div>
      <div class="step-content">
        <p>Further <strong>refinement</strong>: use the Perceiver(IO) for complex outputs</p>
      </div>
    </li>
  </ol>
</div>

In this WP we are going to develop deep learning attention mechanisms algorithms to allow concurrent and individual identification of different types of events in the context of each PSG interval, intending to overcome limitations of current approaches and being more robust, generalizable and computationally efficient. 

Here we plan the integration of Transformers within the PSG analysis framework because they do not analyze inputs sequentially, having therefore the potential of modeling complex time series dynamics. This can be done in several ways that must be studied.

A further step down this line can be taken by considering a prediction problem in which each token represents the value of a single variable per time step. Transformers are then free to attend to the values of any variable at any time in order to produce more accurate predictions. Since the complexity of Transformers might become a limiting factor in our PSG context it is planned to use the Perceiver architecture to reduce space complexity by adding a cross attention layer between the input sequence and multi-headed attention. A supercharged version, namely Perceiver(IO), has also been recently proposed which adds extra cross-attention in the last layer of the decoder, this, in the proposed processing pipeline can allow complex output configuration, including event positioning, which might be a convenient approach for integration of self-attention in the event identification framework.