---
layout: wp
number: 6
name: Evaluation of the prototype in the clinical setting
description: Integrate developed solutions into a scalable, generalizable model using heterogeneous datasets, testing ensemble strategies, and evaluating performance in clinical settings. 
image_path: /assets/img/wp/wp_6.png
---

<style>
/* --- CSS for Horizontal Development Stream --- */
.wp-horizontal-stream-container {
  max-width: 1200px; /* Wider container for horizontal flow */
  margin: 50px auto;
  padding: 30px;
  background-color: #fbfdff; /* Very light background */
  border-radius: 15px;
  box-shadow: 0 12px 40px rgba(0,0,0,0.08);
}

.horizontal-stream-roadmap {
  display: flex; /* Key: Use flexbox for horizontal arrangement */
  justify-content: space-between; /* Distribute items evenly */
  align-items: flex-start; /* Align content blocks to the top */
  position: relative;
  padding: 50px 20px 20px; /* Padding for the top line and space */
  overflow-x: auto; /* Allow horizontal scrolling on small screens if needed */
  scroll-behavior: smooth;
}

/* The central horizontal line of the stream */
.horizontal-stream-roadmap::before {
  content: '';
  position: absolute;
  top: 70px; /* Position line below markers */
  left: 0;
  right: 0;
  height: 3px; /* Thickness of the line */
  background-color: #aeb6bf; /* Medium gray line */
  z-index: 0; /* Behind the markers */
}

.stream-point {
  display: flex;
  flex-direction: column; /* Stack marker and content vertically */
  align-items: center; /* Center marker and content horizontally */
  text-align: center;
  flex-shrink: 0; /* Prevent points from shrinking in a narrow container */
  width: 25%; /* Each point takes a quarter of the width initially */
  max-width: 280px; /* Max width for each point to prevent too wide */
  padding: 0 10px; /* Internal padding for spacing */
  position: relative;
}

.stream-marker {
  width: 50px;
  height: 50px;
  background-color: #1f374f; /* Blue for marker */
  color: #d1dceb;
  border-radius: 50%;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-shrink: 0;
  position: relative; /* Relative to stream-point */
  top: 0; /* Align with top of content area */
  z-index: 1; /* Above the line */
  box-shadow: 0 3px 10px rgba(0,0,0,0.2);
  margin-bottom: 20px; /* Space between marker and content */
}

/* Line from marker to horizontal stream line */
.stream-marker::after {
  content: '';
  position: absolute;
  bottom: -20px; /* Position below the marker */
  left: 50%;
  transform: translateX(-50%);
  width: 2px; /* Vertical line from marker */
  height: 20px; /* Length of the vertical line */
  background-color: #aeb6bf; /* Same color as horizontal line */
  z-index: -1; /* Behind marker, but above horizontal line */
}

.stream-content {
  background-color: #ffffff;
  border: 1px solid #d8e6ef;
  border-radius: 10px;
  padding: 20px 15px;
  font-size: 0.8em;
  box-shadow: 0 5px 15px rgba(0,0,0,0.1);
  flex-grow: 1; /* Allow content to grow if needed */
  transition: transform 0.2s ease-in-out, box-shadow 0.2s ease-in-out;
}

.stream-content p {
  line-height: 1.5;
  margin-bottom: 0;
}
</style>


<div class="wp-horizontal-stream-container">
  <div class="horizontal-stream-roadmap">
    <div class="stream-point">
      <div class="stream-marker">1</div>
      <div class="stream-content">
        <p>Model integration and scalability</p>
      </div>
    </div>
    <div class="stream-point">
      <div class="stream-marker">2</div>
      <div class="stream-content">
        <p>Clinical performance validation</p>
      </div>
    </div>
    <div class="stream-point">
      <div class="stream-marker">3</div>
      <div class="stream-content">
        <p>Usability analysis and AI application</p>
      </div>
    </div>
    <div class="stream-point">
      <div class="stream-marker">4</div>
      <div class="stream-content">
        <p>Technology demonstrator development</p>
      </div>
    </div>
  </div>
</div> 

In this WP we intend to <strong>integrate the developed solutions</strong> into a scalable and generalizable model, using the several heterogeneous datasets gathered. Different strategies for ensemble combinations of local models will be tested and compared. 

Performance will also be <strong>analyzed in the clinical setting</strong> with the idea of advancing towards a demonstration prototype, using the experience of one of the PIs in dealing with this kind of systems (the Polyman scoring software) used in the daily clinical routine of a sleep specialized hospital, and considered as a reference tool for many clinical researchers worldwide.