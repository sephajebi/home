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

<b>Organizers:</b> <b><a href="https://sites.google.com/view/lior-gishboliner/home">Lior Gishboliner</a></b> and <b><a href="https://www.sepehrhajebi.com">Sepehr Hajebi</a></b>.
<div style="height: 15px;"></div>

<div style="width: 100%; text-align: justify; margin-bottom:0.8em">
<b>About:</b> This is a combinatorics seminar with little to no pressure from the clock: talk can comfortably run for up 90 minutes (anf sometimes longer).
</div>

<div style="width: 100%; text-align: justify; margin-bottom:0.8em">
<b>Format:</b> Talks are held on Zoom and will be recorded and posted online. The seminar will run in seasons of 8-10 talks, for as long as speakers and audiences can be found. The schedule for Season 1 is below.
</div>

<div style="width: 100%; text-align: justify; margin-bottom:0.8em">
<b>Mailing list:</b> Announcements, Zoom links, and passwords will be sent to the seminar’s mailing list. To join the list, please email <a href="mailto:sepehr.hajebi@utoronto.ca">this</a> address.
</div>

<blockquote>
Season 1
</blockquote>
