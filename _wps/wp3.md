---
layout: wp
number: 3
name: Human-in-the-loop approach
description: Human-in-the-loop strategies, including Curriculum Learning, Active Learning, and Interactive Machine Learning, to enhance model training through expert feedback and dynamic data selection based on case difficulty.
image_path: /assets/img/wp/wp_3.png
---


<style>
/* --- CSS for Streamlined Process Flow --- */
.wp-streamlined-flow-container {
  max-width: 900px;
  margin: 50px auto;
  padding: 30px;
  text-align: center;
  font-size: 0.8em;
}

.process-flow-diagram {
  display: flex;
  flex-wrap: wrap; /* Allow items to wrap on smaller screens */
  justify-content: center;
  align-items: center; /* Vertically center items in a row */
  gap: 20px; /* Space between elements */
  padding: 10px;
}

.flow-stage, .flow-result {
  border: 1px solid #e0e0e0;
  border-radius: 8px;
  padding: 15px 20px;
  box-shadow: 0 2px 8px rgba(0,0,0,0.05);
  flex: 1 1 200px; /* Allow items to grow/shrink, min-width 200px */
  max-width: 250px; /* Max width to keep them concise */
  display: flex;
  flex-direction: column;
  align-items: center;
  text-align: center;
  min-height: 120px; /* Ensure consistent height for alignment */
  justify-content: center;
}

.flow-stage h4, .flow-result h4 {
  margin-top: 0;
  margin-bottom: 8px;
  font-size: 1.1em;
  line-height: 1.3;
}

.flow-stage p, .flow-result p {
  line-height: 1.4;
  margin-bottom: 0;
}

.flow-arrow {
  font-size: 2.5em; /* Large arrow size */
  color: #b0c4de; /* Muted blue for arrows */
  flex-shrink: 0; /* Prevent arrows from shrinking */
  margin: 0 5px; /* Small horizontal margin */
}

.loop-arrow {
  font-size: 4em; /* Larger for the loop arrow */
  color: #b0c4de; /* More prominent blue */
  margin-top: 10px; /* Push down slightly if wrapping */
  font-family: 'Roboto', sans-serif;
}

.flow-result {
  background-color: #e8f5e9; /* Light green for the result */
  border-color: #c8e6c9;
}

.wp-flow-summary {
  margin-top: 40px;
  padding: 25px;
  background-color: #d1dceb;
  border-radius: 10px;
  text-align: justify;
  line-height: 1.6;
}

/* Responsive adjustments */
@media (max-width: 850px) {
  .process-flow-diagram {
    flex-direction: column; /* Stack all items vertically */
    gap: 15px; /* Reduce gap when stacked */
  }
  .flow-stage, .flow-result {
    max-width: 90%; /* Take more width when stacked */
    min-height: auto; /* Allow height to adjust */
  }
  .flow-arrow {
    transform: rotate(90deg); /* Rotate arrows to point downwards */
    margin: 10px 0; /* Vertical margin for stacked arrows */
  }
  .loop-arrow {
    transform: rotate(90deg); /* Keep loop arrow pointing downwards */
  }
}

</style>

<div class="wp-streamlined-flow-container">
  <div class="process-flow-diagram">
    <div class="flow-stage">
      <h4>Model training</h4>
      <p>Initial model training and generalization of patterns from data.</p>
    </div>
    <span class="flow-arrow">&#10140;</span> <div class="flow-stage">
      <h4>Curriculum Learning</h4>
      <p>Organizing datasets by difficulty, expert disagreements measure complexity.</p>
    </div>
    <span class="flow-arrow">&#10140;</span> <div class="flow-stage">
      <h4>Active Learning</h4>
      <p>System queries experts for the most informative cases to label.</p>
    </div>
    <span class="flow-arrow">&#10140;</span> <div class="flow-stage">
      <h4>Interactive Machine Learning</h4>
      <p>Experts provide fluid feedback, correcting errors and offering unprompted insights.</p>
    </div>
    <span class="flow-arrow loop-arrow">&#8635;</span> <div class="flow-result">
      <h4>Enhanced model performance</h4>
      <p>Achieving a more robust, generalizable, and efficient AI model.</p>
    </div>
  </div>
</div>

This WP integrates advanced Human-in-the-Loop (HITL) approaches, including Curriculum Learning and Active Learning, evolving towards Interactive Machine Learning (IML). The core objective is to significantly enhance model performance through continuous, expert-driven feedback.