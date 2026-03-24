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

<label for="point-slider">Selection:</label>
<input type="range" id="point-slider" min="0" max="2" value="0" step="1">
<p id="slider-text">Option A</p>

const slider = document.getElementById('point-slider');
const textDisplay = document.getElementById('slider-text');
const messages = ["Option A", "Option B", "Option C"];

slider.addEventListener('input', function() {
    textDisplay.textContent = messages[this.value];
});
