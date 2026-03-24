# philosopat.github.io

<p>National Park database, itinerary collection, etc.</p>

<p><strong>Grand Canyon National Park</strong><p>
<p>Ideal # of days: 3</p>
<p>Half Day Itinerary: take Desert View Drive, climb the Desert View Watchtower</p>
<p>1 Day Itinerary: </p>
<p>2 Day Itinerary:</p>
<p>3 Day Itinerary:</p>
<p>4 Day Itinerary:</p>
<p>5+ Day Itinierary:</p>

<p><strong>Grand Teton National Park</strong></p>

<div class="slider-container">
  <label for="rating-slider">Rate your experience:</label>
  <input type="range" id="rating-slider" min="0" max="4" step="1" list="tickmarks" value="2">
  
  <!-- Datalist provides tick marks, but not the dynamic text -->
  <datalist id="tickmarks">
    <option value="0"></option>
    <option value="1"></option>
    <option value="2"></option>
    <option value="3"></option>
    <option value="4"></option>
  </datalist>

  <!-- This span will display the dynamic text -->
  <span id="text-output">Average</span>
</div>

.slider-container {
  width: 80%;
  margin: 20px auto;
  text-align: center;
}

#rating-slider {
  width: 100%;
  margin-top: 10px;
}

#text-output {
  display: block;
  margin-top: 10px;
  font-weight: bold;
  color: #04AA6D; /* Example color */
}

const experienceTexts = ["Very Poor", "Poor", "Average", "Good", "Excellent"];

// Get the slider and output elements
const slider = document.getElementById("rating-slider");
const output = document.getElementById("text-output");

// Display the initial text based on the default value
output.innerHTML = experienceTexts[slider.value];

// Update the text whenever the slider value changes
slider.oninput = function() {
  output.innerHTML = experienceTexts[this.value];
};
