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

/* Speaker, Title, Abstract and Recording */

.speaker,
.title,
.abstract,
.recording {
  margin-top: 4px;
}

/* Speaker and Title */

.speaker,
.title {
  display: flex;
  align-items: flex-start;
}

/* Speaker and Title icons */

.speaker i,
.title i {
  width: 18px;
  margin-right: 3px;
  text-align: center;
  flex-shrink: 0;
  line-height: inherit;
}

/* Speaker and Title text */

.speaker-text,
.talk-title {
  flex: 1;
  min-width: 0;
  text-align: justify;
}

/* Abstract and Recording */

.abstract summary,
.recording summary {
  cursor: pointer;
  list-style: none;
  width: fit-content;
}

.abstract summary::-webkit-details-marker,
.recording summary::-webkit-details-marker {
  display: none;
}

/* Abstract and Recording text */

.abstract summary span,
.recording summary span {
  /*color: #1c4587;*/
  text-decoration: none;
}

.abstract summary:hover span,
.recording summary:hover span {
  /*color: #1c4587;*/
  text-decoration: underline;
}

/* Abstract and Recording icons */

.abstract summary i,
.recording summary i {
  width: 18px;
  margin-right: 3px;
  text-align: center;
  /*color: #1c4587;*/
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


<!-- Seminar information below this line. -->




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
<b>Schedule:</b> The seminar will run in rounds of 8-10 talks, for as long as speakers and audiences can be found. The schedule for Round 1 is below.
</div>

<div style="width: 100%; text-align: justify; margin-bottom:3em">
<b>Mailing list:</b> Announcements and Zoom information for the talks are sent to the seminar’s mailing list. To join the list, please email <b><a href="mailto:sepehr.hajebi@utoronto.ca">this</a></b> address.
</div>


<blockquote>
Round 1 (2026)
</blockquote>
<div style="height: -3px;"></div>

Tuesdays at 10:00 a.m. ET, October 6 to December 1 (except October 27).
<div style="height: 30px;"></div>

<div class="talk">
<div class="talk">



<div class="speaker">
  <i class="fa-solid fa-user"></i>
  <span class="speaker-text">
    <b>Speaker:</b> <b><a href="https://web.math.princeton.edu/~pds/">Paul Seymour</a></b> (Princeton University)
  </span>
</div>

<div class="title">
  <i class="fa-solid fa-tag"></i>
  <span class="talk-title">
    <b>Title:</b> TBA.
  </span>
</div>
<div style="height: 10px;"></div>



<div class="talk">

  <div>
    <b>October 13</b>
  </div>

  <div>
    <b>Speaker:</b> <b><a href="https://people.math.ethz.ch/~sudakovb/">Benny Sudakov</a></b> (ETH Zürich)
    <div style="height: 7px;"></div>
<div class="talk-title">
  <b>Title:</b> The Mihail-Vazirani conjecture and strong edge-expansion in random 0/1 polytopes
</div>
    <div style="height: 3px;"></div>
<details class="abstract">
  <summary>
    <i class="fa-regular fa-file-lines"></i><span><b>Abstract</b></span>
  </summary>
  <div class="abstract-text">
We study the edge-expansion of the graph of a random \(0/1\) polytope \(P^d_p\), the convex hull of a random subset of \(\{0,1\}^d\) obtained by retaining each point independently with probability \(p\). This problem, introduced by Gillmann and Kaibel more than twenty years ago, has since attracted substantial attention. We prove that, for every fixed \(\varepsilon>0\) and every \(p\in(0,1-\varepsilon]\), the graph of \(P^d_p\) has edge-expansion \(\Theta(d)\) with high probability, improving the previous best bound of Ferber, Krivelevich, Sales and Samotij and verifying the Mihail--Vazirani conjecture for random \(0/1\) polytopes in a strong form. We further show that the behavior changes sharply at \(p=1/2\): for every fixed \(\varepsilon>0\) and integer \(k\ge 2\), if \(p\le 1/2-\varepsilon\), then the edge-expansion is \(\Omega(d^k)\) with high probability. Thus, random \(0/1\) polytopes exhibit a striking expansion phase transition at \(p=1/2\).
<div style="height: 3px;"></div>
    
This is joint work with Micha Christoph, Sahar Diskin, Lyuben Lichev.
  </div>
</details>
    <div style="height: 3px;"></div>
    <details class="recording">
  <summary>
    <i class="fa-brands fa-youtube"></i><span><b>Recording</b></span>
  </summary>
  TBA
      
<!--<div class="video-container">
    <iframe
      src="https://www.youtube.com/embed/3CzRUhi9KFo?rel=0"
      title="YouTube video player"
      loading="lazy"
      allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
      allowfullscreen>
    </iframe></div>-->
  
</details>
  </div>
</div>
<div style="height: 10px;"></div>





<div class="talk">

  <div>
    <b>October 20</b>
  </div>

  <div>
    <b>Speaker:</b> <b><a href="https://sites.google.com/view/oliver-janzer/home">Oliver Janzer</a></b> (EPFL)
    <div style="height: 7px;"></div>
    <div class="talk-title">
  <b>Title:</b> TBA
</div>
    <div style="height: 3px;"></div>
<details class="abstract">
  <summary>
    <i class="fa-regular fa-file-lines"></i><span><b>Abstract</b></span>
  </summary>
  <div class="abstract-text">
    TBA
  </div>
</details>
    <div style="height: 3px;"></div>
    <details class="recording">
  <summary>
    <i class="fa-brands fa-youtube"></i><span><b>Recording</b></span>
  </summary>
  TBA
      
<!--<div class="video-container">
    <iframe
      src="https://www.youtube.com/embed/3CzRUhi9KFo?rel=0"
      title="YouTube video player"
      loading="lazy"
      allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
      allowfullscreen>
    </iframe></div>-->
  
</details>
  </div>

</div>
<div style="height: 10px;"></div>





<div class="talk">

  <div>
    <b>November 3</b>
  </div>

  <div>
    <b>Speaker:</b> <b><a href="https://shohamlet.github.io">Shoham Letzter</a></b> (University College London)
    <div style="height: 7px;"></div>
    <div class="talk-title">
  <b>Title:</b> TBA
</div>
    <div style="height: 3px;"></div>
<details class="abstract">
  <summary>
    <i class="fa-regular fa-file-lines"></i><span><b>Abstract</b></span>
  </summary>
  <div class="abstract-text">
    TBA
  </div>
</details>
    <div style="height: 3px;"></div>
    <details class="recording">
  <summary>
    <i class="fa-brands fa-youtube"></i><span><b>Recording</b></span>
  </summary>
  TBA
      
<!--<div class="video-container">
    <iframe
      src="https://www.youtube.com/embed/3CzRUhi9KFo?rel=0"
      title="YouTube video player"
      loading="lazy"
      allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
      allowfullscreen>
    </iframe></div>-->
  
</details>
  </div>

</div>
<div style="height: 10px;"></div>





<div class="talk">

  <div>
    <b>November 10</b>
  </div>

  <div>
    <b>Speaker:</b> <b><a href="https://sites.google.com/site/sophiespirkl/">Sophie Spirkl</a></b> (University of Waterloo)
    <div style="height: 7px;"></div>
    <div class="talk-title">
  <b>Title:</b> Cliques and coloring in tournaments
</div>
    <div style="height: 3px;"></div>
<details class="abstract">
  <summary>
    <i class="fa-regular fa-file-lines"></i><span><b>Abstract</b></span>
  </summary>
  <div class="abstract-text">
    Tournaments are orientations of complete graphs, and many graph theory questions -- in particular, from the world of induced subgraphs -- have analogues in tournaments. In particular, notions of colouring (due to Neumann-Lara) and clique number (Aboulker, Aubian, Charbit, Lopes) exist. I will tell you what these are, as well as some of what we know about them, and questions that remain.
  </div>
</details>
    <div style="height: 3px;"></div>
    <details class="recording">
  <summary>
    <i class="fa-brands fa-youtube"></i><span><b>Recording</b></span>
  </summary>
  TBA
      
<!--<div class="video-container">
    <iframe
      src="https://www.youtube.com/embed/3CzRUhi9KFo?rel=0"
      title="YouTube video player"
      loading="lazy"
      allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
      allowfullscreen>
    </iframe></div>-->
  
</details>
  </div>

</div>
<div style="height: 10px;"></div>





<div class="talk">

  <div>
    <b>November 17</b>
  </div>

  <div>
    <b>Speaker:</b> <b><a href="https://sites.google.com/view/domagoj-bradac/">Domagoj Bradač</a></b> (ETH Zürich)
    <div style="height: 7px;"></div>
    <div class="talk-title">
  <b>Title:</b> TBA
</div>
    <div style="height: 3px;"></div>
<details class="abstract">
  <summary>
    <i class="fa-regular fa-file-lines"></i><span><b>Abstract</b></span>
  </summary>
  <div class="abstract-text">
    TBA
  </div>
</details>
    <div style="height: 3px;"></div>
    <details class="recording">
  <summary>
    <i class="fa-brands fa-youtube"></i><span><b>Recording</b></span>
  </summary>
  TBA
      
<!--<div class="video-container">
    <iframe
      src="https://www.youtube.com/embed/3CzRUhi9KFo?rel=0"
      title="YouTube video player"
      loading="lazy"
      allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
      allowfullscreen>
    </iframe></div>-->
  
</details>
  </div>

</div>
<div style="height: 10px;"></div>





<div class="talk">

  <div>
    <b>November 24</b>
  </div>

  <div>
    <b>Speaker:</b> <b><a href="https://web.math.princeton.edu/~mchudnov/">Maria Chudnovsky</a></b> (Princeton University)
    <div style="height: 7px;"></div>
    <div class="talk-title">
  <b>Title:</b> TBA
</div>
    <div style="height: 3px;"></div>
<details class="abstract">
  <summary>
    <i class="fa-regular fa-file-lines"></i><span><b>Abstract</b></span>
  </summary>
  <div class="abstract-text">
    TBA
  </div>
</details>
    <div style="height: 3px;"></div>
    <details class="recording">
  <summary>
    <i class="fa-brands fa-youtube"></i><span><b>Recording</b></span>
  </summary>
  TBA
      
<!--<div class="video-container">
    <iframe
      src="https://www.youtube.com/embed/3CzRUhi9KFo?rel=0"
      title="YouTube video player"
      loading="lazy"
      allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
      allowfullscreen>
    </iframe></div>-->
  
</details>
  </div>

</div>
<div style="height: 10px;"></div>





<div class="talk">

  <div>
    <b>December 1</b>
  </div>

  <div>
    <b>Speaker:</b> <b><a href="https://robiscounting.github.io">Rob Morris</a></b> (IMPA)
    <div style="height: 7px;"></div>
    <div class="talk-title">
  <b>Title:</b> TBA
</div>
    <div style="height: 3px;"></div>
<details class="abstract">
  <summary>
    <i class="fa-regular fa-file-lines"></i><span><b>Abstract</b></span>
  </summary>
  <div class="abstract-text">
    TBA
  </div>
</details>
    <div style="height: 3px;"></div>
    <details class="recording">
  <summary>
    <i class="fa-brands fa-youtube"></i><span><b>Recording</b></span>
  </summary>
  TBA
      
<!--<div class="video-container">
    <iframe
      src="https://www.youtube.com/embed/3CzRUhi9KFo?rel=0"
      title="YouTube video player"
      loading="lazy"
      allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
      allowfullscreen>
    </iframe></div>-->
  
</details>
  </div>

</div>



