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
  <!-- Radio Buttons -->
  <input type="radio" name="slider" id="slide1" checked>
  <input type="radio" name="slider" id="slide2">
  
  <!-- Slides -->
  <div class="slides">
    <div class="slide" id="content1">Text 1: Welcome!</div>
    <div class="slide" id="content2">Text 2: Learn More</div>
  </div>
  
  <!-- Navigation -->
  <div class="nav">
    <label for="slide1">1</label>
    <label for="slide2">2</label>
  </div>
</div>


.slides {
  display: flex;
  overflow: hidden;
}

.slide {
  display: none; /* Hide all slides by default */
  width: 100%;
}

/* Show slide based on checked radio button */
#slide1:checked ~ .slides #content1,
#slide2:checked ~ .slides #content2 {
  display: block;
}

/* Optional: Simple navigation styling */
.nav { text-align: center; }
.nav label { cursor: pointer; padding: 10px; }
