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

<!-- Font Awesome icons -->
<link rel="stylesheet"
href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.2/css/all.min.css">

<style>
.talk {
  display: grid;
  grid-template-columns: 100px 1fr;
  column-gap: 20px;
  width: 55%;
  margin-bottom: 2em;
}

/* Mobile */
@media (max-width: 768px) {
  .talk {
    width: 97%;
    grid-template-columns: 75px 1fr;
    column-gap: 12px;
  }
}

/* Abstract and Recording */

.abstract,
.recording {
  margin-top: 4px;
}

.abstract summary,
.recording summary {
  cursor: pointer;
  list-style: none;
  color: #1c4587;
  width: fit-content;
}

.abstract summary::-webkit-details-marker,
.recording summary::-webkit-details-marker {
  display: none;
}

/* Underline on hover */

.abstract summary:hover span,
.recording summary:hover span {
  text-decoration: underline;
}

/* Icons */

.abstract summary i,
.recording summary i {
  width: 18px;
  margin-right: 3px;
  text-align: center;
  color: #1c4587;
}
  
  /* Abstract */

  .talk-title {
  text-align: justify;
}

/* Abstract */

.abstract-text {
  margin-top: 7px;
  width: 100%;
  line-height: 1.4;
  text-align: justify;
}

/* YouTube player */

.video-container {
  margin-top: 7px;
  width: 100%;
  aspect-ratio: 16 / 9;
}

.video-container iframe {
  display: block;
  width: 100%;
  height: 100%;
  border: 0;
}
</style>


<blockquote>
Season 1 (2026)
</blockquote>

<div class="talk">

  <div>
    <b>October 6</b>
  </div>

  <div>
    <b>Time:</b> 10:00 AM ET<br>
       <div style="height: 7px;"></div>
    <b>Speaker:</b> Paul Seymour
    <div style="height: 7px;"></div>
    <div class="talk-title">
  <b>Title:</b> TBA.
</div>
    <div style="height: 7px;"></div>
    <details class="abstract">
      <summary>
  <i class="fa-regular fa-file-lines"></i><span><b>Abstract</b></span>
</summary>
      <div class="abstract-text">
        This is the abstract of the talk. The text will automatically
        wrap within this width.
      </div>
    </details>
    <div style="height: 7px;"></div>
    <details class="recording">
     <summary>
  <i class="fa-brands fa-youtube"></i><b>Recording</b>
</summary>
      <div class="video-container">
        <iframe
          src="https://www.youtube.com/embed/3CzRUhi9KFo?rel=0"
          title="YouTube video player"
          loading="lazy"
          allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
          allowfullscreen>
        </iframe>
      </div>
    </details>
  </div>

</div>
