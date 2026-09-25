---
layout: page
title: Long Talks in Combinatorics
permalink: /long-talks-in-combinatorics/
nav: false
---

<style>
/* Hide right-hand navigation */
.navbar-nav {
  display: none !important;
}

/* Hide the normal "Sepehr Hajebi" */
.navbar-brand {
  font-size: 0 !important;
  position: relative;
  display: flex !important;
  align-items: flex-end;
}

/* CN Tower + horizontal stroke of the L */
.navbar-brand::before {
  content: "";
  display: inline-block;

  width: 38px;
  height: 48px;

  margin-right: 1px;

  background-color: currentColor;

  clip-path: polygon(
    /* antenna */
    48% 0%, 52% 0%,
    53% 17%,

    /* upper mast */
    57% 20%,
    57% 31%,

    /* upper observation deck */
    67% 33%,
    70% 37%,
    70% 40%,

    /* main observation deck */
    82% 42%,
    84% 47%,
    82% 52%,
    68% 54%,

    /* shaft */
    62% 100%,

    /* LONG HORIZONTAL FOOT OF THE L */
    100% 100%,
    100% 94%,
    54% 94%,

    /* other side of shaft */
    38% 54%,

    /* observation deck */
    18% 52%,
    16% 47%,
    18% 42%,
    30% 40%,
    30% 37%,
    33% 33%,

    /* upper mast */
    43% 31%,
    43% 20%,
    47% 17%
  );
}

/* Seminar name */
.navbar-brand::after {
  content: "ong Talks in Combinatorics";

  font-family: "Ubuntu", sans-serif !important;
  font-size: 1.25rem !important;
  font-weight: 500;
  line-height: 1;

  margin-left: -2px;
  padding-bottom: 1px;
}
</style>

# Long Talks in Combinatorics

Something should go here...
