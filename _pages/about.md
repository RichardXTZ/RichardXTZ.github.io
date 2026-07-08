---
layout: default
title: About
permalink: /
subtitle:
nav: false
nav_order: 1
---

<style>
  .home {
    max-width: 860px;
    margin: 0 auto;
    padding: 2.2rem 0 1.5rem;
    line-height: 1.65;
    font-family: "Roboto", Arial, sans-serif;
    font-size: 1.1rem;
  }

  .home h1 {
    font-size: 2.8rem;
  }

  .home h2 {
    margin-top: 2rem;
    font-family: "Roboto", Arial, sans-serif;
    font-size: 1.8rem;
  }

  .home a,
  footer a {
    color: #b509ac !important;
    font-weight: 700;
    text-decoration: none;
  }

  .home a:hover,
  footer a:hover {
    color: #8f087f !important;
    text-decoration: underline;
  }

  .navbar a,
  .navbar-brand,
  .navbar-nav a {
    color: #b509ac !important;
    font-weight: 700 !important;
  }

  .navbar a:hover,
  .navbar-brand:hover,
  .navbar-nav a:hover {
    color: #8f087f !important;
  }

  .home-header {
    display: grid;
    grid-template-columns: minmax(0, 1fr) 250px;
    gap: 2rem;
    align-items: start;
  }

  .contact-links {
    margin: 0.7rem 0 0;
    text-align: center;
    font-size: 1.2rem;
  }

  .contact-links a,
  .paper-links a {
    white-space: nowrap;
  }

  .home-photo {
    width: 250px;
    border-radius: 2px;
    display: block;
    height: auto;
    box-shadow: 4px 4px 10px rgba(0, 0, 0, 0.18);
  }

  .home-aside {
    width: 250px;
  }

  .publication-note {
    margin: 0.25rem 0 1rem;
    color: var(--global-text-color-light);
  }

  .publication-list {
    margin: 0;
    padding-left: 1.35rem;
  }

  .publication-list li {
    margin-bottom: 1.15rem;
  }

  .publications .periodical {
    font-size: 1rem;
  }

  .paper-title {
    font-weight: 500;
  }

  .paper-authors {
    margin-top: 0.2rem;
  }

  .paper-links {
    margin-top: 0.25rem;
  }

  .publications {
    margin-top: 0.5rem;
  }

  .publications h2.bibliography {
    margin-top: 0.8rem !important;
    padding-top: 0.5rem !important;
  }

  @media (max-width: 640px) {
    .home-header {
      display: block;
    }

    .home-photo {
      width: 150px;
      margin: 0 0 1rem;
    }

    .home-aside {
      width: 150px;
      margin-bottom: 1rem;
    }

    .contact-links {
      text-align: left;
      margin-top: -0.4rem;
    }
  }

  .publications ol.bibliography li .preview {
    width: 120px !important;
    max-width: 120px !important;
    height: auto !important;
  }
</style>

<main class="home">
  <div class="home-header">
    <section>
      <h1>Tianzhi Xiang</h1>

      <p>I am an M.S. candidate in Mechanics at Tianjin University, advised by Prof. <a href="https://scholar.google.com.hk/citations?user=oob-8JwAAAAJ&hl=zh-CN">Yanfeng Wang</a>. I received my B.Eng. in Engineering Mechanics from Tianjin University. Currently I am fortunate to work with Prof. <a href="https://scholar.google.com/citations?user=4sE5xgwAAAAJ&hl=en">Johan Christensen</a> at <a href="https://materials.imdea.org/">IMDEA Materials Institute</a>.</p>

      <p>My research focuses on acoustic metasurfaces and vibro-acoustic wave manipulation, with an emphasis on efficient wave transmission across strongly impedance-mismatched interfaces.</p>
    </section>

    <aside class="home-aside">
      <img class="home-photo" src="/assets/img/prof_pic.jpg" alt="Tianzhi Xiang" />

      <p class="contact-links">
        <a href="mailto:xiangtz@tju.edu.com">Email</a> |
        <a href="/assets/pdf/cv.pdf">CV</a> |
        <a href="https://github.com/RichardXTZ">GitHub</a>
      </p>
    </aside>
  </div>

  <h2>Publications</h2>

  <!-- <p class="publication-note">* means equal contribution</p> -->

  <div class="publications">
    {% bibliography --query @*[selected=true] %}
  </div>
</main>
