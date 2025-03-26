<div class="candidate-buttons">
  <button data-target="canning-section">Canning</button>
  <button data-target="curtin-section">Curtin</button>
  <button data-target="flinders-section">Flinders</button>
  <button data-target="wa-liberal-section">WA Liberal Candidates</button>
</div>

<div id="canning-section">
  <h1>Canning</h1>
  <h3>90 Days</h3>
  {% raw %}
  <div id="fb-root"></div>
  <script async defer src="https://connect.facebook.net/en_US/sdk.js#xfbml=1&version=v7.0"></script>
  <div class="fb-ad-library-spend-tracker" data-country="AU" data-page-ids="948595148496917,498624823340124" data-time-preset="last_90_days" data-width="500"></div>
  {% endraw %}
  <br>
  <br>
  <h3>7 Days</h3>
  {% raw %}
  <div id="fb-root"></div>
  <script async defer src="https://connect.facebook.net/en_US/sdk.js#xfbml=1&version=v7.0"></script>
  <div class="fb-ad-library-spend-tracker" data-country="AU" data-page-ids="948595148496917,498624823340124" data-time-preset="last_7_days" data-width="500"></div>
  {% endraw %}
  <br>
</div>

<div id="curtin-section" style="display: none;">
  <h1>Curtin</h1>
  <h3>90 Days</h3>
  {% raw %}
  <div id="fb-root"></div>
  <script async defer src="https://connect.facebook.net/en_US/sdk.js#xfbml=1&version=v7.0"></script>
  <div class="fb-ad-library-spend-tracker" data-country="AU" data-page-ids="289373994253840,110679918187811" data-time-preset="last_90_days" data-width="500"></div>
  {% endraw %}
  <br>
  <br>
  <h3>7 Days</h3>
  {% raw %}
  <div id="fb-root"></div>
  <script async defer src="https://connect.facebook.net/en_US/sdk.js#xfbml=1&version=v7.0"></script>
  <div class="fb-ad-library-spend-tracker" data-country="AU" data-page-ids="289373994253840,110679918187811" data-time-preset="last_7_days" data-width="500"></div>
  {% endraw %}
  <br>
</div>

<div id="flinders-section" style="display: none;">
  <h1>Flinders</h1>
  <h3>90 Days</h3>
  {% raw %}
  <div id="fb-root"></div>
<script async defer src="https://connect.facebook.net/en_US/sdk.js#xfbml=1&version=v7.0"></script>
<div class="fb-ad-library-spend-tracker" data-country="AU" data-page-ids="503830579480432,103943488824397" data-time-preset="last_90_days" data-width="500"></div>
  {% endraw %}
  <br>
  <br>
  <h3>7 Days</h3>
  {% raw %}
  <div id="fb-root"></div>
<script async defer src="https://connect.facebook.net/en_US/sdk.js#xfbml=1&version=v7.0"></script>
<div class="fb-ad-library-spend-tracker" data-country="AU" data-page-ids="503830579480432,103943488824397" data-time-preset="last_7_days" data-width="500"></div>
  {% endraw %}
  <br>
</div>

<div id="wa-liberal-section" style="display: none;">
  <h1>WA Liberal Candidates</h1>
  <h3>90 Days</h3>
  {% raw %}
  <div id="fb-root"></div>
  <script async defer src="https://connect.facebook.net/en_US/sdk.js#xfbml=1&version=v7.0"></script>
  <div class="fb-ad-library-spend-tracker" data-country="AU" data-page-ids="289373994253840,262340686960375,948595148496917,357223777483754,442693582252181,346201718577605,776811619361742,428271723699770,146533948886081,125627804305487" data-time-preset="last_90_days" data-width="500"></div>
  {% endraw %}
  <br>
  <br>
  <h3>7 Days</h3>
  {% raw %}
  <div id="fb-root"></div>
  <script async defer src="https://connect.facebook.net/en_US/sdk.js#xfbml=1&version=v7.0"></script>
  <div class="fb-ad-library-spend-tracker" data-country="AU" data-page-ids="289373994253840,262340686960375,948595148496917,357223777483754,442693582252181,346201718577605,776811619361742,428271723699770,146533948886081,125627804305487" data-time-preset="last_7_days" data-width="500"></div>
  {% endraw %}
  <br>
</div>

document.querySelectorAll('.candidate-buttons button').forEach(function(button) {
  button.addEventListener('click', function() {
    // Hide all sections
    document.querySelectorAll(".candidate-section").forEach(function(section) {
      section.style.display = "none";
    });
    // Show the target section
    var target = this.getAttribute('data-target');
    document.getElementById(target).style.display = "block";
  });
});
