---
layout: page
title: Long Talks in Combinatorics
permalink: /long-talks-in-combinatorics/
nav: false
---

<style>
/* Translucent navy header, on this page only. */
#navbar {
  background: rgba(16, 25, 43, 0.83) !important;
  padding-top: 12px !important;
  padding-bottom: 12px !important;
}

/* Hide the right-hand links and the mobile menu button. */
#navbarNav,
#navbar .navbar-toggler {
  display: none !important;
}

/* Remove any earlier CSS-generated tower and lettering. */
#navbar .navbar-brand::before,
#navbar .navbar-brand::after {
  content: none !important;
  display: none !important;
}

/* Keep the logo container at its existing size. */
#navbar .navbar-brand {
  display: block !important;
  width: 170px;
  max-width: 100%;
  height: auto !important;
  margin: 0 !important;
  padding: 0 !important;
  font-size: 0 !important;
  line-height: 0 !important;
  background: transparent !important;
}

/* Enlarge the logo by 8% without increasing the bar's height. */
#navbar .navbar-brand img {
  display: block;
  width: 100%;
  max-width: 100%;
  height: auto;
  background: transparent !important;
  transform: scale(1.3);
  transform-origin: left center;
}
</style>

<script>
(() => {
  const navbar = document.getElementById("navbar");
  const brand = navbar && navbar.querySelector(".navbar-brand");
  if (!brand) return;

  const logo = document.createElement("img");
  logo.src = {{ '/assets/img/long-talks-logo-white.png' | relative_url | jsonify }};
  logo.alt = "Long Talks in Combinatorics";
  logo.width = 1969;
  logo.height = 469;

  // Replace the original name with the logo.
  brand.replaceChildren(logo);

  // Make the logo link to this seminar page.
  brand.href = {{ '/long-talks-in-combinatorics/' | relative_url | jsonify }};
  brand.setAttribute("aria-label", "Long Talks in Combinatorics");

  // Keep a fixed header from covering the page content.
  function reserveHeaderSpace() {
    if (getComputedStyle(navbar).position === "fixed") {
      document.body.style.paddingTop = navbar.offsetHeight + "px";
    }
  }

  reserveHeaderSpace();
  logo.addEventListener("load", reserveHeaderSpace);
  window.addEventListener("resize", reserveHeaderSpace);
})();
</script>

<!-- Put your seminar information below this line. -->

<div style="width: 100%; text-align: justify; margin-bottom:0.8em">
<b>Organizers:</b> <b><a href="https://sites.google.com/view/lior-gishboliner/home">Lior Gishboliner</a></b> and <b><a href="https://www.sepehrhajebi.com">Sepehr Hajebi</a></b>.
</div>

<div style="width: 100%; text-align: justify; margin-bottom:0.8em">
<b>About:</b> This is a combinatorics seminar with little to no pressure from the clock: talks can comfortably run for up to 90 minutes (and sometimes even longer).
</div>

<div style="width: 100%; text-align: justify; margin-bottom:0.8em">
<b>Format:</b> Talks are held on Zoom and will be recorded and posted online.
</div>


<div style="width: 100%; text-align: justify; margin-bottom:0.8em">
<b>Schedule:</b> The seminar will run in seasons of 8-10 talks, for as long as speakers and audiences can be found. The schedule for Season 1 is below.
</div>

<div style="width: 100%; text-align: justify; margin-bottom:1em">
<b>Mailing list:</b> Announcements and Zoom information for the talks are sent to the seminar’s mailing list. To join the list, please email <b><a href="mailto:sepehr.hajebi@utoronto.ca">this</a></b> address.
</div>

<style>
.talk {
  display: grid;
  grid-template-columns: 100px 1fr;
  column-gap: 20px;
  width: 45%;
  margin-bottom: 2em;
}

/* Abstract */

.abstract {
  margin-top: 4px;
}

.abstract summary {
  cursor: pointer;
  color: #0366d6;
  text-decoration: none;
  list-style: none;
}

.abstract summary::-webkit-details-marker {
  display: none;
}

.abstract summary:hover {
  text-decoration: underline;
}

.abstract-text {
  margin-top: 10px;
  line-height: 1.4;
}

/* Recording */

.recording {
  margin-top: 4px;
}

.recording summary {
  cursor: pointer;
  color: #0366d6;
  text-decoration: none;
  list-style: none;
}

.recording summary::-webkit-details-marker {
  display: none;
}

.recording summary:hover {
  text-decoration: underline;
}

/* YouTube player */

.video-container {
  margin-top: 10px;
  width: 100%;
  aspect-ratio: 16 / 9;
}

.video-container iframe {
  width: 100%;
  height: 100%;
  border: 0;
}
</style>


<blockquote>
Season 1
</blockquote>

<div class="talk">

  <div>
    <b>October 6</b>
  </div>

  <div>
    <b>Time:</b> 10:00 AM ET<br>
    <b>Speaker:</b> Paul Seymour<br>
    <b>Title:</b> Title of the talk
    <details class="abstract">
      <summary><b>Abstract</b></summary>
      <div class="abstract-text">
        This is the abstract of the talk. It can be as long as necessary,
        and the text will automatically wrap within the width of the talk.
      </div>
    </details>
    <details class="recording">
      <summary><b>Recording</b></summary>
      <div class="video-container">
        <iframe
          src="https://www.youtube.com/embed/3CzRUhi9KFo"
          title="YouTube video player"
          allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
          allowfullscreen>
        </iframe>
      </div>
    </details>
  </div>

</div>
